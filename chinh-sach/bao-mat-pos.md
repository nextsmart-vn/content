---
title: "Chính sách Bảo mật — NextSmart POS (QLBH)"
description: "Chính sách bảo mật của NextSmart POS: cách chúng tôi thu thập, sử dụng và bảo vệ dữ liệu cá nhân của người dùng theo Nghị định 13/2023/NĐ-CP."
keywords: ["chính sách bảo mật", "privacy policy", "NextSmart POS", "bảo vệ dữ liệu cá nhân", "QLBH"]
slug: chinh-sach/bao-mat-pos
canonical: "https://nextsmart.vn/chinh-sach/bao-mat-pos"
ogTitle: "Chính sách Bảo mật — NextSmart POS"
ogDescription: "Tìm hiểu cách NextSmart POS thu thập, sử dụng và bảo vệ dữ liệu cá nhân theo Nghị định 13/2023/NĐ-CP và yêu cầu Google Play / App Store."
datePublished: "2026-05-12"
dateModified: "2026-05-12"
---

**Áp dụng từ:** 12/05/2026  
**Phiên bản:** 1.0  
**Nhà phát triển:** Công ty TNHH NextSmart Vietnam  
**Email liên hệ:** support@nextsmart.vn

---

## 1. Giới thiệu

NextSmart POS (gọi tắt là **"Ứng dụng"** hoặc **"Dịch vụ"**) là phần mềm quản lý bán hàng đa nền tảng (web + mobile) phục vụ cho cửa hàng bán lẻ, F&B, nhà hàng, cafe tại Việt Nam. Khi sử dụng Ứng dụng, bạn đồng ý với các điều khoản thu thập, sử dụng và bảo vệ dữ liệu cá nhân được mô tả trong Chính sách này.

Chính sách này tuân thủ:
- **Nghị định 13/2023/NĐ-CP** về Bảo vệ dữ liệu cá nhân (Việt Nam)
- **Google Play Data Safety** requirements
- **Apple App Store Privacy Nutrition Label** (cho phiên bản iOS)

---

## 2. Dữ liệu cá nhân chúng tôi thu thập

### 2.1. Thông tin tài khoản (bắt buộc)

- **Tên đăng nhập** (email hoặc số điện thoại)
- **Mật khẩu** (mã hoá one-way bcrypt, không lưu plain-text)
- **Họ tên nhân viên**
- **Số điện thoại liên hệ**
- **Vai trò / cấp độ** trong doanh nghiệp

**Mục đích**: xác thực đăng nhập, phân quyền truy cập, liên hệ hỗ trợ.

### 2.2. Vị trí địa lý (Location)

- **Mục đích**: Chấm công GPS — xác minh nhân viên có mặt tại địa điểm cửa hàng khi check-in/check-out ca làm việc.
- **Khi thu thập**: Chỉ khi nhân viên chủ động bấm nút "Chấm công vào / ra".
- **Độ chính xác**: Tọa độ kinh độ/vĩ độ (precise location).
- **Background access**: KHÔNG. Ứng dụng KHÔNG theo dõi vị trí khi đang chạy nền.
- **Lưu trữ**: Tọa độ check-in được lưu cùng với timestamp ca làm việc trong cơ sở dữ liệu nội bộ, không chia sẻ với bên thứ 3.

### 2.3. Camera

- **Mục đích sử dụng**:
  - Quét mã vạch/barcode sản phẩm khi bán hàng (POS)
  - Quét QR code menu để đặt món tại bàn (khách hàng)
  - Chụp ảnh sản phẩm khi thêm/sửa hàng hoá (admin)
- **Khi thu thập**: Chỉ khi user chủ động mở chức năng quét hoặc chụp.
- **Lưu trữ ảnh sản phẩm**: Lưu trong máy chủ NextSmart (Vietnam datacenter) gắn với cửa hàng. KHÔNG truy cập gallery toàn bộ thiết bị.
- **Background access**: KHÔNG.

### 2.4. Danh bạ (Contacts)

- **Mục đích**: Cho phép nhân viên/quản lý thêm khách hàng mới nhanh từ danh bạ điện thoại (không bắt buộc — user có thể nhập tay).
- **Khi thu thập**: Chỉ khi user chủ động bấm "Chọn từ danh bạ" trong form thêm khách hàng.
- **Lưu trữ**: Chỉ tên + số điện thoại của contact được chọn được lưu vào CSDL khách hàng của cửa hàng. KHÔNG đọc toàn bộ danh bạ, KHÔNG upload danh bạ lên server.

### 2.5. Dữ liệu nghiệp vụ (do user nhập)

- **Khách hàng cuối**: tên, số điện thoại, email (nếu user nhập), điểm tích luỹ, lịch sử mua hàng.
- **Hoá đơn**: thông tin giao dịch bán hàng, sản phẩm, giá, hình thức thanh toán.
- **Nhân viên**: thông tin nhân sự, lương, ca làm việc, chấm công.
- **Sản phẩm**: tên, giá, ảnh, mô tả, tồn kho.

### 2.6. Dữ liệu thiết bị (technical)

- **Loại thiết bị**: model, hệ điều hành, phiên bản OS
- **Định danh thiết bị**: device ID (chỉ dùng cho fingerprint chống fraud, không liên kết quảng cáo)
- **Địa chỉ IP**: lưu trong audit log mục đích bảo mật
- **Logs**: lỗi crash, log truy cập (giữ 30 ngày)

---

## 3. Cách chúng tôi sử dụng dữ liệu

| Mục đích | Loại dữ liệu | Cơ sở pháp lý |
|---|---|---|
| Vận hành ứng dụng POS | Tài khoản, nghiệp vụ | Hợp đồng dịch vụ |
| Chấm công nhân viên | Location, tài khoản | Quan hệ lao động + đồng ý của NV |
| Quét barcode/QR | Camera | Đồng ý của user |
| Quản lý khách hàng / tích điểm | Khách hàng (do cửa hàng nhập) | Cửa hàng phải có đồng ý từ khách của họ |
| Bảo mật, audit, chống gian lận | Logs, IP, device ID | Lợi ích chính đáng |
| Hỗ trợ khách hàng | Email/SĐT liên hệ | Hợp đồng |
| Cải thiện sản phẩm | Logs ẩn danh, crash report | Lợi ích chính đáng |

**Chúng tôi KHÔNG**:
- Bán dữ liệu cá nhân cho bên thứ 3
- Sử dụng dữ liệu cho mục đích quảng cáo có chủ đích
- Thu thập location khi không cần (chỉ tại moment chấm công)
- Truy cập danh bạ khi không có user action

---

## 4. Chia sẻ dữ liệu với bên thứ 3

NextSmart POS có thể chia sẻ dữ liệu với các bên sau, **CHỈ trong phạm vi cần thiết để cung cấp dịch vụ**:

| Bên thứ 3 | Mục đích | Loại dữ liệu chia sẻ |
|---|---|---|
| **VNPay, MoMo, ZaloPay, SePay** | Xử lý thanh toán điện tử | Số tiền giao dịch, mã đơn — KHÔNG chia sẻ thông tin khách hàng |
| **Shopee Food, Grab Food** | Đồng bộ đơn hàng giao đi | Thông tin đơn (món, địa chỉ giao do app đối tác nắm) |
| **Resend** | Gửi email thông báo (kích hoạt tài khoản, hoá đơn điện tử) | Email người nhận, tên |
| **Google Play / App Store** | Phân phối ứng dụng | Crash report, basic device info |
| **Sentry** | Ghi nhận lỗi runtime (chống bug) | Stack trace, device info (ẩn danh hoá user) |
| **Cloudflare** | CDN, DDoS protection | IP, request metadata |

Tất cả các bên thứ 3 trên đều có cam kết bảo mật riêng. Người dùng có quyền yêu cầu danh sách đối tác cụ thể đang xử lý dữ liệu của mình.

---

## 5. Lưu trữ và bảo mật dữ liệu

### 5.1. Vị trí lưu trữ

- **Máy chủ chính**: Việt Nam (Datacenter tại Hà Nội hoặc TP.HCM)
- **Backup**: Encrypted, stored in cùng datacenter
- **Một số dịch vụ phụ trợ** (Sentry, Cloudflare) có thể có node toàn cầu

### 5.2. Biện pháp bảo mật

- Mã hoá HTTPS/TLS 1.2+ cho mọi traffic
- Mật khẩu bcrypt one-way hash (không thể decrypt)
- Token JWT với httpOnly cookie + signed (chống XSS)
- Multi-tenant isolation cấp database (Row-Level Security)
- Audit log mọi thao tác nhạy cảm (đăng nhập, thay đổi quyền, xoá data)
- Backup tự động hàng ngày, retention 30 ngày
- 2FA (xác thực 2 yếu tố) cho tài khoản quản trị

### 5.3. Thời gian lưu trữ

| Loại dữ liệu | Thời gian lưu |
|---|---|
| Dữ liệu tài khoản | Suốt thời gian hợp đồng + 90 ngày sau khi huỷ |
| Lịch sử giao dịch | Tối thiểu 5 năm (yêu cầu kế toán/thuế) |
| Logs bảo mật | 90 ngày |
| Crash report | 30 ngày |
| Backup | 30 ngày |
| Dữ liệu khách hàng cuối | Theo policy của cửa hàng — chúng tôi cung cấp công cụ xoá theo yêu cầu |

---

## 6. Quyền của người dùng

Theo **Nghị định 13/2023/NĐ-CP**, bạn có các quyền sau:

1. **Quyền được biết** — yêu cầu thông tin về dữ liệu chúng tôi đang lưu trữ về bạn
2. **Quyền truy cập** — xem dữ liệu cá nhân của mình
3. **Quyền sửa đổi** — yêu cầu chỉnh sửa thông tin sai
4. **Quyền xoá** — yêu cầu xoá dữ liệu (trừ dữ liệu bắt buộc lưu theo luật)
5. **Quyền hạn chế xử lý** — yêu cầu tạm dừng sử dụng dữ liệu cho mục đích cụ thể
6. **Quyền portability** — yêu cầu xuất dữ liệu của mình dưới format đọc được (JSON/CSV)
7. **Quyền phản đối** — phản đối việc xử lý dữ liệu cho mục đích marketing
8. **Quyền khiếu nại** — gửi khiếu nại đến cơ quan chức năng (Bộ Thông tin & Truyền thông)

**Cách thực hiện**: Gửi email tới `support@nextsmart.vn` với tiêu đề **"Yêu cầu quyền dữ liệu"**. Chúng tôi phản hồi trong **30 ngày**.

---

## 7. Cookie và công nghệ tương tự

Ứng dụng web sử dụng:

| Loại cookie | Mục đích | Có thể tắt? |
|---|---|---|
| Cookie cần thiết (httpOnly, signed) | Lưu phiên đăng nhập | Không |
| Cookie CSRF | Chống tấn công cross-site | Không |
| localStorage | Lưu cấu hình hiển thị (theme, ngôn ngữ) | Có |

**KHÔNG sử dụng**: cookie tracking, third-party advertising cookie.

---

## 8. Trẻ em

Ứng dụng KHÔNG dành cho người dưới 18 tuổi. Chúng tôi không cố ý thu thập dữ liệu từ trẻ em. Nếu phát hiện, dữ liệu sẽ bị xoá ngay khi được thông báo.

---

## 9. Thay đổi chính sách

Chúng tôi có thể cập nhật Chính sách này theo thời gian. Phiên bản mới sẽ được công bố tại `https://nextsmart.vn/chinh-sach/bao-mat-pos` với thông báo trên ứng dụng **ít nhất 7 ngày** trước khi có hiệu lực. Việc tiếp tục sử dụng Ứng dụng sau ngày hiệu lực được coi là đồng ý với phiên bản mới.

---

## 10. Liên hệ

**Câu hỏi, khiếu nại, yêu cầu quyền dữ liệu:**

- **Email**: support@nextsmart.vn
- **Điện thoại**: *(sẽ cập nhật)*
- **Địa chỉ**: *(sẽ cập nhật)*
- **Website**: https://nextsmart.vn

**Cơ quan giám sát**: Cục An toàn thông tin — Bộ Thông tin và Truyền thông (https://ais.gov.vn)

---

*Tài liệu này có hiệu lực từ 12/05/2026. Phiên bản: 1.0.*
