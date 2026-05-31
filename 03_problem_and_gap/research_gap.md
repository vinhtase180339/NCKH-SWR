# Research Gap

## 1. Group Information

- **Class:** SE2037
- **Group:** 04
- **Topic:** A Lightweight AI-Powered Learning Management System for Personalized Feedback and Quiz Generation in Software Engineering Education

---

## 2. What Existing Work Has Done

Dựa trên phân tích literature review matrix, các nghiên cứu trước đã đạt được:

| Area | What Has Been Done |
|---|---|
| LLM in LMS | Tích hợp virtual assistant LLM vào LMS để hỗ trợ hỏi đáp và điều hướng (Paper 01) |
| Quiz generation | Dùng LLM để tự động sinh câu hỏi từ tài liệu khóa học (Paper 02) |
| RAG + Quiz | Kết hợp RAG với LLM để sinh quiz bám sát nội dung môn học (Paper 03) |
| Personalized feedback | Dùng LLM với in-context learning để sinh phản hồi cá nhân hóa (Paper 04) |
| RAG in education | Survey toàn diện về ứng dụng RAG trong giáo dục (Paper 05) |
| RAG architecture | Đặt nền móng kỹ thuật cho kiến trúc retriever + generator (Paper 06) |

---

## 3. Identified Research Gaps

### Gap 1: Thiếu CLO-awareness trong quiz generation

**Observation:** Các hệ thống quiz generation hiện tại (Paper 02, Paper 03) sinh câu hỏi từ nội dung tài liệu nhưng chưa gắn kết câu hỏi với Course Learning Outcomes (CLO) cụ thể.

**Impact:** Giảng viên không thể biết sinh viên đang yếu ở CLO nào, và câu hỏi được sinh ra không đảm bảo phân bổ đều theo mục tiêu học tập.

**Our contribution:** Hệ thống của nhóm sẽ gắn tag CLO cho từng câu hỏi được sinh ra, đảm bảo phân bổ theo CLO và hỗ trợ theo dõi CLO achievement.

---

### Gap 2: Thiếu hệ thống tích hợp quiz generation và personalized feedback trong cùng một LMS

**Observation:** Quiz generation (Paper 02, 03) và personalized feedback (Paper 04) được nghiên cứu độc lập. Chưa có hệ thống nào tích hợp cả hai tính năng trong một LMS hoàn chỉnh phục vụ cả giảng viên và sinh viên.

**Impact:** Sinh viên phải dùng nhiều công cụ riêng lẻ, thiếu trải nghiệm học tập liên tục và xuyên suốt.

**Our contribution:** Hệ thống của nhóm tích hợp quiz generation + personalized feedback + learning assistant trong một nền tảng LMS duy nhất.

---

### Gap 3: Thiếu RAG pipeline gắn với syllabus và CLO trong môi trường Software Engineering Education

**Observation:** Paper 03 dùng RAG cho quiz generation nhưng knowledge base chỉ là tài liệu thô, chưa được cấu trúc theo syllabus và CLO. Paper 05 (survey) xác nhận đây là gap phổ biến trong RAG educational applications.

**Impact:** AI có thể sinh nội dung không bám sát mục tiêu giảng dạy, gây khó khăn cho giảng viên trong kiểm soát chất lượng.

**Our contribution:** Nhóm xây dựng RAG pipeline với knowledge base được tổ chức theo syllabus và CLO, đảm bảo nội dung sinh ra luôn course-aware.

---

### Gap 4: Thiếu đánh giá thực nghiệm trong môi trường Software Engineering Education

**Observation:** Hầu hết các hệ thống được đánh giá trên quy mô nhỏ hoặc trong domain tổng quát. Chưa có nghiên cứu đánh giá hệ thống AI-powered LMS cụ thể trong môi trường giảng dạy Software Engineering tại Việt Nam.

**Impact:** Thiếu bằng chứng về tính hiệu quả của AI-powered LMS trong bối cảnh cụ thể này.

**Our contribution:** Nhóm thực hiện đánh giá thực nghiệm với dataset mô phỏng và user survey trong môi trường Software Engineering Education.

---

## 4. Gap Summary Statement

> Existing AI-powered learning management systems mainly focus on either quiz generation or personalized feedback as isolated features, while limited attention has been given to integrating both features with CLO-awareness and RAG-based syllabus retrieval in a unified LMS platform for Software Engineering Education. Furthermore, empirical evaluation of such systems in the context of Vietnamese higher education remains scarce.

---

## 5. How Our System Addresses These Gaps

| Gap | Our Solution |
|---|---|
| Gap 1: No CLO-awareness in quiz generation | CLO-tagged quiz generation; dashboard tracking CLO achievement per student |
| Gap 2: No unified system for quiz + feedback | Single LMS integrating quiz generation, personalized feedback, and learning assistant |
| Gap 3: RAG not aligned with syllabus/CLO | RAG knowledge base structured by syllabus topics and CLO; course-aware retrieval |
| Gap 4: Limited empirical evaluation in SE Education | Experimental evaluation with simulated dataset + user survey with SE students |
