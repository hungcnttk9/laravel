# Cài đặt các gói cần thiết trong dự án
composer install<br>
npm install

# Tạo file cấu hình env
cp .env.example .env

# Cập nhật file env cấu hình database
DB_CONNECTION=mysql<br>
DB_HOST=127.0.0.1<br>
DB_PORT=3306<br>
DB_DATABASE=laravel<br>
DB_USERNAME=root<br>
DB_PASSWORD=

# Tạo ra key cho dự án
php artisan key:generate

# Tạo ra các bảng và dữ liệu mẫu cho database
php artisan migrate<br>
php artisan db:seed

# Storage:link
php artisan storage:link

# Cho phép quyền ghi cho thư mục
chmod -R 777 storage/ bootstrap/cache/
