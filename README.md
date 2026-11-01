# Bài thực hành số 7 - Microservices .NET Core (Đại lý bảo hiểm)

- Họ và tên: Ngô Hồng Phúc
- MSSV: 2424802010413
- Lớp: D24CNTT05
- GitHub username: phuc123-hn

## Nội dung Lab 7

- Task 1: cài đặt thư viện Marten 7.19.1 (PostgreSQL làm document database) cho PaymentService.
- Task 2: bổ sung code PaymentService, PaymentService.Api, PaymentService.Test.
- Task 3: bổ sung code ProductService, ProductService.Api, ProductService.Test.

## Ghi chú

- Solution build thành công, 0 lỗi (dotnet build). PaymentService.Test pass 6/6, ProductService.Test pass 14/14.
- PaymentService dùng Marten (thư mục DataAccess/Marten); ProductService dùng Entity Framework và Steeltoe Eureka theo code mẫu.
- PaymentService tham chiếu PolicyService.Api, nên bổ sung tối thiểu PolicyService.Api/Events/PolicyCreated.cs (Lab 6) và PolicyService.Api/Events/PolicyTerminated.cs để solution biên dịch được.
- Cảnh báo NU1901/NU1903 về gói Steeltoe.Discovery.Eureka 3.2.7 là cảnh báo bảo mật của gói theo yêu cầu đề, không ảnh hưởng việc build.
