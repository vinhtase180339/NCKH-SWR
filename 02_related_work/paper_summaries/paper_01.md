# Paper 01 Summary

## Citation

- **Title:** Exploring the Integration of Virtual Assistant Using Large Language Models in Learning Management System: Enhancing Educational Accessibility and Efficiency
- **Year:** 2024
- **Venue:** ICITSI 2024
- **Source:** IEEE
- **DOI:** 10.1109/ICITSI65188.2024.10929366

---

## Problem

Các hệ thống LMS truyền thống thiếu khả năng hỗ trợ sinh viên tự động và theo thời gian thực. Sinh viên thường phải chờ đợi phản hồi từ giảng viên, gây ảnh hưởng đến trải nghiệm học tập và khả năng tiếp cận tài nguyên giáo dục.

---

## Method

Tích hợp một virtual assistant dựa trên LLM vào hệ thống LMS hiện có. Assistant này có khả năng trả lời câu hỏi của sinh viên, hướng dẫn tìm tài liệu, và hỗ trợ điều hướng trong hệ thống học tập.

---

## Dataset

Dữ liệu tương tác từ hệ thống LMS trong môi trường thực tế, bao gồm lịch sử hỏi đáp và log hoạt động của sinh viên.

---

## Evaluation

- User satisfaction survey
- Accessibility score
- Response accuracy (manual review)

---

## Results

Hệ thống cải thiện đáng kể khả năng tiếp cận thông tin cho sinh viên và giảm thời gian chờ phản hồi. Điểm hài lòng của người dùng tăng so với hệ thống không có AI assistant.

---

## Limitations

- Đánh giá quy mô nhỏ, chỉ thực hiện trong một khóa học.
- Virtual assistant chưa được gắn với CLO hoặc syllabus cụ thể.
- Không có so sánh baseline định lượng rõ ràng.

---

## Relevance to Our Topic

**Mức độ liên quan: Cao**

Bài báo cung cấp bằng chứng thực tiễn về khả năng tích hợp LLM vào LMS. Hệ thống của nhóm mở rộng hướng này bằng cách thêm RAG, quiz generation, và CLO-aware feedback thay vì chỉ dừng ở virtual assistant đơn giản.

---

## Possible Improvement

- Thêm CLO-awareness để assistant trả lời đúng với mục tiêu học tập từng bài.
- Kết hợp RAG để truy xuất nội dung từ syllabus và slide môn học.
- Mở rộng đánh giá sang nhiều môn học và nhiều nhóm sinh viên.
