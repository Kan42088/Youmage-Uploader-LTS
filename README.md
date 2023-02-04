# Youmage-Uploader-LTS

*Note: 
- Phần mềm là file rar trong file được tải về.
- Tải file json authen tại https://console.cloud.google.com/apis/dashboard mục Credentials phần OAuth 2.0 Client IDs. Lần đầu tiên chạy app có thể sẽ phải cấp quyền cho tài khoản gmail để đăng video lên youtube.
- Khi dùng phương thức tải video bằng browser, đảm bảo cập nhật chromedriver.exe trùng với phiên bản chrome đang dùng được cài trên máy, cập nhật chromedriver.exe mới nhất tại https://chromedriver.chromium.org/downloads phiên bản cho win32. Tải chromedriver về, giải nén và replace vào thư mục chứa tool.
- Khi dùng phương thức tải video bằng api, key api được lấy từ: https://account.api2convert.com/user/apikeys .
- Khi dùng phương thức xử lí bằng FFmpeg phải cài đặt ffmpeg tại https://www.gyan.dev/ffmpeg/builds/ .
- Bản ổn định hiện tại: v1.10.0

*Bản 1.10.0:
- Thêm tính năng cho phép tải video về thư mục được chọn.
- Cho phép lựa chọn upload hoặc không upload lên youtube.

*Bản 1.9.2:
- Thêm tính năng xử lý video bằng FFmpeg.
- Nên copy dữ liệu trên các control nhập liệu, không nên copy file config do cấu hình của google không tương thích ngược.

*Bản 1.9.0:
- Thêm tính năng xử lý video bằng FFmpeg.

*Bản 1.8.5:
- Thêm hàng đợi phản hồi từ server api2convert.

*Bản 1.8.4:
- Chuyển đổi gọi api qua resharp thành httpwebrequest.

*Bản 1.8.2:
- Hiển thị innerException để bắt lỗi chưa xác định.

*Bản 1.8.0:
- Thêm bộ lọc sản phẩm theo thời gian.
- Thêm tùy chọn bộ lọc cho sản phẩm.
- Thêm tùy chọn phương thức tải video theo api của api2convert.

*Bản 1.5.2:
- Sửa lỗi màn login không tự lưu tài khoản đăng nhập trước đó.
- Thêm snippet {tags}: Tạo chuỗi tag từ các tag của sản phẩm.
- Thêm snippet {hashtags}: Tạo chuỗi hashtag từ các tag của sản phẩm.

*Bản 1.4.1:
- Sửa lỗi upload video lên youtube bị đứng sau khi tải video đầu.

*Bản 1.4.0:
- Tùy chỉnh title và desc của video (bao gồm các snippet variables);

*Bản 1.3.1:
- kiểm tra quá trình tải ảnh lên trang video.online-convert;
- sửa lỗi lấy video tag.
- Cho phép bật tắt hiển thị quá trình tải của browser.

*Bản 1.1.0:
- thay đổi tên mô tả video thành "(#tên web) (link sản phẩm)" .

*Bản 1.0.0:
- Tải danh sách sản phẩm từ woocommerce.
- Tải ảnh từ sản phẩm lấy được, tự động dùng https://video.online-convert.com/convert-to-mp4 để tạo video.
- Upload video kèm thông tin sản phẩm lên youtube.
- Lưu thông tin danh sách sản phẩm đã tải lên youtube kèm tránh upload trùng video.
