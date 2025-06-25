# 🛍️ Website Bán Hàng Thời Trang sử dụng Laravel Framework 10

## 🔗 Link Repo 

[https://github.com/mcuong12/webncaoo](https://github.com/mcuong12/webncaoo)

---

## 👤 Thông tin sinh viên

- **Họ và tên:** Nguyễn Mạnh Cường  
- **Mã sinh viên:** 23010271
- **Lớp:** K17-CNTT3  
- **Môn học:** Thiết kế Web nâng cao (TH3) 
---

## 📝 Giới thiệu dự án
Website Bán Hàng Thời Trang là một ứng dụng web được xây dựng bằng Laravel Framework 10, nhằm mục đích mô phỏng một hệ thống bán hàng trực tuyến hiện đại. Ứng dụng hỗ trợ người dùng có thể đăng ký tài khoản, đăng nhập, duyệt sản phẩm, thêm vào giỏ hàng, thanh toán đơn hàng và theo dõi lịch sử mua sắm. Đồng thời, quản trị viên có thể quản lý toàn bộ hệ thống như sản phẩm, danh mục, người dùng và đơn hàng.

Dự án áp dụng kiến trúc MVC (Model - View - Controller), sử dụng Laravel Breeze cho chức năng xác thực, và tích hợp đầy đủ các tính năng bảo mật như CSRF, XSS, xác thực, phân quyền, và kiểm tra đầu vào (validation). Toàn bộ dữ liệu được lưu trữ và thao tác thông qua MySQL sử dụng Eloquent ORM, đồng thời hỗ trợ kết nối với cơ sở dữ liệu trên nền tảng cloud như Aiven hoặc Railway.

Website có giao diện thân thiện với người dùng, được thiết kế bằng Blade Template kết hợp Tailwind CSS/Bootstrap, đảm bảo trải nghiệm người dùng mượt mà và dễ sử dụng 
### 1. Sử dụng framework Laravel xây dựng ứng dụng theo yêu cầu

- Website sử dụng **Laravel 10**, phát triển theo mô hình MVC.
- Dùng **Laravel Breeze** để xác thực đăng ký/đăng nhập.
- Giao diện được thiết kế bằng Blade và Bootstrap/Tailwind.

---
## 🛠️ Công Nghệ sử dụng
Dự án sử dụng các công nghệ sau:
- **Laravel Framework**
- **PHP 8.x**
- **MySQL - PhpAdmin**
- **DataTables với jQuery**
- **HTML, CSS, JavaScript**
## 📍 Sơ đồ hệ thống
### Biểu đồ usecase tổng quát ( người dùng và quản trị)
![Image](https://github.com/user-attachments/assets/0f6aa534-10d8-4fde-b222-6673fe0ebcbb)
### Biểu đồ quan hệ giữa các bảng trong cơ sở dữ liệu
![Image](https://github.com/user-attachments/assets/735a23d3-0f33-4871-8b31-7cba7ee89804)

## Một số hình ảnh giao diện chính
- **Giao diện đăng nhập**
![Image](https://github.com/user-attachments/assets/9f37d5df-ace5-4b01-922e-14c1b2cd7e33)

- **Đăng nhập/Đăng kí**
 ![Log](https://github.com/user-attachments/assets/27782b7c-5835-4cea-a44e-47c0f27da68e)

- **Giao diện admin**
  ![admin](https://github.com/user-attachments/assets/00f70d1f-43d2-4538-b481-9024e3f68ebe)

## 🔐 Bảo mật
- **Sử dụng @CSRF Token:**
  
![Image](https://github.com/user-attachments/assets/b77d7945-f8ee-43a2-89ac-472634c8ef30)

- **Chống XSS hiển thị dữ liệu ra giao diện.:**

![Image](https://github.com/user-attachments/assets/620161b2-e72e-44b0-9aa0-e6c2cabae0da)
  
- **Session & Cookies:**
  
  
![Image](https://github.com/user-attachments/assets/577d2ad9-8209-4934-be43-a416deeb5ffe)

- **Truy vấn an toàn với Eloquent ORM (chống SQL Injection):**

  ![Image](https://github.com/user-attachments/assets/8a748b6e-d188-4556-acdc-c260abdff447)
  

## 🚀 Hướng dẫn cài đặt

```bash
git clone https://github.com/your-username/library-management.git
cd library-management
composer install
cp .env.example .env
php artisan key:generate

# Cấu hình DB trong file .env
# DB_CONNECTION=mysql
# DB_HOST=xxx
# DB_PORT=3306
# DB_DATABASE=your_db
# DB_USERNAME=your_user
# DB_PASSWORD=your_pass

php artisan migrate
npm install && npm run dev
php artisan serve
