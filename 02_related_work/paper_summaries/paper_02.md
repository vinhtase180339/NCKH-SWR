# Paper 02 Summary

## Citation

- **Title:** LLM-Based Quiz Generation for Assessments in Learning Management System
- **Year:** 2025
- **Venue:** ICC-ROBINS 2025
- **Source:** IEEE
- **DOI:** 10.1109/ICC-ROBINS64345.2025.11086273

---

## Problem

Việc tạo câu hỏi kiểm tra (quiz) thủ công trong LMS tốn nhiều thời gian của giảng viên và khó đảm bảo tính đa dạng, phù hợp với nội dung bài học. Các hệ thống quiz tự động trước đây dựa trên rule-based hoặc template đơn giản, chưa tận dụng được khả năng sinh ngôn ngữ của LLM.

---

## Method

Đề xuất pipeline sử dụng LLM để tự động sinh câu hỏi quiz từ nội dung khóa học (slide, textbook). Pipeline bao gồm:

1. Trích xuất nội dung từ tài liệu môn học.
2. Đưa nội dung vào LLM kèm prompt hướng dẫn sinh câu hỏi.
3. Lọc và định dạng câu hỏi đầu ra theo chuẩn LMS.
4. Tích hợp câu hỏi vào hệ thống LMS để sinh viên làm bài.

---

## Dataset

Tài liệu khóa học thực tế bao gồm slide bài giảng và giáo trình môn học. Không sử dụng dataset benchmark chuẩn hóa.

---

## Evaluation

- Quiz quality (đánh giá bởi chuyên gia)
- Content accuracy
- Expert rating (thang điểm Likert)

---

## Results

LLM tạo ra câu hỏi có chất lượng tốt, phù hợp với nội dung tài liệu. Chuyên gia đánh giá cao tính rõ ràng và độ chính xác của câu hỏi. Thời gian tạo quiz giảm đáng kể so với làm thủ công.

---

## Limitations

- Chưa có cơ chế gắn câu hỏi với CLO cụ thể.
- Không có cá nhân hóa theo năng lực từng sinh viên.
- Chưa đánh giá trên nhiều môn học khác nhau.
- Không có baseline so sánh định lượng (TF-IDF, rule-based).

---

## Relevance to Our Topic

**Mức độ liên quan: Cao**

Đây là bài báo gần nhất với chức năng quiz generation của hệ thống nhóm. Tuy nhiên, hệ thống của nhóm mở rộng thêm CLO-awareness (câu hỏi được gắn với từng CLO), cá nhân hóa theo năng lực sinh viên, và tích hợp RAG để đảm bảo câu hỏi bám sát syllabus.

---

## Possible Improvement

- Thêm CLO tagging cho từng câu hỏi được sinh ra.
- Tích hợp RAG để truy xuất đúng phần nội dung cần kiểm tra.
- Thêm cơ chế điều chỉnh độ khó câu hỏi theo kết quả học tập của từng sinh viên.
- So sánh với baseline TF-IDF hoặc template-based để có đánh giá định lượng.
