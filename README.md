🛒 Shop Mini App
📌 Giới thiệu

Shop Mini App là một ứng dụng web bán hàng mini được xây dựng bằng HTML, CSS và JavaScript thuần.
Ứng dụng chạy trực tiếp trên trình duyệt, không cần backend, dữ liệu được lưu bằng localStorage.

Mục tiêu của project:

Giao diện shop đơn giản, dễ dùng
Quản lý sản phẩm và giỏ hàng nhanh
Chạy offline trên máy tính hoặc điện thoại
Không cần server hoặc database phức tạp
⚙️ Công nghệ sử dụng
HTML5
CSS3
JavaScript (Vanilla JS)
localStorage (lưu dữ liệu local)
🚀 Cách chạy dự án
Cách 1: Chạy trực tiếp
Tải file shop-mini-fixed.html
Nhấp đúp mở bằng Chrome / Edge
Sử dụng bình thường
Cách 2: Dùng Live Server (khuyến nghị)
Mở VS Code
Cài extension Live Server
Click “Go Live”
📦 Tính năng chính
🛍️ Danh sách sản phẩm
➕ Thêm / xóa sản phẩm
🛒 Giỏ hàng (cart system)
💰 Tính tổng tiền tự động
💾 Lưu dữ liệu bằng localStorage
📱 Giao diện responsive (mobile + desktop)
🧠 Kiến trúc app

App được thiết kế theo mô hình đơn giản:

UI (HTML)
   ↓
Event (onclick / addEventListener)
   ↓
App Object (logic chính)
   ↓
LocalStorage (data persistence)
⚠️ Lưu ý kỹ thuật
Nếu gặp lỗi app is not defined:
→ kiểm tra script load hoặc cần expose window.app
Nếu lỗi Invalid or unexpected token:
→ thường do ký tự lạ hoặc dấu nháy sai trong JS
App không dùng backend nên dữ liệu:
→ chỉ lưu trên trình duyệt hiện tại
