# Literature Review Matrix

## 1. Group Information

- **Class:** SE2037
- **Group:** 04
- **Topic:** A Lightweight AI-Powered Learning Management System for Personalized Feedback and Quiz Generation in Software Engineering Education

---

## 2. Literature Review Matrix

| No | Paper Title | Year | Venue | Domain | AI Method | Dataset | Evaluation Metrics | Main Contribution | Limitation | Relevance to Our Topic |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Exploring the Integration of Virtual Assistant Using Large Language Models in Learning Management System: Enhancing Educational Accessibility and Efficiency | 2024 | ICITSI 2024 (IEEE) | Education / LMS | LLM, Virtual Assistant | LMS interaction logs | User satisfaction, accessibility score | Integrated LLM-based virtual assistant into LMS to improve accessibility and reduce manual workload | Small-scale evaluation, limited to one course context | High – directly addresses LLM integration into LMS, similar system scope |
| 2 | LLM-Based Quiz Generation for Assessments in Learning Management System | 2025 | ICC-ROBINS 2025 (IEEE) | Education / Assessment | LLM | Course materials, textbook content | Quiz quality, accuracy, expert rating | Proposed an LLM pipeline to automatically generate quiz questions from course content inside LMS | No CLO alignment, no personalization based on student performance | High – core feature of our system; provides baseline for quiz generation |
| 3 | Enhancing Engineering Education through LLM-Driven Adaptive Quiz Generation: A RAG-Based Approach | 2024 | FIE 2024 (IEEE) | Engineering Education | LLM, RAG | Engineering course slides and textbooks | Quiz relevance, expert evaluation | Combined RAG with LLM to generate context-aware quizzes aligned with course materials | Limited to quiz generation only, no feedback or progress tracking | High – closest to our approach; RAG + LLM for quiz generation in engineering education |
| 4 | Generating In-Context, Personalized Feedback for Intelligent Tutors with Large Language Models | 2025 | Int. Journal of AI in Education (Springer) | Intelligent Tutoring | LLM, prompt engineering | Student responses and tutor logs | Feedback relevance, correctness, user rating | Used LLM with in-context learning to generate personalized feedback aligned with student answers | Dependent on high-quality prompt design; may not generalize across domains | High – directly supports personalized feedback feature in our system |
| 5 | Retrieval-Augmented Generation for Educational Application: A Systematic Survey | 2025 | Computers and Education: AI (Elsevier) | Education (survey) | RAG, LLM, embedding | Various educational datasets | Survey-based analysis | Systematic review of RAG applications in education; identifies trends, gaps, and best practices | Survey only, no new system implemented | High – provides theoretical foundation and identifies research gaps for RAG in education |
| 6 | Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks | 2020 | NeurIPS 2020 | NLP / General | RAG, DPR, BART | Open-domain QA datasets | Exact Match, F1 | Proposed the RAG architecture combining dense retrieval with seq2seq generation | General-purpose; not tailored for education or LMS context | Medium – foundational RAG paper; provides technical basis for our AI service design |
| 7 | A Survey on Retrieval-Augmented Text Generation | 2023 | arXiv | NLP / General | RAG, various retrievers | Multiple NLP benchmarks | Task-specific metrics | Comprehensive survey on RAG variants, retrieval strategies, and generation methods | Not education-specific | Medium – useful for understanding RAG design choices in our system |
| 8 | Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks | 2019 | EMNLP 2019 | NLP / Embeddings | BERT, Siamese network | STS benchmark, NLI datasets | Spearman correlation, accuracy | Efficient sentence embedding model for semantic similarity tasks | Fixed embedding space; may need fine-tuning for domain-specific content | Medium – embedding model candidate for our RAG retrieval component |

---

## 3. Gap Analysis Summary

Dựa trên bảng trên, các gap được xác định:

| Gap | Observation |
|---|---|
| **Gap 1** | Hầu hết hệ thống quiz generation chưa gắn kết với CLO (Course Learning Outcome) cụ thể. |
| **Gap 2** | Phản hồi cá nhân hóa vẫn chưa được tích hợp đồng thời với quiz generation trong một hệ thống LMS duy nhất. |
| **Gap 3** | Chưa có hệ thống nào kết hợp đầy đủ RAG + LLM + CLO-awareness + personalized feedback trong môi trường Software Engineering Education. |
| **Gap 4** | Đánh giá hiệu quả thực tế của AI trong LMS vẫn còn hạn chế về quy mô và tính đa dạng của đối tượng sinh viên. |

---

## 4. Notes

- Bảng sẽ được cập nhật khi có thêm bài báo mới được tìm và đọc.
- Mỗi bài trong bảng có file tóm tắt riêng tại `paper_summaries/paper_0X.md`.
- Gap analysis ở đây là tóm tắt; chi tiết hơn xem tại `03_problem_and_gap/research_gap.md`.
