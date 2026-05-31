# Problem Statement

## 1. Group Information

- **Class:** SE2037
- **Group:** 04
- **Topic:** A Lightweight AI-Powered Learning Management System for Personalized Feedback and Quiz Generation in Software Engineering Education

---

## 2. Context

Trong môi trường giáo dục đại học, đặc biệt các môn học thuộc ngành Kỹ Thuật Phần Mềm (Software Engineering), số lượng sinh viên đông và khối lượng nội dung lớn tạo ra áp lực đáng kể cho cả giảng viên lẫn sinh viên.

Các hệ thống Learning Management System (LMS) truyền thống như Moodle, Canvas, hay Google Classroom hiện đang được sử dụng rộng rãi, nhưng phần lớn các tác vụ quan trọng trong quá trình dạy và học vẫn phụ thuộc vào thao tác thủ công của giảng viên.

---

## 3. Core Problem

### 3.1. Về phía giảng viên

Giảng viên phải xử lý nhiều công việc lặp lại và tốn thời gian:

- **Tạo quiz thủ công:** Mỗi bài kiểm tra yêu cầu giảng viên tự soạn câu hỏi, đáp án, và phân loại theo chủ đề hoặc CLO — một quy trình tốn nhiều giờ mỗi tuần.
- **Phản hồi bài làm:** Với lớp học lớn (50–200 sinh viên), giảng viên không thể cung cấp phản hồi chi tiết, cá nhân hóa cho từng sinh viên sau mỗi bài tập.
- **Theo dõi tiến độ:** Việc xác định sinh viên nào đang gặp khó khăn ở CLO nào đòi hỏi phân tích dữ liệu thủ công, thường không được thực hiện thường xuyên.
- **Gợi ý tài liệu học tập:** Giảng viên khó có thể gợi ý tài liệu phù hợp với từng nhu cầu học tập riêng biệt của sinh viên.

### 3.2. Về phía sinh viên

Sinh viên gặp nhiều hạn chế trong quá trình tự học:

- **Phản hồi chậm hoặc thiếu:** Sinh viên phải chờ đợi lâu để nhận phản hồi từ giảng viên, làm giảm hiệu quả học tập.
- **Thiếu tài nguyên luyện tập:** Số lượng câu hỏi luyện tập có sẵn thường hạn chế và không đa dạng.
- **Khó tự đánh giá điểm yếu:** Sinh viên không dễ dàng biết mình đang yếu ở CLO nào để tập trung ôn luyện.
- **Hỗ trợ ngoài giờ học hạn chế:** Ngoài giờ lên lớp, sinh viên ít có kênh hỗ trợ học tập hiệu quả.

### 3.3. Về phía hệ thống AI hiện tại

Các giải pháp AI hiện có trong giáo dục vẫn còn nhiều hạn chế:

- Chatbot giáo dục thường trả lời chung chung, thiếu ngữ cảnh cụ thể của môn học.
- Hệ thống quiz tự động chưa gắn kết với CLO hoặc syllabus.
- Phản hồi AI chưa được cá nhân hóa theo năng lực và lịch sử học tập của từng sinh viên.
- Thiếu hệ thống tích hợp đầy đủ: quiz generation + personalized feedback + learning analytics trong một LMS duy nhất.

---

## 4. Impact

Những vấn đề trên dẫn đến hậu quả cụ thể:

| Vấn đề | Hậu quả |
|---|---|
| Thiếu quiz luyện tập đa dạng | Sinh viên không có đủ tài nguyên tự kiểm tra kiến thức |
| Phản hồi chậm và chung chung | Sinh viên không biết cụ thể điểm nào cần cải thiện |
| Không theo dõi được CLO | Giảng viên khó phát hiện sớm sinh viên có nguy cơ không đạt chuẩn đầu ra |
| Workload giảng viên cao | Chất lượng giảng dạy bị ảnh hưởng khi giảng viên quá tải |
| Thiếu hỗ trợ ngoài giờ | Sinh viên tự học kém hiệu quả, phụ thuộc vào thời gian lên lớp |

---

## 5. Proposed Solution

Nhóm đề xuất xây dựng **A Lightweight AI-Powered Learning Management System** tích hợp:

- **LLM + RAG** để sinh quiz bám sát syllabus và tài liệu môn học.
- **CLO-aware quiz generation** để câu hỏi gắn với từng mục tiêu học tập cụ thể.
- **Personalized feedback generation** để cung cấp phản hồi chi tiết, phù hợp với từng bài làm của sinh viên.
- **Learning analytics dashboard** để giảng viên theo dõi tiến độ và CLO achievement.
- **RAG-based learning assistant** để hỗ trợ sinh viên hỏi đáp theo đúng nội dung môn học.

---

## 6. Positioning Statement

> This study does not aim to propose a new AI model from scratch. Instead, it investigates how existing AI technologies — specifically Large Language Models and Retrieval-Augmented Generation — can be integrated into a domain-specific Learning Management System and evaluates their effectiveness in improving quiz generation quality, personalized feedback delivery, and learning outcome tracking in Software Engineering Education.
