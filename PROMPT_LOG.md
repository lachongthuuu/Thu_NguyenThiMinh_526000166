# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)
- **Họ và tên:** Nguyễn Thị Minh Thu
- **MSSV:** 526000166
- **Tên đề tài Website:** Landing Page Phim Kinh Dị: Phí Phông - Quỷ Máu Rừng Thiêng
- **Công cụ AI đã sử dụng:** Antigravity (Gemini 3.1 Pro)

## 1. Yêu cầu ban đầu (System/Initial Prompt)
> *Ghi lại prompt tổng quan ban đầu bạn dùng để khởi tạo khung website.*
"Bạn là một AI Coding Agent hoạt động trong môi trường Antigravity. Hãy tự động tạo toàn bộ cấu trúc file và viết mã nguồn cho dự án Landing Page giới thiệu bộ phim kinh dị Việt Nam: 'Phí Phông: Quỷ Máu Rừng Thiêng'. Dự án phải đáp ứng 100% các tiêu chuẩn kỹ thuật và khung chấm điểm của bài kiểm tra giữa kỳ Thiết kế Web: chuẩn Semantic HTML5, CSS Variables, Flexbox/Grid, hiệu ứng Animate.css và AOS."

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)
### Lần 1: Dựng khung Semantic HTML & CSS Variable
- **Prompt đã dùng:** Yêu cầu AI viết file `index.html` sử dụng đúng các thẻ `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` và file `style.css` với `:root` cho màu đỏ máu, đen, font Creepster.
- **Kết quả AI tạo ra:** AI đã tạo khung chuẩn HTML5 và khai báo biến CSS chính xác, không dùng thẻ `<div>` vô nghĩa.
- **Nhận xét & Tinh chỉnh của SV:** AI đã phân chia tốt các khối chức năng. Cấu trúc rõ ràng, sử dụng biến CSS giúp tôi dễ dàng thay đổi tông màu chung của web.

### Lần 2: Tích hợp thư viện Animate.css & AOS
- **Prompt đã dùng:** "Nhúng Google Fonts, Animate.css và AOS qua CDN. Thêm các class hiệu ứng vào phần Hero, Tiêu đề, và kích hoạt AOS.init() cho các section khi cuộn chuột."
- **Thách thức gặp phải:** AOS đôi khi không chạy mượt do các class CSS hoặc thiếu kịch bản khởi tạo.
- **Cách sửa prompt (Debug prompt):** "Đảm bảo AOS được khởi tạo `AOS.init()` ở cuối thẻ `<body>` và thêm các thuộc tính `data-aos`, `data-aos-delay` vào các thẻ `<section>`, `<article>` trong Grid nhân vật."

## 3. Đánh giá cá nhân về quá trình Vibe Coding
- **AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?**
  AI giúp tiết kiệm rất nhiều thời gian trong việc gõ các đoạn code boilerplate (khung cơ bản HTML), thiết lập CSS grid/flexbox và tìm kiếm/nhúng chính xác các link CDN của thư viện.
- **Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?**
  Cần phải cụ thể về yêu cầu (ví dụ: chỉ rõ phải dùng thẻ semantic nào, thư viện tên gì), và chia nhỏ quá trình để dễ kiểm soát mã nguồn thay vì yêu cầu tạo toàn bộ mọi thứ một cách chung chung.
