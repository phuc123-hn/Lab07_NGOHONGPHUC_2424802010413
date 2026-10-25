# Bài thực hành số 6 - Microservices .NET Core (Đại lý bảo hiểm)

- Họ và tên: Ngô Hồng Phúc
- MSSV: 2424802010413
- Lớp: D24CNTT05
- GitHub username: phuc123-hn

## Nội dung Lab 6

- Task 1: cấu hình API Gateway (AgentPortalApiGateway) với Ocelot, Ocelot.Provider.Eureka, Ocelot.Cache.CacheManager; ocelot.json và cấu hình Eureka trong appsettings.json.
- Task 2: bổ sung code AuthService.
- Task 3: bổ sung code ChatService và ChatService.Api.
- Task 4: bổ sung code DashboardService, DashboardService.Api và DashboardService.Test.

## Ghi chú

- Solution build thành công, 0 lỗi (dotnet build).
- Dự án chạy .NET 8 nên dùng Ocelot 23.3.3 (ocelot.json dùng "Routes" thay cho "ReRoutes" của bản cũ) thay vì các phiên bản của .NET Core 2.1 trong đề.
- Project PolicyService.Api trong solution chưa có sự kiện PolicyCreated mà DashboardService và ChatService sử dụng, nên em bổ sung tối thiểu file PolicyService.Api/Events/PolicyCreated.cs (kèm gói MediatR) để solution biên dịch được.
- Các bài trước: Eureka Server chạy bằng Docker ở cổng 8761, PricingService chạy ở cổng 5050 (cổng 5040 bị tiến trình hệ thống svchost chiếm).
