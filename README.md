
# Telegram Bot Điều Khiển Windows Từ Xa
Một bot Telegram cho phép điều khiển và giám sát máy tính Windows từ xa thông qua các lệnh đơn giản. Bot này có thể thực hiện nhiều hành động như lấy mật khẩu trình duyệt, ghi lại phím nhấn (Keylogger), chụp màn hình, mở URL, và hơn thế nữa.
Lưu ý: Script này chỉ hoạt động trên hệ điều hành Windows.

## Tính Năng

🔑 Lấy mật khẩu từ các trình duyệt phổ biến như Chrome, Edge, Brave, CocCoc.
⌨️ Ghi lại phím nhấn (keylogger) và gửi log qua Telegram.
📸 Chụp màn hình và gửi qua Telegram.
🌐 Mở URL trong trình duyệt Chrome.
📂 Tìm và gửi các file quan trọng (.txt, .docx, .pdf, .jpg, .png) từ các ổ đĩa.
🛑 Tắt máy hoặc khởi động lại máy.
🔓 Bỏ qua UAC để chạy với quyền admin.
💾 Tự sao lưu và chống xóa.
🕵️ Ẩn console để hoạt động ngầm.
💓 Heartbeat để xác nhận bot còn hoạt động.


## Cài Đặt

Cài đặt Python 3.x từ python.org.
Cài đặt các thư viện cần thiết:pip install -r requirements.txt


Tạo bot Telegram:
Tạo bot mới qua BotFather và lấy BOT_TOKEN.
Lấy CHAT_ID của nhóm hoặc người dùng mà bot sẽ gửi tin nhắn đến.


Cập nhật script:
Thay thế BOT_TOKEN và CHAT_ID trong file main.py.


Chạy script:python main.py



Chú ý: Script sẽ tự động ẩn console và chạy ngầm. Nó cũng cố gắng bypass UAC để có quyền admin. Do tính chất của các hành động này, script có thể bị phát hiện bởi phần mềm diệt virus.

## Sử Dụng
Sau khi bot đã chạy, bạn có thể gửi các lệnh sau đến bot qua Telegram:

/lay_pass: Lấy mật khẩu từ trình duyệt.
/lay_keylog: Xem log phím nhấn.
/chup_man_hinh: Chụp màn hình.
/mo_url <url>: Mở URL trong Chrome (ví dụ: /mo_url google.com).
/lay_file: Tìm và gửi file quan trọng.
/shutdown: Tắt máy.
/restart: Khởi động lại máy.
/help: Hiển thị danh sách lệnh.


🔧 Biến Script Thành EXE
Để biến script thành file EXE độc lập, bạn có thể sử dụng PyInstaller:

Cài đặt PyInstaller:pip install pyinstaller


Chạy lệnh sau để biên dịch script:pyinstaller --onefile --noconsole main.py


File EXE sẽ được tạo trong thư mục dist.

Lưu ý: Khi chạy file EXE, nó sẽ tự động ẩn console và chạy ngầm.

⚠️ Tuyên Bố Từ Chối Trách Nhiệm
Script này được tạo ra với mục đích giáo dục và thử nghiệm. Việc sử dụng script này để xâm nhập hoặc giám sát máy tính của người khác mà không có sự cho phép là bất hợp pháp và vi phạm đạo đức. Người dùng chịu hoàn toàn trách nhiệm về cách họ sử dụng script này.

🤝 Đóng Góp
Nếu bạn muốn đóng góp vào dự án, vui lòng fork repository và gửi pull request với các cải tiến hoặc sửa lỗi.

📜 Giấy Phép
Script này được phát hành dưới giấy phép MIT.
