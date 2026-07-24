---
title: "Worklog Tuần 5"
date: 2026-7-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---



### Mục tiêu tuần 5:

* Xây dựng RAG pipeline
### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Tiền xử lý dữ liệu <br> - Chuyển đổi từ pdf sang dạng văn bản có thể xử lý được                                                                                                           | 6/07/2026   | 6/07/2026      |
| 3   | - Chunking: Chia nhỏ tập dữ liệu                                                                                                                                                            | 7/07/2026   | 7/07/2026      | |
| 4   | - Chuyển đổi từng đoạn văn bản thành vector số <br> - Chuẩn bị dữ liệu phục vụ cho quá trình tìm kiếm ngữ nghĩa                                                                             | 8/07/2026   | 8/07/2026      | |
| 5-6 | - Thiết kế quy trình truy xuất tài liệu dựa trên câu hỏi của người dùng <br> - Chuyển câu hỏi thành embedding và tìm kiếm các đoạn văn bản liên quan trong Vector Database <br>             | 9/07/2026   | 10/07/2026      | |                                                                 | 15/07/2026   | 15/07/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 5:

- Hoàn thành việc thu thập và tiền xử lý các tài liệu tuyển sinh từ các trường thuộc Đại học Quốc gia TP.HCM.

- Chuyển đổi thành công các tài liệu PDF sang dạng văn bản có thể xử lý phục vụ cho hệ thống RAG.
- Hiểu được vai trò của bước **Chunking** trong hệ thống Retrieval-Augmented Generation (RAG).
- Thực hiện chia nhỏ tài liệu thành các đoạn văn bản (Chunks) với kích thước phù hợp nhằm đảm bảo khả năng lưu giữ ngữ cảnh và tối ưu hiệu quả truy xuất.
- Hiểu được nguyên lý hoạt động của **Embedding**, chuyển đổi văn bản thành các vector số để biểu diễn ngữ nghĩa.
- Xây dựng pipeline tạo Embedding cho toàn bộ tập tài liệu tuyển sinh.
- Tìm hiểu cơ chế lưu trữ Embedding trong Vector Database và vai trò của Vector Database trong hệ thống RAG.

- Hiểu được quy trình truy xuất thông tin (Retrieval), bao gồm:
  - Chuyển đổi câu hỏi của người dùng thành Embedding.
  - Thực hiện tìm kiếm ngữ nghĩa (Semantic Search).
  - Truy xuất các đoạn tài liệu có độ tương đồng cao nhất.

- Hoàn thiện pipeline xử lý dữ liệu cho hệ thống RAG theo quy trình:
- Chuẩn bị dữ liệu và pipeline phục vụ cho việc tích hợp Large Language Model (LLM) ở giai đoạn tiếp theo.