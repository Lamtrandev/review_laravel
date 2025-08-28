# review_laravel
Ôn tập làm lại một website laravel
Các bước thực hiện 
Bước 1: Tạo môi trường hoat động cho laravel
        - Cài đặt composer
        - Cài đặt xampp/wampserver/...
        - Tạo database trong phpmyadmin và liện kết database với source laravel
        - Tạo table default laravel
        - Tạo tài khoản admin ([php artisan tinker] và echo brcypte('mật khẩu'))
Bước 2: Cài đặt giao diện Đăng nhập
        - Tạo Logincontroller
                + code function index
        - Tạo Route giao điện đăng nhập
        - Layout Đăng nhập
                + Copy assets vào public tạo template/admin quản lý
                + Thay đổi link assets trong Layout
                + Chia layout thành nhiều file nhỏ
                + Liện kết các thành phần lại trong playout
Bước 3: Xử lý đăng nhập
        - Tạo Route chức năng đăng nhập
        - Thay đổi thông tin form đăng nhập
        - Vào Logincontroller viết hàm đăng nhập
                + Kiểm tra điều kiện đăng nhập
                + Kiểm tra thông tin đăng nhập
        - Viết code hiển thị thông báo lỗi trên layout đăng nhập
Bước 4: Cài đặt giao diện Admin (dashboard)
        - Tạo Route::middleware('auth') hàm kiểm tra các giao diện cần đăng nhập sử dụng
        - Tạo Route Giao diện admin (dashboard)
        - Tạo Maincontroller
                + Code hàm hiển thị dashboard
        - Xử lý Layout dashboard
                + Thay đổi link assets
                + Chia layout thành nhiều phần head,footer,sidebar,..
                + Tạo Layout main (Mẫu chứa các thành phần xuất hiện nhiều lần)
                + Tạo Layout dashboard gọi Layout main
                + Code content cho Layout dashboard
 Bước 5: Tạo Menu dashboard
        - Tạo các mục thành phần mới trên menu dựa trên các mẫu hiện tại
        - Xóa các mục thành phần không cần thiết
        - Thay đổi đường dẫn trên các mục mới
        - Tạo model, migration
        - Tạo table menus
                + Vào Migration Menu để thêm thuộc tính các trường
                + Chạy Lệnh migrate tạo table menus
        - Tạo Route nhóm các chức năng menu
                + Route tạo menu mới
                + Route hiển Thị menu
                + Route sửa menu mới
                + Route xóa menu mới
        - Tạo Menucontroller
                + CRUD (Thêm Đọc Sửa Xóa)
        - Cắt Layout Menu
                + Thêm Layout
                + Sửa Layout
                + Read Layout
        - Ngoài rà còn có một số chức năng sử đụng jquery như:
                + Tìm kiếm
                + Sắp Xếp

         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
         
