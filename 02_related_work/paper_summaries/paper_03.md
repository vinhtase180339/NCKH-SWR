# Paper 03 Summary

## Citation

- **Title:** Enhancing Engineering Education through LLM-Driven Adaptive Quiz Generation: A RAG-Based Approach
- **Year:** 2024
- **Venue:** FIE 2024 (Frontiers in Education)
- **Source:** IEEE
- **DOI:** 10.1109/FIE61694.2024.10893146

---

## Problem

Trong giáo dục kỹ thuật, việc tạo quiz thủ công không đủ đáp ứng nhu cầu luyện tập đa dạng và liên tục của sinh viên. Các hệ thống tự động trước đây thiếu khả năng truy xuất đúng nội dung từ tài liệu môn học, dẫn đến câu hỏi không bám sát syllabus.

---

## Method

Kết hợp RAG (Retrieval-Augmented Generation) với LLM để sinh quiz thích ứng trong giáo dục kỹ thuật:

1. Tài liệu môn học (slide, textbook) được chunk và embedding vào vector database.
2. Khi cần sinh quiz, hệ thống truy xuất các đoạn tài liệu liên quan nhất.
3. LLM nhận đoạn tài liệu đã truy xuất làm context để sinh câu hỏi phù hợp.
4. Quiz được tích hợp vào luồng học tập của sinh viên.

---

## Dataset

Slide bài giảng và giáo trình các môn kỹ thuật tại trường đại học. Dữ liệu được chunk theo đoạn văn và embedding bằng mô hình sentence transformer.

---

## Evaluation

- Quiz relevance (đánh giá bởi giảng viên)
- Expert evaluation (thang điểm Likert 5 mức)
- So sánh với LLM-only (không có RAG)

---

## Results

Hệ thống RAG + LLM tạo ra câu hỏi bám sát nội dung môn học tốt hơn đáng kể so với LLM-only. Giảng viên đánh giá câu hỏi có tính chính xác và phù hợp cao hơn. Thời gian tạo quiz giảm mạnh so với thủ công.

---

## Limitations

- Chỉ tập trung vào quiz generation, chưa có phản hồi cá nhân hóa.
- Chưa theo dõi tiến độ học tập hay CLO achievement của sinh viên.
- Chưa có user study với sinh viên thực tế làm quiz.
- Vector database cần cập nhật thủ công khi tài liệu môn học thay đổi.

---

## Relevance to Our Topic

**Mức độ liên quan: Rất cao**

Đây là bài báo kỹ thuật gần nhất với hướng nghiên cứu của nhóm. Nhóm sử dụng cùng kiến trúc RAG + LLM, nhưng mở rộng thêm: CLO-aware quiz generation, personalized feedback, learning progress tracking, và tích hợp đầy đủ vào LMS cho cả giảng viên và sinh viên.

---

## Possible Improvement

- Thêm CLO mapping để câu hỏi được gắn với từng mục tiêu học tập cụ thể.
- Tích hợp personalized feedback sau khi sinh viên nộp bài quiz.
- Thêm dashboard theo dõi CLO achievement cho giảng viên.
- Thực hiện user study với sinh viên để đánh giá trải nghiệm học tập thực tế.
