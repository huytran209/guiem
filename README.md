# Our 6 Months Together — Huy Tran & Thuỳ Linh (v1.3)

Website kỷ niệm 6 tháng yêu nhau, dùng HTML/CSS/JavaScript thuần, có thể triển khai miễn phí trên GitHub Pages.

## Cấu trúc
- `index.html` — trang chính
- `style.css` — giao diện responsive, scrapbook vintage
- `script.js` — mở nhật ký, bộ đếm, trình phát nhạc và lời nhắn
- `assets/images/huy-tran.jpeg` — ảnh Huy (bên trái)
- `assets/images/thuy-linh.jpeg` — ảnh Thuỳ Linh (bên phải)
- `assets/music/our-song.mp3` — bản MP3 ưu tiên phát nhạc
- `assets/music/our-song.m4a` — bản M4A dự phòng

## Những thay đổi ở v1.3
- Đổi font sang Playfair Display, Dancing Script và Be Vietnam Pro.
- Đưa hai ảnh lên bìa nhật ký để chúng hiển thị ngay từ màn hình đầu tiên; giữ ảnh trong phần giới thiệu bên trong nhật ký.
- Chuyển bài nhạc M4A gốc sang MP3 và đặt MP3 làm nguồn phát ưu tiên; giữ M4A làm nguồn dự phòng.
- Cải thiện thông báo khi trình duyệt không tải/phát được nhạc.
- Giữ nguyên nội dung thư, sáu lời nhắn, ngày bắt đầu 30/04/2026 và lời kết đã duyệt.
- Không có mục “Little Moments”.

## Chạy thử
Nên mở qua máy chủ tĩnh cục bộ để kiểm tra đường dẫn tài nguyên, ví dụ chạy `python -m http.server 8000` trong thư mục dự án rồi truy cập `http://localhost:8000`. Khi nghe nhạc, hãy bấm nút phát vì trình duyệt có thể chặn tự động phát.

## Đăng lên GitHub Pages
1. Tải **toàn bộ nội dung bên trong thư mục dự án** lên repository (để `index.html` nằm ở thư mục gốc được xuất bản).
2. Vào **Settings → Pages**.
3. Chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi lưu.
4. Đợi GitHub Pages triển khai xong và mở URL được cung cấp.
5. Kiểm tra ảnh và nhạc trên URL đã xuất bản, không chỉ trên máy tính cá nhân.

## Lưu ý
- Website công khai: bất kỳ ai có URL đều có thể xem nội dung và tài nguyên.
- Google Fonts cần kết nối Internet; nếu ngoại tuyến, website dùng font dự phòng.
- Nếu tài nguyên không tải trên GitHub Pages, kiểm tra đúng chữ hoa/thường và đảm bảo đã tải cả thư mục `assets`.
- Đây là website tĩnh; không có hệ thống đăng nhập hoặc bảo vệ nội dung bằng mật khẩu.


## Lưu ý triển khai để tránh lỗi ảnh/nhạc

1. Giải nén ZIP trên máy tính trước khi tải lên GitHub.
2. Đưa `index.html`, `style.css`, `script.js` và thư mục `assets` vào cùng thư mục gốc của repository (không tải nguyên file ZIP lên, không để các file nằm thêm một cấp thư mục).
3. Kiểm tra tên file đúng chữ hoa/chữ thường: `assets/images/huy-tran.jpeg`, `assets/images/thuy-linh.jpeg`, `assets/music/our-song.mp3`.
4. Sau khi GitHub Pages triển khai xong, mở trang, nhấn “Mở cuốn nhật ký”, rồi nhấn nút phát nhạc.
5. Nếu dùng `index-single-standalone.html`, đổi tên thành `index.html` trước khi đặt vào thư mục gốc. Bản standalone nhúng ảnh và nhạc bên trong HTML nên không phụ thuộc thư mục `assets`; dung lượng lớn hơn đáng kể.
