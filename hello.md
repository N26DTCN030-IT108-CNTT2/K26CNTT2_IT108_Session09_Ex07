# Phần 1: Phân tích lỗi
1. Liệt kê các lỗi cú pháp trong đoạn Markdown
Lỗi 1 (Heading): Đoạn ###Lưu ý quan trọng viết liền khối ### với chữ Lưu ý mà không có khoảng trắng ở giữa.

Lỗi 2 (List): Các bước -Bước 1:, -Bước 2:, -Bước 3:, -Bước 4: viết liền dấu gạch ngang (-) với từ Bước mà không có khoảng trắng.

Lỗi 3 (Bold & Italic): Định dạng in đậm đoạn tên repository **HNKS25CNTT1_IT101_Session08 bị thiếu dấu sao kép khép lại (**) ở cuối tên, khiến toàn bộ các đoạn văn bản/danh sách phía sau bị ảnh hưởng. Tương tự, cuối câu deadline có dấu gạch ngang và sao chéo —* *Nộp muộn... bị thừa/sai quy cách đóng mở thẻ.

2. Giải thích hậu quả khi hệ thống render
Hậu quả lỗi Heading (###Lưu ý quan trọng): Trình biên dịch Markdown không nhận diện đây là tiêu đề cấp 3 (H3) mà hiển thị thành một dòng chữ bình thường dính liền ký tự ###Lưu ý quan trọng.

Hậu quả lỗi List (-Bước 1:...): Hệ thống không nhận diện đây là các mục danh sách (Bullet list), khiến chúng hiển thị thành các đoạn văn bản thường hoặc dính sát vào nhau thay vì tạo thành các hàng liệt kê rõ ràng.

Hậu quả lỗi Bold / Italic: Do thiếu thẻ đóng **, toàn bộ các dòng văn bản đứng sau đoạn mở ** sẽ bị kích hoạt hiệu ứng in đậm kéo dài liên tục, làm hỏng toàn bộ cấu trúc định dạng của phần cuối trang hướng dẫn.

# Phần 2 Sửa lỗi
## Hướng Dẫn Nộp Bài Tập - Session 08

### Lưu ý quan trọng

Các bước nộp bài:
- Bước 1: Tạo tài khoản GitHub tại [GitHub](https://github.com)
- Bước 2: Tạo repository mới đặt tên theo định dạng **HNKS25CNTT1_IT101_Session08**
- Bước 3: Upload file .md của bài làm lên repository
- Bước 4: Copy đường dẫn và nộp lên *Portal*

> **Deadline:** Chủ nhật 23:59 — *Nộp muộn sẽ bị trừ 50% điểm!*

4. Xử lý bẫy dữ liệu về liên kết (Link)
Hiệu ứng khi quên gõ https://: Nếu sinh viên nhập đường liên kết dạng [GitHub](github.com) mà thiếu tiền tố giao thức (https:// hoặc http://), trình duyệt hoặc trình biên dịch Markdown sẽ hiểu nhầm đó là một đường dẫn tương đối (Relative URL) nằm bên trong thư mục hiện tại của trang web thay vì một địa chỉ tên miền tuyệt đối trên Internet.

Hậu quả: Khi người dùng bấm vào liên kết đó, trình duyệt sẽ bị điều hướng sai sang một đường dẫn dạng [https://lms-student.rikkei.edu.vn/courses/github.com](https://lms-student.rikkei.edu.vn/courses/github.com) (hoặc tên miền hiện tại của trang), dẫn đến lỗi 404 Not Found hoặc không thể mở được trang GitHub.
