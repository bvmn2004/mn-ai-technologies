# MN AI Technologies – Website Giới Thiệu Giải Pháp AI Doanh Nghiệp

Website tĩnh chính thức của **MN AI Technologies** – Startup công nghệ chuyên cung cấp giải pháp AI Chatbot, AI Agent, SaaS và tự động hóa quy trình nghiệp vụ cho doanh nghiệp Việt Nam.

- **Tên thương hiệu:** MN AI Technologies (Viết tắt: **MN AI**)
- **Slogan:** *Giải pháp AI thông minh cho doanh nghiệp Việt*
- **Tên miền chính thức:** [https://mnaitechnologies.tech](https://mnaitechnologies.tech)
- **Email liên hệ:** [minz@mnaitechnologies.tech](mailto:minz@mnaitechnologies.tech)
- **Địa chỉ:** 59 Khương Hữu Dụng, Hòa Xuân, Cẩm Lệ, Đà Nẵng, Việt Nam
- **Mốc khởi động nghiên cứu:** Từ năm 2024 (R&D mô hình ngôn ngữ lớn và xử lý tiếng Việt)
- **Giai đoạn phát triển hiện tại (2026):** Thử nghiệm Private Beta, đang hoàn thiện thủ tục pháp nhân doanh nghiệp theo quy định

---

## 🚀 Mục Lục

1. [Tổng Quan Kiến Trúc & Công Nghệ](#-tổng-quan-kiến-trúc--công-nghệ)
2. [Cấu Trúc Thư Mục & Danh Sách Trang](#-cấu-trúc-thư-mục--danh-sách-trang)
3. [Chạy Thử Nghiệm Cục Bộ (Local Testing)](#-chạy-thử-nghiệm-cục-bộ-local-testing)
4. [Hướng Dẫn Triển Khai GitHub Pages](#-hướng-dẫn-triển-khai-github-pages)
5. [Cấu Hình DNS Tên Miền Tùy Chỉnh (mnaitechnologies.tech)](#-cấu-hình-dns-tên-miền-tùy-chỉnh-mnaitechnologiestech)
6. [Danh Sách Cần Bổ Sung (TODO Checklist Cho Chủ Dự Án)](#-danh-sách-cần-bổ-sung-todo-checklist-cho-chủ-dự-án)
7. [Bản Quyền & Giấy Phép](#-bản-quyền--giấy-phép)

---

## 🛠 Tổng Quan Kiến Trúc & Công Nghệ

Website được xây dựng theo mô hình **trang tĩnh 100% (Pure Static HTML/CSS/JS)**, không phụ thuộc vào máy chủ Node.js, Docker hay hệ thống backend runtime, đảm bảo tốc độ tải cực nhanh, bảo mật cao và tương thích hoàn hảo với GitHub Pages, Cloudflare Pages, Vercel, Netlify.

- **UI Framework:** Bootstrap 5.3 (Responsive Grid, Modals, Flex utilities)
- **Styling:** CSS3 tùy chỉnh theo Design System thương hiệu MN AI (hỗ trợ Light / Dark Mode tự động lưu `localStorage`)
- **Biểu tượng (Icons):** Font Awesome 6 (SVG / Webfonts)
- **Hiệu ứng động (Animation):** AOS (Animate On Scroll)
- **Thư viện trượt (Slider):** Swiper.js
- **Biểu đồ trực quan:** Chart.js (tùy biến giao diện số liệu minh họa)
- **Bảo mật:** Tuyệt đối không nhúng API Key (OpenAI, Anthropic Claude, Gemini) phía frontend.

---

## 📂 Cấu Trúc Thư Mục & Danh Sách Trang

```text
ka-saas-landing-page/
├── CNAME                    # Cấu hình tên miền mnaitechnologies.tech cho GitHub Pages
├── README.md                # Tài liệu hướng dẫn kỹ thuật & triển khai
├── 404.html                 # Trang báo lỗi 404 tiếng Việt
├── about.html               # Giới thiệu MN AI: Sứ mệnh, tầm nhìn, giá trị & lộ trình
├── blog.html                # Danh mục bài viết công nghệ AI & tự động hóa doanh nghiệp
├── blog-post.html           # Chi tiết bài viết: AI Chatbot thế hệ mới & Kiến trúc RAG
├── blog-post-agent.html     # Chi tiết bài viết: AI Agent & Tự động hóa quy trình nghiệp vụ
├── blog-post-security.html  # Chi tiết bài viết: Chiến lược bảo mật dữ liệu nội bộ
├── blog-post-sme-roi.html   # Chi tiết bài viết: Tối ưu chi phí CSKH đa kênh cho SME
├── blog-post-comparison.html # Chi tiết bài viết: So sánh Chatbot kịch bản vs. AI Chatbot
├── blog-post-automation.html # Chi tiết bài viết: Tự động hóa luồng tiếp nhận Zalo OA vào CRM
├── contact.html             # Trang liên hệ: Bản đồ, địa chỉ Đà Nẵng, email & form tư vấn
├── features.html            # Tính năng giải pháp: Chatbot, Agent, Dashboard, Security, API
├── index.html               # Trang chủ chính thức MN AI Technologies
├── integrations.html        # Danh mục tích hợp hệ sinh thái (Dự kiến hỗ trợ vs. Lộ trình nghiên cứu)
├── login.html               # Trang đăng nhập (Thông báo chương trình Private Beta)
├── pricing.html             # Bảng gói giải pháp: Starter, Growth, Enterprise (Báo giá may đo)
├── privacy.html             # Chính sách bảo mật dữ liệu khách hàng (Bản nháp hoạt động thực tế)
├── register.html            # Trang đăng ký dùng thử có kiểm duyệt (Private Beta Waitlist)
├── terms.html               # Điều khoản dịch vụ & sử dụng nền tảng AI
├── ui-kit.html              # Bộ tài nguyên giao diện & Design System mẫu
│
├── assets/
│   ├── css/                 # File stylesheet chính (style.css, bootstrap, swiper, aos)
│   ├── js/                  # JavaScript logic (main.js, bootstrap, swiper, aos, chart)
│   └── images/              # Logo SVG, Favicon vector, hình ảnh giải pháp & đối tác
└── screenshot/              # Ảnh chụp giao diện minh họa
```

---

## 💻 Chạy Thử Nghiệm Cục Bộ (Local Testing)

Vì đây là website tĩnh thuần túy, bạn có thể kiểm tra trực tiếp mà không cần cài đặt Node.js hay cơ sở dữ liệu:

### Cách 1: Mở trực tiếp bằng trình duyệt
Nhấp đúp chuột vào file `index.html` hoặc chuột phải chọn **Open with** -> Google Chrome / Microsoft Edge / Brave.

### Cách 2: Sử dụng VS Code Live Server (Khuyên dùng)
1. Cài đặt tiện ích mở rộng **Live Server** trên Visual Studio Code.
2. Chuột phải vào file `index.html` và chọn **Open with Live Server**.
3. Trang web sẽ mở tại địa chỉ `http://127.0.0.1:5500/index.html`.

### Cách 3: Sử dụng Python HTTP Server (Nếu máy đã có Python)
Chạy lệnh sau trong thư mục dự án:
```bash
python -m http.server 8000
```
Sau đó truy cập trình duyệt tại: `http://localhost:8000`

---

## 🌐 Hướng Dẫn Triển Khai GitHub Pages

Website đã được chuẩn bị sẵn sàng cho việc lưu trữ miễn phí, băng thông cao và chứng chỉ SSL miễn phí trên **GitHub Pages**.

### Bước 1: Khởi tạo và đẩy code lên GitHub Repository
Nếu bạn chưa đưa mã nguồn lên GitHub, mở terminal tại thư mục dự án và thực hiện:
```bash
git init
git add .
git commit -m "feat: release MN AI Technologies Vietnamese landing page"
git branch -M main
git remote add origin https://github.com/<username>/<ten-repository>.git
git push -u origin main
```

### Bước 2: Kích hoạt GitHub Pages
1. Truy cập vào Repository của bạn trên trình duyệt GitHub.
2. Nhấp vào tab **Settings** (Cài đặt) ở thanh menu trên cùng.
3. Ở menu bên trái, tìm mục **Code and automation** -> chọn **Pages**.
4. Tại phần **Build and deployment**:
   - **Source:** Chọn `Deploy from a branch`.
   - **Branch:** Chọn branch `main` (hoặc `master`), thư mục chọn `/ (root)`.
   - Nhấn **Save**.

---

## 🔒 Cấu Hình DNS Tên Miền Tùy Chỉnh (mnaitechnologies.tech)

Dự án đã có sẵn file `CNAME` tại thư mục gốc chứa giá trị `mnaitechnologies.tech`. Để tên miền hoạt động chính xác với GitHub Pages:

### Bước 1: Cấu hình bản ghi DNS tại nhà cung cấp tên miền
Đăng nhập vào trang quản trị tên miền của bạn (Namecheap, Cloudflare, GoDaddy, Pavietnam, Matbao, v.v.) và thêm các bản ghi DNS sau:

#### 1. Bản ghi A Records (Trỏ tên miền gốc `@` về cụm máy chủ GitHub Pages):
Thêm 4 bản ghi `A` với tên Host là `@` (hoặc để trống tùy nhà cung cấp):

| Loại (Type) | Tên (Host / Name) | Giá trị (Target / IP Address) | TTL |
| :--- | :--- | :--- | :--- |
| **A** | `@` | `185.199.108.153` | Auto / 3600 |
| **A** | `@` | `185.199.109.153` | Auto / 3600 |
| **A** | `@` | `185.199.110.153` | Auto / 3600 |
| **A** | `@` | `185.199.111.153` | Auto / 3600 |

#### 2. Bản ghi CNAME Record (Trỏ tiền tố `www` về tên miền chính):

| Loại (Type) | Tên (Host / Name) | Giá trị (Target) | TTL |
| :--- | :--- | :--- | :--- |
| **CNAME** | `www` | `<username>.github.io.` hoặc `mnaitechnologies.tech.` | Auto / 3600 |

> *Ghi chú:* Thay `<username>` bằng tên tài khoản GitHub của bạn.

### Bước 2: Bật Custom Domain & HTTPS trong GitHub
1. Quay lại trang **Settings** -> **Pages** trên GitHub.
2. Kiểm tra phần **Custom domain**, đảm bảo đã hiển thị `mnaitechnologies.tech`.
3. Nhấn nút **Save** (nếu chưa lưu) và chờ GitHub tiến hành kiểm tra DNS (DNS check).
4. Sau khi DNS được xác thực (thường mất từ vài phút đến tối đa 24 giờ):
   - Đánh dấu chọn ô **Enforce HTTPS** để buộc tất cả truy cập chuyển hướng sang giao thức mã hóa `https://`.

---

## 📝 Danh Sách Cần Bổ Sung (TODO Checklist Cho Chủ Dự Án)

Để đảm bảo tính minh bạch, trung thực và tuân thủ pháp lý doanh nghiệp, toàn bộ các vị trí chưa có thông tin chính thức đã được gắn thẻ `<!-- TODO: ... -->` trong mã nguồn. Chủ dự án vui lòng rà soát và cập nhật:

- [ ] **Thông tin pháp nhân & Mã số thuế:**
  - Bổ sung tên đầy đủ công ty/hộ kinh doanh, số đăng ký doanh nghiệp tại `about.html`, `privacy.html`, `terms.html` và footer các trang.
- [ ] **Số điện thoại Hotline:**
  - Cập nhật số điện thoại chính thức tại `contact.html` (hiện đang hiển thị hướng dẫn ưu tiên liên hệ qua email `minz@mnaitechnologies.tech`).
- [ ] **Tích hợp Backend xử lý biểu mẫu (Form Submission):**
  - Hiện tại, file `assets/js/main.js` đã được thiết lập để **không giả lập gửi thành công ảo**. Thay vào đó, hệ thống hướng dẫn người dùng gửi trực tiếp qua email.
  - Khi chủ dự án sẵn sàng backend (hoặc sử dụng dịch vụ miễn phí như [Formspree](https://formspree.io), [Web3Forms](https://web3forms.com), Google Form Webhook), hãy cập nhật thuộc tính `action="URL_ENDPOINT"` tại các biểu mẫu trong `contact.html`, `pricing.html`, `index.html`.
- [ ] **Hình ảnh đội ngũ sáng lập & nhân sự thực tế:**
  - Cập nhật ảnh đại diện và thông tin của Founder / Co-founder tại phần "Đội Ngũ Sáng Lập & Kỹ Sư AI" trong trang `about.html`.
- [ ] **Case Study & Khách hàng đối tác:**
  - Khi có các hợp đồng hợp tác thử nghiệm hoặc triển khai thực tế, bổ sung logo và lời chứng thực (testimonials) đã được khách hàng phê duyệt vào `index.html` và `about.html`.

---

## 📄 Bản Quyền & Giấy Phép

- Giao diện được phát triển dựa trên mẫu thiết kế mã nguồn mở **KA SaaS Landing Page** của [Kod Atölye](https://kodatolye.com.tr).
- Nội dung, cấu trúc giải pháp, bộ nhận diện thương hiệu và tài liệu bản ngữ tiếng Việt thuộc quyền sở hữu của **MN AI Technologies**.
- Mọi thắc mắc kỹ thuật hoặc đề xuất hợp tác, vui lòng gửi email về: [minz@mnaitechnologies.tech](mailto:minz@mnaitechnologies.tech).
