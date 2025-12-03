⚙ CÀI ĐẶT DỰ ÁN
Bước 1: Copy dự án vào htdocs
C:/xampp/htdocs/quanly
Bước 2: Tạo database
CREATE DATABASE phongtro;
Import file SQL.
Bước 3: Chỉnh config.php
$pdo = new PDO("mysql:host=localhost;dbname=phongtro;charset=utf8","root","");

Bước 4: Truy cập
Chủ trọ:
http://localhost/quanly/admin/login.php


Người thuê:
http://localhost/quanly/tenant/login.php

🔐 TÀI KHOẢN MẶC ĐỊNH
Admin
user: admin
pass: admin123

Tenant
Đăng nhập bằng:
→ Số điện thoại hoặc CCCD
→ Mật khẩu: số điện thoại


Cấu trúc module
/quanly
│
├── admin
│   ├── index.php
│   ├── login.php
│   ├── logout.php
│   ├── header.php
│   ├── footer.php
│   ├── rooms.php
│   ├── tenants.php
│   ├── contracts.php
│   ├── bills.php
│   ├── payments.php
│   ├── maintenance_requests.php
│  
│
├── tenant
│   ├── index.php
│   ├── login.php
│   ├── logout.php
│   ├── header.php
│   ├── footer.php
│   ├── view-bills.php
│   ├── view-room.php
│   ├── maintenance.php
│   
│
├── assets
│   ├── css
│   ├── img
│   └── js
│
└── config.php
