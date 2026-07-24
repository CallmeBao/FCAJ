---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

- Xây dựng Backend và tích hợp Large Language Model (LLM)

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu AWS Lambda <br> - Xây dựng hàm xử lý yêu cầu từ người dùng | 13/07/2026 | 13/07/2026 | https://docs.aws.amazon.com/lambda/ |
| 3 | - Tìm hiểu Amazon API Gateway <br> - Xây dựng REST API | 14/07/2026 | 14/07/2026 | https://docs.aws.amazon.com/apigateway/ |
| 4 | - Tích hợp Amazon Bedrock với hệ thống RAG | 15/07/2026 | 15/07/2026 | https://docs.aws.amazon.com/bedrock/ |
| 5 | - Kết nối Retrieval với LLM <br> - Sinh câu trả lời dựa trên ngữ cảnh truy xuất | 16/07/2026 | 16/07/2026 | |
| 6 | - Kiểm thử API <br> - Ghi log bằng Amazon CloudWatch | 17/07/2026 | 17/07/2026 | https://docs.aws.amazon.com/cloudwatch/ |

### Kết quả đạt được tuần 6:

- Hiểu được kiến trúc Backend của hệ thống RAG trên AWS.

- Xây dựng thành công REST API bằng Amazon API Gateway và AWS Lambda.

- Hoàn thành việc tích hợp Amazon Bedrock vào hệ thống.

- Xây dựng luồng xử lý câu hỏi từ người dùng:
  - Tiếp nhận câu hỏi.
  - Thực hiện Retrieval.
  - Chuyển ngữ cảnh tới LLM.
  - Sinh câu trả lời.

- Kiểm thử API bằng Postman và xác nhận hệ thống trả về kết quả đúng.

- Thiết lập CloudWatch Logs để theo dõi quá trình xử lý và hỗ trợ gỡ lỗi.

- Hoàn thiện Backend cho chatbot tuyển sinh.