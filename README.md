Dự án: SportMatch
SportMatch là một ứng dụng di động giúp những người yêu thích thể thao dễ dàng tìm thấy nhau. Bạn có thể bật bản đồ để quét xem xung quanh mình có ai đang tìm người đá bóng, đánh cầu lông hay bóng chuyền không để "nhảy vào" chốt kèo và đi chơi ngay.

1. Các tính năng chính
Đăng nhập nhanh: Xác thực qua số điện thoại bằng mã OTP (Firebase).
Tìm kèo quanh đây: Xem bản đồ để biết các nhóm hoặc cá nhân nào đang thiếu người ở gần vị trí của bạn(dự kiến).
Chat trực tiếp: Nhắn tin ngay trên ứng dụng để trao đổi về thời gian, địa điểm và trình độ chơi.
Quản lý hồ sơ: Lưu trữ thông tin cá nhân và số điện thoại liên lạc.

2. Công nghệ sử dụng
- Frontend
Ngôn ngữ: Kotlin.
Giao diện: Jetpack Compose (Modern UI).
Bản đồ: Google Maps SDK.
Kết nối mạng: Retrofit & OkHttp.
Xác thực: Firebase Auth (OTP).

- Backend
Ngôn ngữ: C# (.NET 9).
Cơ sở dữ liệu: MySQL.
Công nghệ: ASP.NET Core API, Entity Framework Core.
Xử lý bản đồ: NetTopologySuite (để tính khoảng cách người chơi).

3. Cấu trúc thư mục
Android Project
com.example.sportmatch/
├── data/               # Xử lý gọi API và định nghĩa dữ liệu
├── ui/                 # Giao diện (Màn hình Login, OTP, Bản đồ, Chat)
├── navigation/         # Quản lý chuyển màn hình
└── MainActivity.kt     # Điểm khởi chạy ứng dụng

Backend Project (.NET)
SportMatchAPI/
├── Controllers/        # Nơi nhận request (Auth, Location, Chat)
├── Data/               # Kết nối Cơ sở dữ liệu (DbContext)
├── Models/             # Các bảng dữ liệu (User, Match)
├── DTO/                # Các mẫu dữ liệu gửi nhận giữa App và API
└── Program.cs          # Cấu hình khởi tạo hệ thống
4. Nhóm phát triển
Đặng Phong Hào
Bùi Tấn Khang
Võ Thị Kiều Trang
