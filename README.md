# SpendSmart - Expense Tracker 💰

SpendSmart là một ứng dụng web quản lý chi tiêu cá nhân hiện đại, trực quan, giúp bạn dễ dàng theo dõi thu nhập, chi phí, lập ngân sách và đặt mục tiêu tài chính cá nhân. Dự án được xây dựng bằng **Vanilla JavaScript** kết hợp lưu trữ dữ liệu cục bộ (**LocalStorage**) và đi kèm hệ thống kiểm thử toàn diện bằng **Vitest** và **Playwright**.

---

## 🚀 Tính năng chính

- **Dashboard:** Tổng quan tình hình tài chính, số dư, thu chi qua biểu đồ và các chỉ số nhanh.
- **Quản lý giao dịch (Transactions):** Thêm, sửa, xóa, tìm kiếm và lọc giao dịch theo danh mục/loại (Thu/Chi).
- **Ngân sách (Budgets):** Thiết lập và theo dõi hạn mức chi tiêu theo từng danh mục kèm phần trăm cảnh báo.
- **Mục tiêu (Goals):** Tạo và nạp tiền vào các mục tiêu tiết kiệm cá nhân.
- **Subscriptions:** Quản lý các khoản thanh toán định kỳ.
- **Đa tiền tệ & Đa ngôn ngữ:** Hỗ trợ chuyển đổi tiền tệ (USD, EUR, VND,...) và ngôn ngữ linh hoạt.
- **Lưu trữ dữ liệu:** Đồng bộ và duy trì dữ liệu an toàn ngay trên trình duyệt thông qua `LocalStorage`.

---

## 🛠️ Công nghệ sử dụng

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Unit Testing:** [Vitest](https://vitest.dev/) + JSDOM
- **E2E Testing:** [Playwright](https://playwright.dev/)
- **Quản lý gói:** npm

---

## 📂 Cấu trúc thư mục

```text
├── index.html              # Giao diện chính của ứng dụng
├── script.js               # Logic xử lý frontend & quản lý State/LocalStorage
├── styles.css              # Tệp định dạng giao diện (CSS)
├── tests/
│   ├── e2e/                # E2E Test tự động
│   │   └── spendsmart.spec.js
│   └── unit/               # Unit Test hàm xử lý
│       ├── loader.js
│       ├── script.test.js
│       └── setup.js
├── package.json            # Cấu hình dự án và dependencies
├── vitest.config.js        # Cấu hình Vitest
└── playwright.config.js    # Cấu hình Playwright
