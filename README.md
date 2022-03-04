# Chạy composer và npm để cài đặt các gói cần thiết trong dự án
composer install
npm install

# Tạo file cấu hình env
cp .env.example .env

# Cập nhật file env cấu hình database
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=

# Tạo ra key cho dự án
php artisan key:generate

# Tạo ra các bảng và dữ liệu mẫu cho database
php artisan migrate
php artisan db:seed

# Storage:link
php artisan storage:link

# Cho phép quyền ghi cho thư mục
chmod -R 777 storage/ bootstrap/cache/
