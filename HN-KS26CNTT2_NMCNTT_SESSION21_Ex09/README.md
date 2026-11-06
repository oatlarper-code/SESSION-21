# 5.Yêu cầu đầu ra
1. Phần I. Thiết kế Prompt 3 Thành phần chuẩn hóa
- Nguyên nhân AI trả lời sai lệnh do thiếu ngữ cảnh cụ thể và suy diễn sai bản chất vấn đề
- 3 câu prompt hoàn chỉnh: Tôi đang làm việc vì gặp sự cố ERROR trong file log "2000-02-12 21:15:30 [ERROR] Computer failed to start.". Hãy giải thích lỗi này bằng tiếng việt sau đó đưa ra các bước cụ thể để sửa lỗi.
2. Phần II. Giải mã lỗi và kịch bản khắc phục
- `UnauthorizedAccessException: Access to the path ... is denied` là ""lỗi truy cập chưa có sự cho phép: Đường dẫn bị từ chối""
- Nguyên nhân là: Thư mục nằm trong ổ đĩa chính của máy tính. Window 11 bắt buộc phải chặn tài khoản đang chạy không có quyền truy cập vào thư mục này. Kết quả là bị hủy với mã lỗi.
> 3 bước xử lý cụ thể tại chỗ
- Bước 1: Mở ứng dụng hoặc Terminal với quyền quản trị viên
- Bước 2: Cấp quyền ghi cho file data
- Bước 3: Khởi động lại hệ thống
- Phân quyền cho thư mục data: Chuyển đường dẫn đến thư mục Data -> Chuột phải chọn Properties -> Chuyển sang Security -> Nhấn edit -> chọn tài khoản đang dùng và tích chọn Full Control hoặc Modify ở cột Allow -> Tích apply và Ok
- Xử lý bẫy an ninh:
  - Xóa bỏ hoặc thay chuỗi khóa bị mật. Lý do Tránh việc rò rĩ mã khóa API nội bộ ra bên ngoài từ đó ngăn chặn bị xâm nhập. Tránh gửi mã Secret, mật khẩu cơ sở hay mã OTP ra ngoài hay AI.