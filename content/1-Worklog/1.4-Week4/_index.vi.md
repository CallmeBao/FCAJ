---
title: "Worklog Tuần 4"
date: 2026-07-04
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:
- Thống nhất ý tưởng và chốt đề tài xây dựng project
- Tìm hiểu Amazon VPC, Subnet, Security Group
- Tìm hiểu Amazon ECS và mô hình triển khai Fargate

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2   | - Tìm kiếm và chốt đề tài cho dự án cuối khóa | 29/06/2026 | 29/06/2026 | |
| 3   | - Xác định các chức năng chính, phân tích người dùng và thiết kế sơ bộ kiến trúc hệ thống | 30/06/2026 | 30/06/2026 | |
| 4   | - Nghiên cứu Amazon VPC: Public/Private Subnet, NAT Gateway, Internet Gateway, Security Group | 1/07/2026 | 1/07/2026 | <https://docs.aws.amazon.com/vpc/> |
| 5   | - Tìm hiểu Amazon ECS: Cluster, Service, Task Definition, Fargate Launch Type | 2/07/2026 | 2/07/2026 | <https://docs.aws.amazon.com/ecs/> |
| 6   | - **Thực hành:** Tạo VPC với Public và Private Subnet, cấu hình Security Group, khởi tạo ECS Cluster Fargate | 3/07/2026 | 3/07/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:

- Hoàn thành việc khảo sát và chốt đề tài cho dự án: Xây dựng một nền tảng web (dạng forum/mạng xã hội học tập) backend bằng **NestJS**, triển khai trên **Amazon ECS Fargate**.

- Xác định được bài toán và phạm vi của dự án:
  - Đối tượng sử dụng là sinh viên, học viên và giảng viên có nhu cầu chia sẻ tài liệu học tập.
  - Mục tiêu xây dựng nền tảng web có khả năng mở rộng, bảo mật cao, sử dụng kiến trúc container trên AWS.
  - Xác định các chức năng chính: đăng nhập/đăng ký người dùng, đăng tải tài liệu lên S3, tìm kiếm, quản lý phiên bằng Redis.

- Hiểu được vai trò của **Amazon VPC** trong việc cô lập và bảo vệ tài nguyên AWS:
  - **Public Subnet**: Đặt ALB và NAT Gateway, tiếp nhận traffic từ bên ngoài.
  - **Private Application Subnet**: Đặt ECS Tasks (NestJS), không tiếp xúc trực tiếp Internet.
  - **Private DB Subnet**: Đặt RDS PostgreSQL, chỉ cho phép kết nối từ Application Subnet.

- Nắm được các khái niệm cơ bản của **Amazon ECS Fargate**:
  - Cluster, Service, Task Definition, Container Definition.
  - Fargate Launch Type: không cần quản lý EC2 instance.
  - Task Role và IAM Task Role để phân quyền cho container.

- Thực hành tạo VPC từ đầu:
  - Tạo VPC với CIDR block phù hợp.
  - Tạo Public Subnet và Private Subnet ở Availability Zone A.
  - Gắn Internet Gateway cho Public Subnet, NAT Gateway cho Private Subnet.
  - Cấu hình Security Group phân tách theo tầng: ALB SG → ECS SG → DB SG.

- Khởi tạo ECS Cluster Fargate và thực hành chạy Task thử nghiệm.

- Đánh giá được tính khả thi của dự án và định hướng kiến trúc **Container-based trên AWS ECS Fargate**, kết hợp với CI/CD bằng GitHub Actions để tự động hóa quy trình build và deploy.