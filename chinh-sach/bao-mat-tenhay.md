---
title: "Bảo mật — Tên Hay"
description: "Chính sách quyền riêng tư của ứng dụng đặt tên phong thủy Tên Hay: kiến trúc local-first + zero-knowledge, tuân thủ Nghị định 13/2023/NĐ-CP."
keywords: ["chính sách bảo mật", "Tên Hay", "đặt tên phong thủy", "local-first", "zero-knowledge", "Nghị định 13/2023"]
slug: bao-mat-tenhay
canonical: "https://nextsmart.vn/chinh-sach/bao-mat-tenhay"
ogTitle: "Chính sách Bảo mật — Tên Hay"
ogDescription: "Tên Hay lưu dữ liệu của bé trên máy bạn, chỉ gửi thông tin ẩn danh khi gọi AI, sao lưu mã hóa end-to-end. Tuân thủ NĐ 13/2023/NĐ-CP."
dateModified: "2026-06-10"
---

**Áp dụng từ:** 10/06/2026 · **Phiên bản:** 1.1
**Đơn vị phát hành:** NextTech Smart Solutions (sau đây gọi là "Chúng tôi")
**Email liên hệ:** [contact@nextsmart.vn](mailto:contact@nextsmart.vn)
**Website:** [https://nextsmart.vn](https://nextsmart.vn)

Chính sách này tham chiếu **Nghị định 13/2023/NĐ-CP** về bảo vệ dữ liệu cá nhân của Việt Nam.

---

## Tóm tắt nhanh

> "Tên Hay" được thiết kế **local-first** + **zero-knowledge**. Dữ liệu của bé lưu trên máy bạn, không gửi lên server. Khi gọi AI, chỉ gửi thông tin **ẩn danh** (Họ, giới tính, năm Can Chi) — không gửi ngày sinh đầy đủ hay tên bé. Sao lưu đám mây là tuỳ chọn và mã hóa end-to-end — chúng tôi không thể đọc nội dung sao lưu của bạn.

---

## 1. Triết lý thiết kế — Privacy by Default

"Tên Hay" được thiết kế theo nguyên tắc **local-first + zero-knowledge**:

- **Sổ Gia Đình lưu hoàn toàn trên máy bạn** (mã hóa SQLite). Chúng tôi không có bản sao.
- **Khi gọi AI, chỉ gửi dữ liệu ẩn danh:** Họ + giới tính + năm Can Chi (dạng tổ hợp văn hóa, ví dụ "Bính Ngọ"), không gửi ngày/tháng sinh, không gửi tên đầy đủ của bé khi gợi ý.
- **Sao lưu đám mây (tuỳ chọn) mã hóa end-to-end:** Máy chủ chỉ lưu bytes đã mã hóa, **chúng tôi không thể giải mã được** dù muốn — bạn nắm khóa duy nhất.

---

## 2. Dữ liệu chúng tôi xử lý

### 2.1. Dữ liệu lưu trên máy bạn

Các dữ liệu sau **không bao giờ rời máy của bạn** trừ khi bạn chủ động bật sao lưu đám mây:

- Họ tên bé, ngày sinh, giới tính (nếu bạn nhập vào Sổ Gia Đình)
- Lịch sử gợi ý + chấm tên
- Cài đặt cá nhân

Đây là **dữ liệu của bạn, trên thiết bị của bạn**. Chúng tôi không can thiệp.

### 2.2. Dữ liệu gửi lên dịch vụ AI

Khi bạn dùng tính năng gợi ý tên hợp phong thủy, ứng dụng gửi **các trường ẩn danh sau** tới dịch vụ AI:

| Trường | Ví dụ | Có identify cá nhân không? |
|---|---|---|
| Họ | "Nguyễn" | Không (~40% dân số VN) |
| Giới tính | "male" | Không |
| Năm Can Chi (đã tính sẵn) | "Bính Ngọ" | Không (hàng triệu người cùng năm) |
| Mệnh chủ | "Thủy" | Không |
| Cung mệnh | "Khảm" | Không |
| Phong cách bạn chọn | "Hiện đại" | Không |

**KHÔNG bao giờ gửi:** ngày/tháng sinh chính xác, tên đầy đủ của bé, tên cha mẹ, địa chỉ, số điện thoại, vị trí, định danh thiết bị.

Theo Điều 2.1 NĐ 13/2023, dữ liệu phải "gắn liền với một cá nhân cụ thể" mới được coi là dữ liệu cá nhân. Payload chúng tôi gửi AI **không identify được bất kỳ ai cụ thể**.

**Lưu ý về tính năng "Chấm điểm tên":** Khi bạn nhập một tên cụ thể để chấm điểm, ứng dụng gửi tên đó + Can Chi tới AI. Nếu đây là tên thật của bé đã sinh, đó được coi là dữ liệu cá nhân — ứng dụng sẽ hỏi đồng ý của bạn trước.

### 2.3. Dữ liệu tài khoản (chỉ khi bạn đăng nhập)

- **Email** (qua Sign in with Apple / Google)
- **User ID nội bộ** (UUID) do Supabase Auth cấp

Đây là dữ liệu cá nhân của **bạn (cha mẹ)**, không phải của bé.

### 2.4. Dữ liệu kỹ thuật ẩn danh

- Crash logs (Sentry, đã loại bỏ PII)
- Số lần gọi AI (ẩn danh, chỉ để áp quota miễn phí)

### 2.5. Dữ liệu chúng tôi KHÔNG thu thập

- ❌ Vị trí địa lý
- ❌ Danh bạ, ảnh, lịch
- ❌ Mã định danh quảng cáo (IDFA/AAID)
- ❌ Tên hoặc thông tin của cha mẹ (ngoài email đăng nhập)
- ❌ Lịch sử duyệt web hay hoạt động ngoài app

---

## 3. Mục đích sử dụng dữ liệu

| Mục đích | Dữ liệu sử dụng | Cơ sở pháp lý |
|---|---|---|
| Gợi ý tên hợp phong thủy | Demographic ẩn danh | Sự đồng ý |
| Chấm điểm tên | Tên + Can Chi | Sự đồng ý rõ ràng |
| Lưu Sổ Gia Đình offline | Toàn bộ thông tin bạn nhập (**trên máy bạn**) | Bạn tự quản lý |
| Sao lưu đám mây (tuỳ chọn) | Bản mã hóa E2E, server không đọc được | Sự đồng ý rõ ràng |
| Khắc phục sự cố | Crash log ẩn danh | Lợi ích chính đáng |

---

## 4. Bên thứ ba xử lý dữ liệu

### 4.1. Nhà cung cấp AI

- **Nhà cung cấp hiện tại:** DeepSeek (máy chủ tại Trung Quốc) hoặc Gemini (Google, máy chủ Singapore) — tuỳ cấu hình tại thời điểm sử dụng.
- **Dữ liệu gửi:** Chỉ demographic ẩn danh như mô tả mục 2.2.
- **Tại sao có Điều 25 NĐ 13/2023:** Vì máy chủ AI đặt ngoài Việt Nam, đây vẫn được xem là chuyển dữ liệu xuyên biên giới — kể cả khi dữ liệu ẩn danh. Chúng tôi hỏi đồng ý của bạn trước khi gọi AI lần đầu.
- **Bạn có thể từ chối:** ứng dụng vẫn dùng được đầy đủ với engine phong thủy offline (rule-based, không gọi AI).

### 4.2. Hạ tầng backend — Supabase

- Region: **Singapore (ap-southeast-1)** — gần Việt Nam, độ trễ thấp.
- Lưu: Cache phong thủy ẩn danh (hash của Can Chi), Sentry crash logs, **ciphertext** mã hóa nếu bạn bật sao lưu.
- Supabase đã ký Data Processing Addendum theo chuẩn quốc tế.

### 4.3. Sentry — Crash reporting

Stack trace + thông tin thiết bị, không kèm dữ liệu cá nhân. Bạn có thể tắt trong **Cài đặt → Quyền riêng tư**.

### 4.4. Apple App Store / Google Play

Khi bạn mua Premium hoặc PDF báo cáo, giao dịch được Apple/Google xử lý hoàn toàn. Chúng tôi chỉ nhận receipt ID, không thấy thông tin thẻ thanh toán.

---

## 5. Mã hóa và bảo mật

- **Local SQLite:** Mã hóa các trường nhạy cảm với **Argon2id + XChaCha20-Poly1305**.
- **Cloud backup (zero-knowledge):** Mã hóa phía client TRƯỚC khi upload. Khóa giải mã chỉ bạn nắm. **Mất mật khẩu = mất data** — chúng tôi không có chức năng "quên mật khẩu" cho sao lưu vì không thể đọc được nội dung.
- **Transport:** HTTPS/TLS 1.3 cho mọi kết nối.
- **Secret keys:** Lưu trong `flutter_secure_storage` (iOS Keychain / Android Keystore).

---

## 6. Thời gian lưu trữ

| Loại dữ liệu | Thời gian lưu |
|---|---|
| Sổ Gia Đình trên máy | Đến khi bạn xóa hoặc gỡ ứng dụng |
| Cache phong thủy ẩn danh | 90 ngày |
| Crash logs (Sentry) | 30 ngày |
| Backup đám mây | Đến khi bạn xóa hoặc xóa tài khoản |
| Tài khoản đã xóa | Xóa vĩnh viễn trong 30 ngày |

---

## 7. Quyền của bạn theo NĐ 13/2023

Bạn có các quyền sau và có thể thực hiện ngay trong ứng dụng tại **Cài đặt → Quyền riêng tư**:

1. **Quyền được biết** (Điều 14) — Đọc chính sách này
2. **Quyền đồng ý / rút lại đồng ý** (Điều 11–12) — Toggle "AI cá nhân hóa (DeepSeek)"
3. **Quyền truy cập** (Điều 15) — Nút "Xuất dữ liệu" → tải JSON toàn bộ dữ liệu của bạn
4. **Quyền chỉnh sửa** (Điều 16) — Sửa thông tin bất cứ lúc nào trong Sổ Gia Đình
5. **Quyền xóa** (Điều 17) — Nút "Xóa tài khoản" — xóa cả dữ liệu local + cloud
6. **Quyền hạn chế xử lý** (Điều 18) — Tắt đồng bộ đám mây / AI cá nhân hóa
7. **Quyền khiếu nại** — Email [privacy@nextsmart.vn](mailto:privacy@nextsmart.vn) hoặc Cục An ninh mạng (A05) Bộ Công an

**Cam kết phản hồi:** Trong vòng 72 giờ làm việc, hoàn tất trong tối đa 30 ngày theo NĐ 13/2023.

---

## 8. Thay đổi chính sách

Mọi thay đổi sẽ được thông báo qua:

- Banner trong ứng dụng khi bạn mở lần kế tiếp.
- Email tới các tài khoản đã đăng ký (nếu thay đổi nghiêm trọng).

Nếu bạn không đồng ý với thay đổi, bạn có thể yêu cầu xóa tài khoản và dữ liệu.

---

## 9. Liên hệ

- **Quyền riêng tư:** [privacy@nextsmart.vn](mailto:privacy@nextsmart.vn)
- **Hỗ trợ chung:** [support@nextsmart.vn](mailto:support@nextsmart.vn)
- **Website:** [https://nextsmart.vn](https://nextsmart.vn)
- **Địa chỉ pháp lý:** Yên Ngưu, Đại Thanh, Hà Nội, Việt Nam

---

*Phiên bản 1.1 — Phản ánh đúng kiến trúc local-first + zero-knowledge. Khuyến nghị có luật sư IT/data law Việt Nam review trước khi công bố chính thức.*
