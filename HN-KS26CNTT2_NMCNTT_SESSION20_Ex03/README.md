# 3.Yêu cầu đầu ra
> Báo cáo phân tích (IPO)
- Input: gõ lệnh Git và nhận được thông báo: "fatal: not a git repository (or any of the parent directories): .git"
- Process: AI dịch sang tiếng việt và giải thích nguyên nhân. Nguyên nhân git init(chưa chạy lệnh), cd(chưa chuyển vào thư mục dự án mã nguồn)
- Output: Hướng dẫn 3 bước khác phục. Bước 1: Kiểm tra thư mục hiện tại, Bước 2: Di chuyển vào thư mục dự án chạy lệnh git init, Bước 3: Kiểm tra lại Git để xác nhận đã khắc phục xong
- Câu lệnh Prompt hoàn chỉnh:
  - Tôi đang việc và gặp phải thông báo lỗi lệnh Git "fatal: not a git repository (or any of the parent directories): .git". Hãy phiên dịch lỗi sang tiếng việt và giải thích cho tôi tại sao lại xảy ra kèm theo hướng dẫn 3 bước sửa lỗi.