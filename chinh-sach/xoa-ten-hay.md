---
title: "Xóa tài khoản — Tên Hay"
description: "Hướng dẫn xóa tài khoản và dữ liệu cá nhân trong ứng dụng đặt tên phong thủy Tên Hay, tuân thủ Điều 17 Nghị định 13/2023/NĐ-CP và chính sách User Data Deletion của Google Play / App Store."
keywords: ["xóa tài khoản", "Tên Hay", "xóa dữ liệu", "data deletion", "Nghị định 13/2023", "Google Play"]
slug: xoa-ten-hay
canonical: "https://nextsmart.vn/chinh-sach/xoa-ten-hay"
ogTitle: "Xóa tài khoản & dữ liệu — Tên Hay"
ogDescription: "Cách xóa tài khoản và toàn bộ dữ liệu cá nhân trong ứng dụng Tên Hay: trong app (vài giây) hoặc yêu cầu qua email (tối đa 30 ngày)."
dateModified: "2026-06-11"
---

**Nhà phát hành:** NextTech Smart Solutions
**Hỗ trợ:** [support@nextsmart.vn](mailto:support@nextsmart.vn)
**Quyền riêng tư:** [privacy@nextsmart.vn](mailto:privacy@nextsmart.vn)

---

## Tóm tắt

Bạn có thể xóa tài khoản và toàn bộ dữ liệu cá nhân trong ứng dụng **Tên Hay** bất cứ lúc nào, theo 2 cách:

1. **Trong ứng dụng** (khuyến nghị, nhanh nhất) — vài giây
2. **Yêu cầu qua email** — tối đa 30 ngày

---

## Cách 1 — Xóa trong ứng dụng (recommend)

### Bước 1: Mở Cài đặt

- Mở app **Tên Hay**
- Tap tab **Tôi** (góc dưới phải) → Cài đặt (icon ⚙️)

### Bước 2: Tìm section "Dữ liệu & Quyền riêng tư"

- Scroll xuống section **DỮ LIỆU & QUYỀN RIÊNG TƯ**

### Bước 3: Chọn loại xóa

#### Tuỳ chọn A — Xóa toàn bộ dữ liệu (giữ tài khoản)
- Tap **"Xóa toàn bộ dữ liệu"**
- Confirm trong dialog
- Hành động: xóa Sổ Gia Đình, lịch sử, cài đặt local. Tài khoản (email login) vẫn còn — có thể đăng nhập lại với data trống.

#### Tuỳ chọn B — Xóa tài khoản hoàn toàn
- Tap **"Xóa tài khoản"**
- Confirm trong dialog "Xóa tài khoản?"
- Hành động: xóa cả dữ liệu local + cloud (nếu có sao lưu) + sign out khỏi Supabase
- Trong vòng **30 ngày**, tài khoản và backup cloud bị xóa vĩnh viễn khỏi server

→ Xong. Tài khoản và dữ liệu đã bị xóa.

---

## Cách 2 — Yêu cầu qua email (nếu không thể truy cập app)

Nếu bạn không còn cài đặt app hoặc không truy cập được tài khoản:

### Gửi email tới
[privacy@nextsmart.vn](mailto:privacy@nextsmart.vn)

### Nội dung email mẫu

```
Tiêu đề: Yêu cầu xóa tài khoản Tên Hay

Họ tên: [Họ tên bạn]
Email tài khoản: [Email bạn dùng để đăng nhập Tên Hay]
Lý do xóa: (tuỳ chọn)

Tôi yêu cầu xóa tài khoản và toàn bộ dữ liệu cá nhân của tôi trong ứng dụng Tên Hay theo quy định Điều 17 Nghị định 13/2023/NĐ-CP.
```

### Cam kết phản hồi

- **Trong 72 giờ làm việc**: Chúng tôi xác nhận đã nhận yêu cầu của bạn
- **Trong 30 ngày**: Hoàn tất xóa data theo NĐ 13/2023

---

## Dữ liệu bị xóa

Khi bạn xóa tài khoản, các dữ liệu sau **bị xóa vĩnh viễn**:

| Dữ liệu | Lưu ở đâu | Cách xóa |
|---|---|---|
| Sổ Gia Đình (thông tin các bé) | Local SQLite trên máy bạn | App tự xóa khi bạn tap "Xóa tài khoản" |
| Lịch sử gợi ý tên + chấm điểm | Local SQLite | App tự xóa |
| Cài đặt cá nhân, AI consent | flutter_secure_storage | App tự xóa |
| Tài khoản auth (email login) | Supabase Auth | Backend cascade delete trong 30 ngày |
| Sao lưu đám mây (nếu bật) | Supabase Storage (ciphertext) | Backend cascade delete trong 30 ngày |
| Crash logs (Sentry) | Sentry server | Tự động xóa sau 30 ngày (chu kỳ Sentry) |
| Cache phong thủy ẩn danh | Supabase | Tự động xóa sau 90 ngày — không identify bạn |
| AI usage log (ẩn danh) | Supabase | Tự động xóa sau 30 ngày — không identify bạn |

---

## Dữ liệu KHÔNG bị xóa (giữ lại)

Theo quy định luật pháp, một số dữ liệu phải lưu cho mục đích:

| Loại dữ liệu | Lý do giữ | Thời gian giữ |
|---|---|---|
| Hoá đơn IAP (Premium subscription, PDF report) | Quy định thuế VN + Apple/Google Play | 5 năm theo Luật Thuế |
| Receipt purchase từ Apple/Google | Phải giữ để xử lý refund nếu cần | 5 năm |

⚠️ Lưu ý: Các hoá đơn này **chỉ chứa email + product ID + giá**, không chứa thông tin Sổ Gia Đình hay nội dung sử dụng app.

---

## Sau khi xóa tài khoản

- Bạn không thể khôi phục lại dữ liệu Sổ Gia Đình đã xóa
- Bạn có thể tải app lại và dùng ở chế độ **Khách (Guest mode)** mà không cần tài khoản
- Hoặc đăng ký tài khoản mới với email khác

---

## Liên hệ

- **Quyền riêng tư & yêu cầu xóa:** [privacy@nextsmart.vn](mailto:privacy@nextsmart.vn)
- **Hỗ trợ chung:** [support@nextsmart.vn](mailto:support@nextsmart.vn)
- **Chính sách bảo mật đầy đủ:** [https://nextsmart.vn/chinh-sach/bao-mat-tenhay](https://nextsmart.vn/chinh-sach/bao-mat-tenhay)

---

*Trang này được cung cấp công khai để tuân thủ chính sách User Data deletion của Google Play và App Store.*
