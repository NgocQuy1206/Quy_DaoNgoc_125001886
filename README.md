# Legends FC — Website giới thiệu câu lạc bộ bóng đá

Website tĩnh giới thiệu câu lạc bộ bóng đá **Legends FC**, viết bằng **HTML5 và CSS3, không sử dụng JavaScript**. Giao diện responsive, logo SVG tự thiết kế, ảnh các ngôi sao bóng đá, các khu vực giới thiệu CLB, đội hình biểu tượng, huyền thoại, lịch thi đấu mẫu, học viện và lời kêu gọi hành động.

## Cấu trúc

- `index.html` — nội dung với các thẻ semantic HTML5
- `style.css` — CSS Variables, Flexbox/Grid, responsive, hover/focus, Animate.css classes và hiệu ứng cuộn CSS-only
- `assets/legends-logo.svg` — logo vector của Legends FC
- `PROMPT_LOG.md` — nhật ký Prompt Engineering, cần cá nhân hóa trước khi nộp

## Điểm quan trọng về yêu cầu đề thi

Đề thi gốc yêu cầu tích hợp **AOS (Animate On Scroll)**. AOS cần JavaScript để phát hiện vị trí cuộn và thêm trạng thái animation. Vì yêu cầu của bạn là **không dùng JavaScript**, phiên bản này không nạp AOS và thay bằng hiệu ứng cuộn thuần CSS (`animation-timeline: view()`) trên trình duyệt hỗ trợ; trình duyệt không hỗ trợ vẫn hiển thị đầy đủ nội dung. Do đó, website tuân thủ ràng buộc không JavaScript nhưng **không thể đồng thời đạt đúng 100% tiêu chí AOS của đề** nếu không cho phép JavaScript. Animate.css vẫn được dùng vì phần hiệu ứng của thư viện này là CSS.

## Chạy thử

Mở `index.html` bằng trình duyệt. Font chữ, Animate.css và ảnh cầu thủ tải từ Internet; logo SVG và nội dung chính nằm trong gói. Không có file JavaScript hoặc thẻ `<script>`.

## Đưa lên GitHub Pages

1. Tạo repository công khai với tên đúng cú pháp giảng viên yêu cầu: `Ten_Ho_MSSV`.
2. Giải nén ZIP, mở thư mục `Legends_FC_Website`, tải **toàn bộ nội dung bên trong** lên repository (không chỉ tải ZIP).
3. Commit các file lên branch `main`.
4. Vào **Settings → Pages**.
5. Chọn **Deploy from a branch**, branch `main`, folder `/(root)`, nhấn **Save**.
6. Chờ GitHub tạo link Pages, mở link để kiểm tra; gửi cả link repository và link Pages theo hướng dẫn nộp bài.

## Trước khi nộp

- Điền họ tên và MSSV trong `PROMPT_LOG.md`.
- Chỉnh nội dung mẫu về lịch đấu/đối thủ theo ý tưởng thực tế của bạn.
- Ảnh huyền thoại lấy qua Wikimedia Commons; hãy kiểm tra trang nguồn và yêu cầu ghi công/giấy phép trước khi công khai.
- Biểu mẫu JavaScript-dependent đã được thay bằng các CTA HTML thuần để mọi thành phần hiển thị đều không cần JS.


## Phiên bản nhận diện xanh sư tử
- Huy hiệu SVG sư tử tự thiết kế, tông navy/cobalt/xanh băng.
- Bổ sung kho hồ sơ 16 cầu thủ nổi tiếng với vị trí, số áo biểu tượng, mô tả phong cách và liên kết ảnh Wikimedia Commons.
- Trang vẫn dùng HTML5 và CSS thuần; không cần JavaScript.


## Bản Blue Lion Premium
- Nâng cấp logo sư tử SVG, hiệu ứng ánh sáng xanh, header sticky có nền blur, hero tương phản cao, thẻ cầu thủ có hover, nền trang có họa tiết và hiệu ứng CSS-only.
- Website không sử dụng JavaScript; hiệu ứng xuất hiện khi cuộn dựa trên CSS Scroll-driven Animations trên trình duyệt hỗ trợ.
- Liên kết logo tham chiếu bạn gửi qua ChatGPT không thể tải trực tiếp từ môi trường xử lý. Logo trong bản này là logo sư tử SVG được thiết kế lại theo cùng chủ đề xanh; để dùng đúng tệp logo tham chiếu, cần tải ảnh logo về và đính kèm trực tiếp.
