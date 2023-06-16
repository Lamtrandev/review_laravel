# review_laravel
Ôn tập làm lại một website laravel
Các bước thực hiện 
- Bước 1: tạo môi trường hoat động cho laravel
        + Cài đặt composer
        + Chạy lệnh composer create-project laravel/laravel review_laravel để tạo source laravel tên: review_laravel
        + Vào cd review_laravel chạy lệnh php artisan serve để tạo server 
        + Vào xampp tạo database tên: review_laravel kiểu utf8mb4_general_ci
        + Vào .evn thay đổi DB_DATABASE=review_laravel
        + Vào cd review_laravel chạy lệnh php artisan migrate tạo các table default
        + Vào table users tạo 1 tài khoản admin
          ++ Nhập thông tin admin
          ++ Vào cd review_laravel chạy lệnh php artisan tinker tạo ra mộ trường php chạy lệnh echo brcypte('mật khẩu');
          ++ Lấy shortcode nhập vào trường password
- Bước 2: Tạo giao diện đăng nhập admin
       + tạo Logincontroller
       + tạo Route giao điện đăng nhập
       + Cắt playout login
         ++ tạo view quản lý admin chứa các giao diện đăng nhập
         ++ Copy source cho giao diện đăng nhập
         ++ Cắt lauout ra nhiều phần để dễ quản lý
         ++ Vào public tạo template tạo admin để quản lý các file assets 
         ++ Thay đổi dường dẫn img js css trong layout login
