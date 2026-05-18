---
title: "LIS — Phần mềm Quản lý Hệ thống Xét nghiệm"
description: "LIS NextTech: phần mềm quản lý xét nghiệm (Laboratory Information System) tích hợp máy xét nghiệm tự động, kiểm soát chất lượng QC/QA, kết nối HIS/PACS, trả kết quả điện tử. Chuẩn ISO 15189."
keywords: ["phần mềm quản lý xét nghiệm LIS", "Laboratory Information System", "kết nối máy xét nghiệm tự động", "kiểm soát chất lượng xét nghiệm QC", "LIS bệnh viện Việt Nam", "ISO 15189", "LIS NextTech"]
slug: lis
canonical: "https://nextsmart.vn/lis"
menuEmoji: "🧪"
menuName: "LIS Xét nghiệm"
menuDesc: "Quản lý hệ thống xét nghiệm, kết nối máy tự động, ISO 15189"
menuHref: "/lis"
ogTitle: "LIS — Quản lý Xét nghiệm, Kết nối Máy Tự động, QC/QA chuẩn ISO 15189"
ogDescription: "Kết nối máy xét nghiệm tự động (ASTM/HL7), kiểm soát chất lượng Westgard, trả kết quả realtime, ký số bác sĩ, kết nối HIS đa chiều."
---

## LIS là gì?

LIS (Laboratory Information System) NextTech là phần mềm quản lý toàn diện hoạt động của khoa xét nghiệm tại bệnh viện, phòng xét nghiệm độc lập và trung tâm y tế dự phòng. Hệ thống kết nối tự động với máy phân tích, kiểm soát chất lượng theo chuẩn ISO 15189 và trả kết quả điện tử về HIS theo thời gian thực.

## Tính năng theo module

### Tiếp nhận & Quản lý mẫu
- Nhận y lệnh từ HIS hoặc nhập tay — in nhãn barcode tự động
- Quét barcode nhận mẫu tại quầy lấy mẫu — không nhầm lẫn
- Theo dõi hành trình mẫu: lấy mẫu → vận chuyển → nhận tại lab → phân tích → trả kết quả
- Quản lý ống mẫu, điều kiện bảo quản, thời gian ổn định
- Cảnh báo mẫu không đạt: tan huyết, đục, thiếu thể tích

### Kết nối máy xét nghiệm tự động
- Giao thức ASTM E1394 và HL7 — kết nối 200+ loại máy phổ biến: Beckman, Roche, Sysmex, Abbott, Mindray
- Tự động nhận kết quả từ máy — không nhập tay
- Kiểm tra delta check: so sánh kết quả lần này vs lần trước cùng bệnh nhân
- Auto-reflex: tự động chỉ định thêm xét nghiệm khi kết quả vượt ngưỡng
- Quản lý calibration, bảo trì máy, vật tư tiêu hao

### Kiểm soát chất lượng QC/QA
- Chạy QC nội bộ (IQC) theo quy tắc Westgard 1-2s, 1-3s, 2-2s, R-4s, 4-1s, 10x
- Biểu đồ Levey-Jennings realtime — phát hiện sai lệch hệ thống
- Tham gia EQAS (External Quality Assessment Scheme) — quản lý hồ sơ PT
- Quản lý tài liệu: SOP, biểu mẫu QC, hồ sơ kiểm chuẩn theo ISO 15189
- Báo cáo QC định kỳ theo yêu cầu kiểm định phòng xét nghiệm

### Phê duyệt & Trả kết quả
- Bác sĩ/KTV phê duyệt kết quả trước khi trả — ký số điện tử
- Tô màu kết quả bất thường: thấp/cao/nguy kịch theo ngưỡng theo lứa tuổi, giới tính
- Trả kết quả về HIS realtime — bác sĩ lâm sàng xem ngay trên EMR
- Gửi kết quả cho bệnh nhân qua SMS/Zalo/email tự động
- In phiếu kết quả: mẫu chuẩn có logo, ký số bác sĩ, mã QR xác thực

### Kho hoá chất & Vật tư
- Quản lý nhập/tồn/xuất hoá chất, thuốc thử theo số lô, hạn dùng
- Tính chi phí xét nghiệm theo hoá chất tiêu hao thực tế
- Cảnh báo sắp hết hoá chất — đề xuất đặt hàng tự động
- Báo cáo tiêu hao vật tư theo máy, theo xét nghiệm

### Báo cáo & Thống kê
- Tần suất xét nghiệm theo loại, theo khoa gửi, theo bác sĩ chỉ định
- Thời gian TAT (Turnaround Time) từng bước — phát hiện điểm tắc nghẽn
- Tỷ lệ mẫu từ chối, lý do từ chối — cải thiện chất lượng trước phân tích
- Báo cáo doanh thu xét nghiệm, kê khai BHYT
- Xuất số liệu giám sát dịch tễ gửi CDC theo định kỳ

## Chuẩn kỹ thuật & Tích hợp

| Tiêu chí | Thông số |
|---|---|
| Giao thức kết nối máy | ASTM E1394, HL7 v2.x, LIS-Host Interface |
| Tích hợp HIS/EMR | HL7 v2.x / FHIR R4 — 2 chiều |
| Chuẩn chất lượng | ISO 15189:2022, TCVN ISO 15189 |
| Bảo mật | RBAC 4 cấp, audit log, TLS 1.3 |
| Hỗ trợ máy | 200+ model: Beckman, Roche, Sysmex, Abbott, Mindray, Horiba |
| Nền tảng | Cloud hoặc On-premise, hỗ trợ cụm nhiều lab |

## Phù hợp với mô hình nào?

| Mô hình | Phù hợp |
|---|---|
| Bệnh viện đa khoa có khoa xét nghiệm | ✅ Rất phù hợp (kết nối máy tự động, QC, kết nối HIS) |
| Phòng xét nghiệm độc lập (lab tư nhân) | ✅ Rất phù hợp (quản lý mẫu, trả kết quả, thu phí) |
| Trung tâm Y tế dự phòng / CDC | ✅ Phù hợp (giám sát dịch tễ, QC chuẩn, báo cáo Sở Y tế) |
| Phòng khám có xét nghiệm mini lab | ✅ Phù hợp (LIS đơn giản, kết nối 1–5 máy, trả kết quả Zalo) |
| Chuỗi phòng xét nghiệm đa điểm | ✅ Phù hợp (LIS tập trung, nhận mẫu vệ tinh, phân tích trung tâm) |
