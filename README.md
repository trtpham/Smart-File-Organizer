# Smart File Organizer 📂

![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Giới thiệu
**Smart File Organizer** là công cụ tự động hóa việc dọn dẹp máy tính, giúp sắp xếp các file lộn xộn vào các thư mục tương ứng dựa trên định dạng file. 
Điểm đặc biệt của tool này là khả năng **phát hiện file trùng lặp (Duplicate Detection)** dựa trên nội dung (File Hash) để tiết kiệm dung lượng lưu trữ, thay vì chỉ so sánh tên file.

## Tính năng chính
- [x] 🧹 **Auto Organize:** Tự động di chuyển file vào thư mục (Ảnh, Nhạc, Tài liệu, Code...).
- [x] 🔍 **Deep Deduplication:** Quét và phát hiện file trùng lặp sử dụng thuật toán MD5/SHA256.
- [x] 🛡️ **Safe Mode:** Chế độ "Dry Run" - chỉ báo cáo những gì sẽ làm, không thực hiện di chuyển/xóa thật.
- [x] 📝 **Logging:** Ghi lại nhật ký hoạt động chi tiết để tra cứu.
- [x] ⚙️ **Configurable:** Tùy chỉnh quy tắc dọn dẹp qua file `config.json`.

## Cấu trúc thư mục sau khi dọn dẹp
Downloads/
├── Images/      # .jpg, .png, .gif
├── Documents/   # .pdf, .docx, .xlsx
├── Archives/    # .zip, .rar
├── Setup/       # .exe, .msi
└── Others/      # Các file còn lại

## Cài đặt
1. Clone dự án:
   ### Bash:
   git clone [https://github.com/username/smart-file-organizer.git](https://github.com/username/smart-file-organizer.git)
2. Yêu cầu hệ thống:
   Python 3.10 trở lên.
   Thư viện: Standard Library (không cần cài thêm pip packages).
3. Hướng dẫn sử dụng
   Chạy tool thông qua dòng lệnh:
    1. Chế độ quét thử (Khuyên dùng lần đầu):
    ### Bash:
    python main.py --source "C:/Downloads" --dry-run
    2. Chế độ dọn dẹp thật:
    ### Bash:
    python main.py --source "C:/Downloads"

Tác giả
Pham Minh Triet - []
