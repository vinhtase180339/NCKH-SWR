# Research Questions

## 1. Group Information

- **Class:** SE2037
- **Group:** 04
- **Topic:** A Lightweight AI-Powered Learning Management System for Personalized Feedback and Quiz Generation in Software Engineering Education

---

## 2. Main Research Question

> How can Large Language Models and Retrieval-Augmented Generation be integrated into a Learning Management System to improve quiz generation quality, personalized feedback delivery, and learning outcome tracking in Software Engineering Education?

---

## 3. Sub Research Questions

### RQ1. Quiz Generation Quality

> How accurately and relevantly can the proposed RAG-based LLM system generate quiz questions aligned with specific Course Learning Outcomes (CLOs) from Software Engineering course materials?

**Motivation:** Xuất phát từ Gap 1 và Gap 3 — quiz generation hiện tại chưa gắn CLO và chưa bám sát syllabus.

**Expected metrics:**
- Quiz relevance score (expert rating, Likert scale 1–5)
- CLO alignment accuracy (% câu hỏi được gắn đúng CLO)
- So sánh với baseline: LLM-only (không RAG), TF-IDF-based generation

---

### RQ2. Personalized Feedback Effectiveness

> To what extent does the LLM-generated personalized feedback help students identify their weaknesses and improve their understanding of Software Engineering concepts?

**Motivation:** Xuất phát từ Gap 2 — phản hồi cá nhân hóa chưa được tích hợp trong LMS và chưa được đánh giá trong SE Education.

**Expected metrics:**
- Feedback relevance and correctness (expert rating)
- Student satisfaction score (survey, SUS)
- So sánh với baseline: template-based feedback, generic LLM feedback (không RAG)

---

### RQ3. System Usability and Integration

> How usable and effective is the proposed AI-powered LMS for both students and instructors in a Software Engineering course context?

**Motivation:** Xuất phát từ Gap 4 — thiếu đánh giá thực nghiệm người dùng trong môi trường SE Education thực tế.

**Expected metrics:**
- System Usability Scale (SUS) score
- Task completion rate
- User satisfaction survey (instructors and students)
- Perceived time saving compared to manual process

---

### RQ4. Learning Outcome Tracking

> How effectively can the proposed system track and visualize student progress in achieving Course Learning Outcomes (CLOs) compared to traditional LMS approaches?

**Motivation:** Xuất phát từ Gap 1 — không có hệ thống nào theo dõi CLO achievement tự động trong LMS.

**Expected metrics:**
- CLO achievement detection accuracy
- Instructor satisfaction with analytics dashboard (survey)
- So sánh với baseline: manual tracking, traditional LMS gradebook

---

## 4. Research Question — Gap Mapping

| Research Question | Addresses Gap |
|---|---|
| RQ1: Quiz generation quality | Gap 1 (no CLO-awareness), Gap 3 (RAG not aligned with syllabus) |
| RQ2: Personalized feedback effectiveness | Gap 2 (no unified quiz + feedback system) |
| RQ3: System usability | Gap 4 (limited empirical evaluation in SE Education) |
| RQ4: Learning outcome tracking | Gap 1 (no CLO-awareness), Gap 2 (no unified system) |

---

## 5. Notes

- Các RQ sẽ được trả lời thông qua thực nghiệm mô phỏng, expert evaluation, và user survey.
- RQ1 và RQ2 tập trung vào chất lượng AI output.
- RQ3 và RQ4 tập trung vào trải nghiệm người dùng và tính hữu dụng của hệ thống.
- Kết quả sẽ được trình bày trong `06_experiment_results/results.md`.
