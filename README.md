# HỆ THỐNG THƯ VIỆN SỐ TÍCH HỢP MÃ QR  
**Mã sinh viên:** 110121224  
**Lớp:** DA21TTC  
**Sinh viên thực hiện:** Nguyễn Hoàng Thương  

---

## Giới thiệu đồ án

Đồ án **"Hệ thống thư viện số tích hợp mã QR cho Trung tâm Văn hóa Miền Tây"** được phát triển nhằm hỗ trợ **Trung tâm Văn hóa Miền Tây** trong công tác quản lý sách và nâng cao trải nghiệm bạn đọc.

### Mục tiêu:
- Xây dựng hệ thống thư viện số trực tuyến.
- Tích hợp mã QR để quản lý sách và hỗ trợ quá trình mượn – trả dễ dàng.
- Tự động hóa thống kê, nhắc hạn trả sách, xử lý vi phạm.
- Gợi ý sách phù hợp và tích hợp chatbot hỗ trợ người dùng.

---

## Kiến trúc hệ thống

- Sử dụng mô hình **MVC (Model - View - Controller)** với **PHP Framework CodeIgniter 4**.
- Phân tách rõ ràng giữa giao diện, xử lý nghiệp vụ và truy xuất dữ liệu.
- Giao diện web thân thiện, dễ sử dụng cho người quản trị và người dùng.

---

## Công nghệ & phần mềm sử dụng

| Công nghệ / Phần mềm | Mô tả |
|----------------------|-------|
| **PHP (>= 8.1)**     | Ngôn ngữ lập trình backend |
| **MySQL**            | Hệ quản trị cơ sở dữ liệu |
| **CodeIgniter 4**    | PHP Framework MVC |
| **Composer**         | Trình quản lý thư viện PHP |
| **XAMPP**            | Môi trường phát triển web local |
| **Trình duyệt**      | Chrome, Edge, Firefox,... |

---

## Hướng dẫn cài đặt & triển khai

### Bước 1: Cài đặt môi trường
- Tải và cài đặt [XAMPP](https://www.apachefriends.org/index.html) (chọn bản hỗ trợ PHP 8.1 trở lên).

### Bước 2: Chuẩn bị mã nguồn & CSDL
- Clone hoặc tải mã nguồn từ repository này.
- Truy cập `phpMyAdmin`, tạo cơ sở dữ liệu với tên `qlthuvien`.
- Import file `qlthuvien.sql` có trong thư mục `database`.

### Bước 3: Cấu hình kết nối cơ sở dữ liệu
Mở file `app/Config/Database.php` và thiết lập:

public array $default = [
    'DSN'      => '',
    
    'hostname' => 'localhost',
    
    'username' => 'root',
    
    'password' => '',
    
    'database' => 'qlthuvien',
    
    'DBDriver' => 'MySQLi',
    
    'DBPrefix' => '',
];
### Bước 4: Chạy chương trình
Mở XAMPP, bật Apache và MySQL.

Đảm bảo thư mục mã nguồn đã được đặt trong thư mục htdocs (ví dụ: C:\xampp\htdocs\thuviensoQR).

Mở trình duyệt và truy cập địa chỉ: http://localhost/thuviensoQR

⚠️ Lưu ý:
Thay thuviensoQR bằng tên thư mục mã nguồn bạn đã lưu trong htdocs. Nếu có thiết lập baseURL trong app/Config/App.php, hãy đảm bảo nó đúng với đường dẫn localhost.


