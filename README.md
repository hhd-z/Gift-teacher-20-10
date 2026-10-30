<div align="center">

# 💌 Royal 3D Greeting Card • Tri Ân GV 20/10 🌸

**Ứng dụng Web Thiệp Chúc Mừng Ngày Phụ Nữ Việt Nam 20/10 Tương Tác 3D Phong Cách Hoàng Gia**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript_ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Web Audio API](https://img.shields.io/badge/Web_Audio_API-FF4081?style=for-the-badge&logo=applemusic&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=for-the-badge&logo=github&logoColor=white)](https://pages.github.com/)

<p align="center">
  <em>Món quà công nghệ tinh tế kết hợp nghệ thuật thị giác 3D CSS, âm thanh hộp nhạc tổng hợp thời gian thực và khả năng cá nhân hóa động qua URL, dành tặng Giáo Viên (GV) nhân dịp 20/10.</em>
</p>

[✨ Xem Demo Trực Tiếp](#) • [📖 Tính Năng](#-tính-năng-nổi-bật) • [🚀 Cài Đặt](#-hướng-dẫn-triển-khai) • [🔗 Cá Nhân Hóa Link](#-cá-nhân-hóa-thiệp-bằng-url-parameters)

</div>

---

## 📌 Tổng Quan Dự Án (Overview)

**Royal 3D Greeting Card (20/10 Edition)** là một ứng dụng web đơn trang (Single-File Web Application) được thiết kế nhằm mang lại trải nghiệm mở thiệp vật lý chân thực ngay trên trình duyệt. Thay vì chỉ hiển thị văn bản tĩnh, người nhận sẽ trực tiếp tương tác với **Con dấu sáp Hoàng Gia đúc nổi 3D**, lắng nghe tiếng chuông gió ngân vang khi tháo dải ruy-băng lụa và đọc tâm thư trên nền giấy cổ điển cùng giai điệu hộp nhạc êm dịu.

Dự án được đóng gói **100% độc lập trong một file `index.html` duy nhất**, không phụ thuộc vào cơ sở dữ liệu hay tệp âm thanh/hình ảnh bên ngoài, đảm bảo tốc độ tải trang tức thì và hoạt động bền bỉ trên GitHub Pages.

---

## ✨ Tính Năng Nổi Bật (Key Features)

| Tính năng | Mô tả chi tiết |
| :--- | :--- |
| **✉️ Phong Thư 3D & Con Dấu Sáp** | Sử dụng CSS `perspective: 1600px` và `transform-style: preserve-3d`. Khi nhấn vào con dấu sáp SVG đa lớp, dải ruy-băng lụa tự động rút mở, nắp thư lật 180 độ và lá thư bên trong trồi lên mượt mà. |
| **📜 Giấy Thư Chuẩn Dòng Kẻ 100%** | Hệ thống lưới dòng kẻ cổ điển (`repeating-linear-gradient`) được đồng bộ toán học với biến `--line-h` (`34px` trên Mobile, `38px` trên Desktop), đảm bảo chân chữ tiếng Việt luôn nằm ngay ngắn trên đường kẻ chỉ vàng ở mọi kích thước màn hình. |
| **🎵 Hộp Nhạc Web Audio API** | Tự động tổng hợp âm thanh chuông gió (Chime) khi mở niêm phong và phát giai điệu hộp nhạc (Music Box) đa âm sắc bằng bộ dao động sóng Sine (`OscillatorNode`), không cần tải file `.mp3` ngoài. |
| **🌸 Hiệu Ứng Hạt Canvas 2D** | Hệ thống hạt vật lý 60fps tái hiện cánh hoa hồng, trái tim và kim tuyến vàng bay lơ lửng; tích hợp hiệu ứng pháo hoa bung tỏa từ tâm con dấu khi mở thư. |
| **✍️ Cá Nhân Hóa & Xuất Link Động** | Tích hợp trình chỉnh sửa trực tiếp trên giao diện (Modal), cho phép đổi tên GV, chọn 4 mẫu lời chúc có sẵn, sửa chữ ký và tự động mã hóa vào đường dẫn URL để gửi riêng cho từng GV. |
| **📱 Tối Ưu Đa Thiết Bị (Responsive)** | Sử dụng hàm `clamp()` của CSS kết hợp với Tailwind CSS để tự động co giãn tỷ lệ phong thư và khung thư hoàn hảo trên cả Smartphone, Tablet và PC. |

---

## 🛠️ Kiến Trúc & Công Nghệ (Tech Stack)

* **Giao diện & Bố cục:** HTML5 Semantic, Tailwind CSS (v3.x qua CDN).
* **Đồ họa & Hoạt ảnh:**
  * **CSS3 3D Transforms & Keyframes:** Xử lý chuyển động lơ lửng (`floatLuxury`), ánh kim quét qua con dấu (`metallicSweep`) và sóng hào quang (`auraPulse`).
  * **Inline SVG & Filters:** Chế tác con dấu sáp đỏ Burgundy mạ vàng cùng 4 góc hoa văn cổ điển (Filigree Frame) sắc nét ở mọi độ phân giải.
  * **HTML5 Canvas 2D:** Xử lý hệ thống hạt mưa hoa thời gian thực.
* **Âm thanh:** Web Audio API (`AudioContext`, `OscillatorNode`, `GainNode`).
* **Typography (Google Fonts):**
  * `Dancing Script`: Chữ viết tay thư pháp cho tiêu đề và lời chào.
  * `Cormorant Garamond`: Phông chữ có chân cổ điển sang trọng cho nội dung bức thư.
  * `Plus Jakarta Sans`: Phông chữ hiện đại, rõ nét cho thanh công cụ và nút bấm.

---

## 📂 Cấu Trúc Thư Mục (Project Structure)

```text
📦 thiep-20-10-gv
 ┣ 📜 index.html      # Toàn bộ mã nguồn Giao diện (HTML), Hoạt ảnh 3D (CSS) và Logic (JS)
 ┗ 📜 README.md       # Tài liệu hướng dẫn và mô tả dự án chuyên nghiệp
```

---

## 🚀 Hướng Dẫn Triển Khai (Deployment Guide)

### 1. Chạy thử nghiệm trên máy cá nhân (Local)
Không cần cài đặt Node.js hay bất kỳ thư viện nào:
1. Tải hoặc clone kho lưu trữ này về máy:
   ```bash
   git clone https://github.com/<username-cua-ban>/<ten-repo>.git
   ```
2. Mở trực tiếp tệp `index.html` bằng trình duyệt bất kỳ (Chrome, Safari, Edge, Firefox).

### 2. Triển khai miễn phí lên GitHub Pages
1. Đẩy file `index.html` và `README.md` lên kho lưu trữ (Repository) trên GitHub của bạn.
2. Truy cập vào tab **Settings** trên thanh menu của Repository.
3. Chọn mục **Pages** ở thanh công cụ bên trái.
4. Tại phần **Build and deployment** > **Branch**, chọn nhánh `main` (hoặc `master`), thư mục `/(root)` và nhấn **Save**.
5. Đợi khoảng 30–60 giây để GitHub khởi tạo trang web, sau đó truy cập vào đường dẫn:
   `https://<username-cua-ban>.github.io/<ten-repo>/`

---

## 🔗 Cá Nhân Hóa Thiệp Bằng URL Parameters

Bạn có thể tạo hàng loạt thiệp cho nhiều GV khác nhau mà **không cần sửa lại mã nguồn** bằng hai cách:

### Cách 1: Sử dụng công cụ trực quan trên Web (Khuyên dùng)
1. Mở trang web thiệp lên, nhấn vào nút **"✍️ Sửa lời chúc"** ở góc trên bên phải.
2. Nhập tên GV, chọn mẫu lời chúc hoặc tự viết tâm thư và nhập tên tập thể lớp/học sinh.
3. Nhấn nút **"🔗 Sao chép Link gửi GV"**. Hệ thống sẽ tự động tạo một đường dẫn chứa toàn bộ thông tin bạn vừa nhập vào bộ nhớ tạm để bạn gửi qua Zalo/Messenger.

### Cách 2: Truyền tham số trực tiếp qua URL
Ứng dụng hỗ trợ 3 tham số truy vấn (Query Parameters) chuẩn UTF-8:

| Tham số | Ý nghĩa | Giá trị mặc định |
| :--- | :--- | :--- |
| `to` | Tên người nhận hiển thị ngoài phong bì và đầu thư | `GV` |
| `msg` | Nội dung chính của bức thư (hỗ trợ xuống dòng `\n\n`) | *Mẫu lời chúc số 1* |
| `from` | Chữ ký người gửi / Tập thể lớp ở cuối thư | `Tập thể học sinh yêu quý của GV ❤️` |

**Ví dụ đường dẫn tùy chỉnh:**
```text
https://<username>.github.io/<repo>/?to=GV%20Chủ%20Nhiệm&from=Tập%20thể%20lớp%2012A1
```

---

## 📱 Khả Năng Tương Thích (Browser Compatibility)

* ✅ **Desktop:** Google Chrome, Microsoft Edge, Mozilla Firefox, Apple Safari.
* ✅ **Mobile / Tablet:** iOS Safari, Android Chrome, trình duyệt tích hợp trong Zalo / Messenger.

---

<div align="center">
  <p>Được thiết kế và phát triển với tất cả lòng biết ơn dành tặng <strong>GV</strong> nhân ngày Phụ nữ Việt Nam 20/10 💐</p>
  <p>Nếu bạn thấy dự án này ý nghĩa, hãy tặng một ⭐ <strong>Star</strong> trên GitHub nhé!</p>

![QR Donate](./donatee.png)

</div>
