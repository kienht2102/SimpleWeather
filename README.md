# 🌤️ App Xem Thời Tiết Đơn Giản

![Tailwind v4](https://img.shields.io/badge/Tailwind_CSS-v4.0-blue?style=flat&logo=tailwind-css)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?style=flat&logo=javascript)

Một ứng dụng web một trang (Single Page Application) giúp tra cứu thông tin thời tiết hiện tại của bất kỳ thành phố nào trên thế giới bằng cách kết nối với API của OpenWeatherMap. Giao diện được thiết kế hiện đại theo phong cách Glassmorphism (hiệu ứng kính mờ).

## 📸 Màn hình Demo ứng dụng

### 1. Giao diện chính khi khởi động
![Giao diện lúc chưa tìm kiếm](<img width="1920" height="928" alt="1" src="https://github.com/user-attachments/assets/ad81a251-0032-494e-9dd1-74b522da93ff" />
)

*Giao diện trang chủ khi chưa nhập tên thành phố*

---

### 2. Kết quả hiển thị dữ liệu thời tiết thành công
![Giao diện trả về kết quả thành công](<img width="1920" height="925" alt="2" src="https://github.com/user-attachments/assets/1f987cfc-ada5-46f8-8799-01f2a2eaf3a8" />
)

*Thông tin thời tiết thực tế chi tiết sau khi tìm kiếm thành công*

---

### 3. Trạng thái thông báo lỗi
![Giao diện thông báo lỗi](<img width="1920" height="928" alt="3" src="https://github.com/user-attachments/assets/389639e8-9668-44f4-86a3-d1d2a31e0251" />
)

*Màn hình thông báo lỗi khi hệ thống không tìm thấy tên thành phố*

---

## 📌 Tính năng nổi bật
* **Tìm kiếm thời gian thực**: Tra cứu thời tiết theo tên thành phố (hỗ trợ cả tiếng Việt có dấu nhờ chuẩn hóa NFC).
* **Thông tin chi tiết**: Hiển thị tên quốc gia, trạng thái thời tiết, nhiệt độ thực tế (36°C), độ ẩm (52%) và tốc độ gió (2.99 m/s).
* **Hiệu ứng trực quan**: Tự động thay đổi Icon thời tiết tương ứng với trạng thái trời nắng, mưa, mây, v.v.
* **Xử lý lỗi & Chờ tải**: Tích hợp màn hình chờ (Loading spinner) và thông báo lỗi thân thiện khi nhập sai tên thành phố hoặc lỗi API.
* **Giao diện Responsive**: Thân thiện và tự động co giãn đẹp mắt trên cả máy tính và điện thoại di động nhờ Tailwind CSS v4.

## 🛠️ Công nghệ sử dụng
* **HTML5**: Cấu trúc ngữ nghĩa của trang web.
* **Tailwind CSS (v4 @browser CDN)**: Xử lý giao diện hiện đại, nhanh chóng thông qua CDN.
* **Vanilla JavaScript (ES6+)**: Xử lý logic gọi API (`fetch`, `async/await`) và cập nhật giao diện (DOM manipulation).
* **OpenWeatherMap API**: Nguồn dữ liệu thời tiết (Endpoint: `Current Weather Data`).

## 🚀 Hướng dẫn chạy ứng dụng

Vì đây là một ứng dụng giao diện tĩnh (Frontend thuần), bạn không cần cài đặt bất kỳ môi trường phức tạp nào.

1. **Tải mã nguồn về máy:**
   Bạn có thể tải file `.html` hoặc clone repository này về.
2. **Mở ứng dụng:**
   Click đúp chuột thẳng vào file `index.html` để mở bằng bất kỳ trình duyệt nào (Chrome, Edge, Safari, Firefox).
   * *Khuyến khích*: Sử dụng extension **Live Server** trên VS Code để có trải nghiệm hot-reload tốt nhất.

## ⚙️ Cấu hình API Key

Hiện tại, ứng dụng đang sử dụng một API Key có sẵn trong mã nguồn:
```javascript
const API_KEY = "0c973805000feed002175af2a37f7a25";
