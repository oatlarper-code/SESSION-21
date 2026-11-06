# 5.Yêu cầu
1. Phần I. Googling đúng cách
- Câu hỏi mang tính chung vô nghĩa đối với thuật toán tìm kiếm, thiếu các từ khóa chuyên ngành và thiếu mã lỗi nguyên văn với các bài viết kỹ thuật chuyên sâu

|Thành phần|Nội dung bóc tách|
|-|-|
Tên phần mềm/Hệ điều hành|Windows 11/Node.js
Mã lỗi nguyên văn|'npm' is not recognized as an internal or external command, operable program or batch file.
Thao tác đang làm|gõ lệnh npm -v trong terminal để kiểm tra cài đặt sau khi cài node.js
> 3 câu truy vấn google tối ưu
- site:stackoverflow.com "'npm' is not recognized as an internal or external command"
- "npm is not recognized as an internal or external command" windows 
- npm is not recognized as an internal or external command nodejs -xp
2. Phần II. Thẩm định StackOverflow

|Tiêu chí|Câu trả lời A|Câu trả lời B
Vote & Tích xanh|Có tích xanh|không có tích xanh
Thời gian đăng bài|2 năm trước|9 năm trước
Tags khớp hệ điều hành/phần mềm|Khớp hoàn toàn|không phù hợp

- Lựa chọn áp dụng câu trả lời A. Vì câu trả lời B là bẫy nguy hiểm hệ điều hành từ 9 năm trước không phù hợp với sự phát triển bây giờ 
- Bước 1: Nhìn biểu tượng tích xanh. Bước 2: Đọc nhanh các Tags ở đầu bài viết. Bước 3: Đọc lướt trực tiếp vào đoạn mã lệnh/giải pháp được bôi đậm trong phần nội dung trả lời
3. Phần III. Hỏi AI đúng cách và nhận diện rủi ro 
> Công thức Prompt hoàn chỉnh gửi cho trợ lý AI
- Tôi đang dùng máy tính Windows 11 cài node.js để làm bài tập lập trình web. Khi mở Terminal, Vsc để kiểm tra thì tôi gặp sự cố hệ thống không nhận lệnh npm. Tôi đã thực hiện theo hướng dẫn thêm đường dẫn và thử lại Terminal nhưng vẫn bị lỗi 'npm' is not recognized as an internal or external command, operable program or batch file. Hãy dịch sang tiếng việt và phân tích nguyên nhân, giải pháp các bước để sửa lỗi
> 3 Nguyên tắc vàng
- Không nên làm theo vì lệnh `del /f /s /q C:\Windows\System32\*` là lệnh nguy hiểm có chức năng xóa hết các tệp tin trong file system32 của windows với Administrator. Nếu thực thi lệnh này hệ điều hành sẽ bị hỏng và phải cài lại win
- Tôi sẽ phản hồi với AI là: "Lệnh `del /f /s /q C:\Windows\System32\*` là gì và tại sao nó lại nguy hiểm khi thực hiện
4. Phần IV. Viết Bug Report chuẩn để nhờ hỗ trợ
- "Thầy ơi, giúp em với em không hiểu tại sao cái này không hoạt động thầy giúp em được không ạ."

|Mảnh ghép|Nội dung trong tin nhắn của bạn
|-|-|
Context|Đang dùng windows 11 cài node.js và thực hiện đường dẫn tới Stackoverflow không thành công
Expected|Gõ lệnh npm -v trong terminal màn hình phải trả về số phiên bản của npm
Actual|gặp lỗi "npm is not recognized as an internal or external command"
Log & Screenshot|Chụp màn hình Terminal hiển thị nguyên văn câu lệnh npm -v và dòng thông báo lỗi màu đỏ


- Phím tắt chụp màn hình: Windows + Shift + S
- Lưu ý: Cần đảm bảo ảnh không bị gặp vấn đề gì trước khi gửi. Không để lộ thông tin cá nhân.