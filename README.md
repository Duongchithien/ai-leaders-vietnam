# AI Leaders Vietnam — Website

Website chính thức của **AI Leaders Vietnam** — AI Marketing Agency đầu tiên tại Việt Nam.

**Domain:** [https://aileaders.vn](https://aileaders.vn)

---

## Cấu trúc thư mục

```
ai-leaders-github/
├── index.html              # Trang chính (SPA entry point)
├── 404.html                # Fallback cho GitHub Pages SPA routing
├── robots.txt              # Cấu hình SEO cho search engines & AI bots
├── sitemap.xml             # Sitemap cho Google Search Console
├── README.md               # File hướng dẫn này
└── assets/
    ├── index-HAuoy4_2.css  # Toàn bộ CSS (Tailwind + custom styles)
    ├── index-BVlYbWqn.js   # Core React framework + routing
    ├── Home-BXCtk2RA.js    # Trang chủ
    ├── About-C1JK4G6Y.js   # Trang Về chúng tôi
    ├── Services-Be8L3d5b.js         # Trang Dịch vụ
    ├── CaseStudies-B-WhZbpB.js      # Trang Hành trình
    ├── AIAgencyVietnam-CIiOUhq9.js  # Trang AI Agency Vietnam (SEO)
    ├── AIGlossary-jxe9SoBr.js       # Trang Từ điển AI
    ├── Blog-D7cnHI2c.js             # Trang Blog
    ├── BlogPost-D_ms15In.js         # Trang bài viết chi tiết
    ├── Newsletter-B18VtdLr.js       # Trang Newsletter
    └── ... (các component chunks khác)
```

---

## Triển khai lên GitHub Pages

### Bước 1: Tạo repository trên GitHub

1. Truy cập [github.com/new](https://github.com/new)
2. Đặt tên repository (ví dụ: `ai-leaders-vietnam`)
3. Chọn **Public**
4. Nhấn **Create repository**

### Bước 2: Push code lên GitHub

```bash
cd ai-leaders-github
git init
git add .
git commit -m "Initial deploy: AI Leaders Vietnam website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/ai-leaders-vietnam.git
git push -u origin main
```

### Bước 3: Bật GitHub Pages

1. Vào **Settings** → **Pages**
2. Source: chọn **Deploy from a branch**
3. Branch: chọn **main** → folder **/ (root)**
4. Nhấn **Save**
5. Chờ 1-2 phút, website sẽ live tại: `https://YOUR_USERNAME.github.io/ai-leaders-vietnam/`

### Bước 4: Cấu hình Custom Domain (tùy chọn)

1. Trong **Settings** → **Pages** → **Custom domain**: nhập `aileaders.vn`
2. Nhấn **Save**
3. Cấu hình DNS tại nhà cung cấp domain:
   - **A Record** trỏ đến: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - **CNAME Record**: `www` trỏ đến `YOUR_USERNAME.github.io`
4. Bật **Enforce HTTPS**

---

## Chạy local để kiểm tra

```bash
# Cách 1: Python HTTP server
cd ai-leaders-github
python3 -m http.server 8080
# Mở http://localhost:8080

# Cách 2: Node.js (npx serve)
npx serve ai-leaders-github -p 8080
# Mở http://localhost:8080
```

---

## Lưu ý quan trọng

- **Hình ảnh:** Tất cả hình ảnh đã được host trên CDN CloudFront, không cần lưu local -> Đã chuyển sang github
- **SPA Routing:** File `404.html` đảm bảo routing hoạt động đúng trên GitHub Pages (React Router).
- **AI SEO:** Website đã được tối ưu cho Google AI Overview, ChatGPT, Perplexity với Schema Markup JSON-LD.
- **Google Search Console:** Đã tích hợp verification tag. Submit sitemap tại: `https://aileaders.vn/sitemap.xml`

---

## Công nghệ

- **Frontend:** React 19 + TypeScript
- **Styling:** Tailwind CSS 4 + shadcn/ui
- **Build:** Vite 6
- **SEO:** Schema.org JSON-LD, Open Graph, AI bot optimization

---

**AI Leaders Vietnam** — Lead with Vision. Amplify with Intelligence.
