# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)

- **Họ và tên:** Đào Ngọc Quý
- **MSSV:** 125001886
- **Tên đề tài Website:** Website giới thiệu câu lạc bộ bóng đá Legends FC
- **Công cụ AI đã sử dụng:** ChatGPT

> Đây là bản nháp hỗ trợ ghi lại quá trình. Trước khi nộp, hãy sửa cho khớp với quá trình làm bài thực tế của bạn.

## 1. Yêu cầu ban đầu (Initial Prompt)

> Tạo website giới thiệu câu lạc bộ bóng đá mang tên Legends FC bằng HTML5 và CSS3, không sử dụng JavaScript. Dùng semantic HTML5 gồm `header`, `nav`, `main`, `section`, `article`, `footer`; tạo bảng màu nhất quán bằng CSS Variables trong `:root`; dùng Flexbox/Grid; giao diện responsive, có hiệu ứng `:hover` và `:focus`; có logo SVG phong cách nghệ thuật và hình ảnh ngôi sao/huyền thoại bóng đá. Chia mã thành `index.html`, `style.css`, `assets/` và `PROMPT_LOG.md`.

## 2. Quá trình tinh chỉnh và giải quyết sự cố

### Lần 1: Dựng cấu trúc semantic và CSS Variables

- **Prompt đã dùng:** “Tạo khung website Legends FC bằng semantic HTML5; sử dụng `header`, `nav`, `main`, `section`, `article`, `footer`; quản lý màu sắc/font/khoảng cách bằng CSS Variables; bố cục bằng CSS Grid và Flexbox.”
- **Kết quả:** Có các phần Hero, bản sắc CLB, đội hình, huyền thoại, lịch đấu, học viện, CTA và footer.
- **Tinh chỉnh:** Đổi thương hiệu sang Legends FC; sử dụng logo SVG riêng và màu xanh đen, xanh chanh, kem.

### Lần 2: Ràng buộc không dùng JavaScript

- **Prompt đã dùng:** “Loại bỏ toàn bộ JavaScript, không dùng thẻ `<script>` và không để nút giao diện nào phụ thuộc vào JavaScript. Menu mobile phải dùng tính năng HTML/CSS thuần; bỏ form demo không thể gửi dữ liệu và thay bằng liên kết điều hướng hoạt động thật.”
- **Kết quả:** Menu điện thoại sử dụng `<details>`/`<summary>`; CTA dùng liên kết HTML; không còn `script.js` hoặc thẻ `<script>`.
- **Thách thức kỹ thuật:** Đề thi yêu cầu AOS (Animate On Scroll), nhưng AOS cần JavaScript để phát hiện cuộn và kích hoạt trạng thái hiệu ứng. Yêu cầu “không dùng JavaScript” mâu thuẫn trực tiếp với việc tích hợp AOS đúng chức năng.
- **Cách xử lý:** Giữ Animate.css (thư viện CSS) và dùng hiệu ứng cuộn CSS thuần dựa trên `animation-timeline: view()` cho trình duyệt hỗ trợ. Nếu trình duyệt không hỗ trợ, nội dung vẫn hiển thị bình thường. Đây là giải pháp thay thế, không phải AOS thật.

### Lần 3: Responsive và khả năng tiếp cận

- **Prompt đã dùng:** “Kiểm tra giao diện ở desktop/mobile; thêm trạng thái hover/focus rõ ràng; hỗ trợ `prefers-reduced-motion`; bảo đảm ảnh có alt text và liên kết mở nguồn ảnh.”
- **Kết quả:** Có lưới responsive, trạng thái focus, tùy chọn giảm chuyển động và các liên kết nguồn ảnh.
- **Việc cần tự kiểm tra:** Mở trang trên trình duyệt desktop và điện thoại; kiểm tra điều hướng, ảnh, tương phản và liên kết; cập nhật nội dung mẫu trước khi nộp.

## 3. Đánh giá cá nhân về quá trình Vibe Coding

- **AI đã giúp tiết kiệm thời gian ở đâu?** Dựng cấu trúc trang, thiết kế logo SVG, xây dựng bảng màu, tạo lưới responsive và đề xuất hiệu ứng CSS.
- **Bài học khi viết prompt:** Nêu rõ công nghệ được phép và bị cấm, cấu trúc file, ngữ nghĩa HTML, phong cách giao diện và cách kiểm thử. Cần đọc mã nguồn và kiểm tra đầu ra thay vì tin rằng AI đã đáp ứng mọi yêu cầu.
- **Bài học về mâu thuẫn yêu cầu:** Cần nhận diện khi hai tiêu chí không thể đồng thời thỏa mãn. Bản này ưu tiên ràng buộc không JavaScript; vì vậy hiệu ứng CSS thay thế không thể được xem là tích hợp AOS đúng theo nguyên văn đề.

## 4. Checklist trước khi nộp

- [ ] Điền họ tên và MSSV.
- [ ] Tạo repository tên `Ten_Ho_MSSV`.
- [ ] Đưa `index.html`, `style.css`, `assets/` và `PROMPT_LOG.md` lên repository.
- [ ] Bật GitHub Pages trong Settings → Pages.
- [ ] Kiểm tra đường link live preview trên máy tính và điện thoại.
- [ ] Kiểm tra giấy phép/ghi công ảnh trước khi công khai.
- [ ] Lưu ý: phiên bản không JavaScript **không đáp ứng mục AOS của đề theo nghĩa chặt**; muốn đạt đủ tiêu chí này phải cho phép JavaScript hoặc hỏi giảng viên chấp nhận giải pháp CSS thay thế.


## Iteration 3 — Blue Lion identity & player archive
**Prompt:** Đổi nhận diện Legends FC sang xanh navy/xanh cobalt với logo sư tử cách điệu; mở rộng hồ sơ cầu thủ, ảnh, vị trí và mô tả phong cách. Giữ HTML/CSS thuần, responsive và không dùng JavaScript.
**Kết quả:** Tạo huy hiệu SVG sư tử riêng; cập nhật biến màu CSS; bổ sung 16 hồ sơ ngôi sao/huyền thoại ngoài bốn biểu tượng ban đầu. Ảnh ngoài được liên kết từ Wikimedia Commons và có liên kết mở nguồn.
**Lưu ý kiểm thử:** URL ảnh Wikimedia có thể thay đổi theo tên tệp và mạng; nếu một ảnh không hiện, thẻ có liên kết để mở kết quả ảnh trên Commons.
