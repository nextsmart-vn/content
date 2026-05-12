---
title: "Bảo mật — NextSmart POS (QLBH)"
description: "Chính sách bảo mật NextSmart POS: cách thu thập, sử dụng và bảo vệ dữ liệu cá nhân theo Nghị định 13/2023/NĐ-CP, Google Play Data Safety và Apple App Store."
keywords: ["chính sách bảo mật", "NextSmart POS", "QLBH", "Google Play", "bảo vệ dữ liệu"]
slug: bao-mat-pos
canonical: "https://nextsmart.vn/chinh-sach/bao-mat-pos"
ogTitle: "Chính sách Bảo mật — NextSmart POS"
ogDescription: "Cách NextSmart POS thu thập dữ liệu location, camera, contacts và tuân thủ NĐ 13/2023/NĐ-CP, Google Play Data Safety."
dateModified: "2026-05-12"
---

**Áp dụng từ:** 12/05/2026 · **Phiên bản:** 1.0
**Nhà phát triển:** Công ty TNHH NextSmart Vietnam

NextSmart POS là phần mềm quản lý bán hàng đa nền tảng (web + mobile) phục vụ cho cửa hàng bán lẻ, F&B, nhà hàng, cafe tại Việt Nam. Khi sử dụng Ứng dụng, bạn đồng ý với các điều khoản thu thập, sử dụng và bảo vệ dữ liệu cá nhân được mô tả trong Chính sách này.

Chính sách này tuân thủ **Nghị định 13/2023/NĐ-CP**, **Google Play Data Safety** và **Apple App Store Privacy Nutrition Label**.

---

## 2. Dữ liệu cá nhân chúng tôi thu thập

### 2.1. Thông tin tài khoản (bắt buộc)

- Tên đăng nhập (email hoặc số điện thoại)
- Mật khẩu (mã hoá one-way bcrypt, không lưu plain-text)
- Họ tên nhân viên, số điện thoại liên hệ, vai trò trong doanh nghiệp

### 2.2. Vị trí địa lý (Location)

- **Mục đích:** Chấm công GPS — xác minh nhân viên có mặt tại địa điểm cửa hàng khi check-in/check-out.
- **Khi thu thập:** Chỉ khi nhân viên chủ động bấm nút "Chấm công vào / ra".
- **Background access:** KHÔNG. Ứng dụng KHÔNG theo dõi vị trí khi đang chạy nền.

### 2.3. Camera

- Quét mã vạch/barcode sản phẩm khi bán hàng (POS)
- Quét QR code menu để đặt món tại bàn
- Chụp ảnh sản phẩm khi thêm/sửa hàng hoá (admin)
- Chỉ kích hoạt khi user chủ động mở chức năng. KHÔNG truy cập gallery toàn bộ thiết bị.

### 2.4. Danh bạ (Contacts)

Chỉ khi user bấm "Chọn từ danh bạ" — chỉ tên + số điện thoại của contact được chọn lưu vào CSDL khách hàng. KHÔNG đọc toàn bộ danh bạ, KHÔNG upload lên server.

### 2.5. Dữ liệu nghiệp vụ

- Khách hàng cuối: tên, số điện thoại, email, điểm tích luỹ, lịch sử mua hàng
- Hoá đơn: thông tin giao dịch, sản phẩm, giá, hình thức thanh toán
- Nhân viên: thông tin nhân sự, lương, ca làm việc, chấm công
- Sản phẩm: tên, giá, ảnh, mô tả, tồn kho

---

## 3. Cách chúng tôi sử dụng dữ liệu

**Chúng tôi KHÔNG:** bán dữ liệu cá nhân cho bên thứ 3, sử dụng cho mục đích quảng cáo có chủ đích, thu thập location khi không có user action, truy cập danh bạ khi không có user action.

## 4. Chia sẻ dữ liệu với bên thứ 3

Chỉ trong phạm vi cần thiết để cung cấp dịch vụ: VNPay/MoMo/ZaloPay (xử lý thanh toán), Shopee Food/Grab Food (đồng bộ đơn), Resend (email thông báo), Sentry (crash report ẩn danh), Cloudflare (CDN/DDoS).

## 5. Bảo mật dữ liệu

- Mã hoá HTTPS/TLS 1.2+, mật khẩu bcrypt one-way hash
- JWT httpOnly cookie + signed (chống XSS)
- Multi-tenant isolation cấp database (Row-Level Security)
- 2FA cho tài khoản quản trị, backup tự động 30 ngày

## 6. Quyền của người dùng

Theo **Nghị định 13/2023/NĐ-CP**: quyền được biết, truy cập, sửa đổi, xoá, hạn chế xử lý, portability, phản đối và khiếu nại.

Gửi email tới **support@nextsmart.vn** với tiêu đề "Yêu cầu quyền dữ liệu". Phản hồi trong 30 ngày.

## 7. Trẻ em

Ứng dụng KHÔNG dành cho người dưới 18 tuổi. Dữ liệu trẻ em sẽ bị xoá ngay khi được thông báo.

## 8. Thay đổi chính sách

Phiên bản mới sẽ được thông báo trong ứng dụng ít nhất **7 ngày** trước khi có hiệu lực.

---

Liên hệ: **support@nextsmart.vn** | Cơ quan giám sát: [Cục An toàn thông tin](https://ais.gov.vn)
