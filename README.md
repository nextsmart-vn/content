# NextSmart — Content Repository

Đây là kho lưu trữ toàn bộ nội dung website [nextsmart.vn](https://nextsmart.vn). Mỗi file `.md` tương ứng với một trang trên website.

> **Cách chỉnh sửa:** Edit file markdown trực tiếp trên GitHub → website tự động cập nhật sau vài phút (qua webhook + rebuild).

---

## Cấu trúc thư mục

```
content/
├── blog/                          # Bài viết blog / SEO articles
│   ├── erp-xay-dung-la-gi.md         → /blog/erp-xay-dung-la-gi
│   ├── phan-mem-quan-ly-khach-san-pms.md → /blog/phan-mem-quan-ly-khach-san-pms
│   └── so-hoa-tai-lieu-ocr-ai.md     → /blog/so-hoa-tai-lieu-ocr-ai
│
├── san-pham/                      # Trang sản phẩm
│   ├── erp.md                        → /erp
│   ├── hotel.md                      → /hotel
│   ├── agent.md                      → /agent
│   ├── edoc.md                       → /edoc
│   ├── marketing.md                  → /marketing
│   └── qlbh.md                       → /qlbh
│
└── cong-ty/                       # Trang công ty
    ├── gioi-thieu.md                 → /gioi-thieu
    └── bang-gia.md                   → /bang-gia
```

---

## Cấu trúc frontmatter (phần đầu mỗi file)

```yaml
---
title: "Tiêu đề trang — hiển thị trên tab browser và Google"
description: "Mô tả SEO — 150-160 ký tự, xuất hiện trong kết quả tìm kiếm"
keywords: ["từ khoá 1", "từ khoá 2", "từ khoá 3"]
slug: ten-trang            # URL path
canonical: "https://nextsmart.vn/ten-trang"
ogTitle: "Tiêu đề khi share lên Facebook/Zalo"
ogDescription: "Mô tả khi share lên mạng xã hội"
# Chỉ cho blog:
category: "Tên danh mục"
readTime: "X phút đọc"
datePublished: "2025-04-15"
dateModified: "2025-04-15"
ctaText: "Text nút CTA"
ctaLink: "/duong-dan"
ctaColor: "blue | emerald | sky"
---
```

---

## Hướng dẫn chỉnh sửa

### Chỉnh sửa nội dung đơn giản
1. Mở file `.md` tương ứng trên GitHub
2. Nhấn nút **✏️ Edit** (bút chì) góc phải
3. Chỉnh sửa nội dung
4. Nhấn **Commit changes**
5. Website tự cập nhật sau ~2-3 phút

### Thêm bài blog mới
1. Tạo file mới trong `content/blog/`
2. Đặt tên file theo slug URL: `ten-bai-viet.md`
3. Copy frontmatter từ file bài viết có sẵn
4. Điền đầy đủ nội dung
5. Commit → website tự tạo trang mới

### Quy tắc viết Markdown
- `## Tiêu đề lớn` — dùng cho các section chính
- `### Tiêu đề nhỏ` — dùng cho sub-section
- `**Chữ đậm**` — highlight từ khoá quan trọng
- `- Dấu gạch đầu dòng` — danh sách không thứ tự
- `| Cột 1 | Cột 2 |` — bảng so sánh
- `✓ ✅ ⚠️ ❌` — icon trạng thái

---

## Liên hệ kỹ thuật

Có vấn đề kỹ thuật hoặc cần thêm tính năng: liên hệ team dev qua GitHub Issues.
