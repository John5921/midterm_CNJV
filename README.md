# MIDTERM
- MSSV: 51900428  
- Tên: Cao Thành Tài
- Môn: Thực hành công nghệ Java

# Tài khoản và database có trong dự án
- Tài khoản admin:
    + username: admin
    + password: admin
- Tài khoản người dùng 1:
    + username: tai
    + password: 123456
- Tài khoản người dùng 2:
    + username: test
    + password: test

- Database sẽ nằm trong folder database/
- Đường dẫn đến database diagram: https://drive.google.com/file/d/1BHmpFfSV-8wW_D2YENsUapcTtCOqBP02/view?usp=sharing

# API có trong dự án
- GET: http://localhost:8080/
    + Hiển thị 6 sản phẩm mới nhất
- GET: http://localhost:8080/brand/*
    + Hiển thị các sản phẩm có cùng thương hiệu
- GET: http://localhost:8080/category/*
    + Hiển thị các sản phẩm có cùng loại sản phẩm
- GET: http://localhost:8080/product
    + Hiển thị tất cả các sản phẩm
- GET: http://localhost:8080/product/ *
    + Hiển thị chi tiết sản phẩm, cùng với đó là 3 sản phẩm có cùng thương hiệu
- GET: http://localhost:8080/card/checkout
    + Trang kiểm tra giỏ hàng trước khi thanh toán
- GET: http://localhost:8080/card/pay
    + Trang thanh toán các sản phẩm có trong giỏ hàng và chuyển hướng người dùng về trang chủ
- GET: http://localhost:8080/order
    + Hiển thị các đơn hàng mà khách hàng đã đặt
- GET: http://localhost:8080/login
    + Trang đăng nhập
- GET: http://localhost:8080/logout
    + Trang đăng xuất
- GET: http://localhost:8080/admin
    + Trang quản lý các sản phẩm có trong cửa hàng (chỉ dành cho người dùng admin)
- POST: http://localhost:8080/admin/add
    + API dùng để thêm sản phẩm vào cửa hàng
- POST: http://localhost:8080/admin/ *
    + API dùng để cập nhập sản phẩm trong cửa hàng
- POST: http://localhost:8080/admin/delete/ *
    + API dùng để xóa sản phẩm trong cửa hàng

# Các công nghệ sử dụng trong dự án
- spring-boot-starter-security
    + Công nghệ này được dùng trong dự án để phân quyền các trang xem người dùng có được truy cập hay không và cũng như là xử lý xem người dùng có đăng nhập chưa. Dữ liệu thông tin người dùng sẽ được lưu trong RAM của hệ thống. Các dự liệu lưu trong hệ thống như mật khẩu sẽ được mã hóa bằng thuật toán Bcrypt
- spring-boot-devtools
    + Công nghệ này dùng để tự động cập nhập mỗi khi tập tin thay đổi
- spring-boot-starter-data-jpa
    + Dùng để giao tiếp với database một cách an toàn, trách các cuộc tấn công nhắm vào các lỗi database
- spring-boot-starter-thymeleaf
    + Dùng để xem đâu là tập tin html sẽ trả về cho người dùng cũng như là hỗ trợ viết code logic trong tập tin html
- lombok
    + Sử dụng các annotation có trong thư viện để rút ngắn đoạn code
- commons-io
    + Dùng để xử lý các tập tin hình ảnh tải lên

# Config dự án
- Thông tin cấu hình dự án:
    + Dự án chạy trên cổng: 8080.
    + src/main/resources/static/ : là nơi sẽ chứa các tập tin liên quan đến js, css, images.
    + src/main/resources/templates/ : là nơi chứa các tập tin html hiển thị cho người dùng.
    + uploads: Nơi chứa các tập tin hình ảnh của admin tải lên.
- Thông tin cấu hình cơ sở dữ liệu
    + Cổng database: 3306
    + Tên database: midtern
    + tài khoản database: root
    + mật khẩu database:

