# 📊 BÁO CÁO THU HOẠCH NGHIỆM THU BÀI LAB 3 (BƯỚC 3 — SUBMISSION ARTIFACT)

> **Họ và Tên Học viên:** Lưu Nguyễn Tiến Anh
> **Mã Sinh Viên / Mã Học viên:** 2A202603002  
> **Chủ đề Lựa chọn:** Trợ lý Học vụ & Tra cứu Lịch thi VinUni:* Tra cứu điểm GPA, lịch thi và đặt lịch tư vấn học vụ với Cố vấn.

---

## 1. BẢNG CHẤM ĐIỂM AGENTIC FIT SCORING MATRIX (ĐÁNH GIÁ CHỦ ĐỀ)

| Tiêu chí Đánh giá | Mức độ (1 - 5) | Giải trình chi tiết lý do chọn điểm |
| :--- | :---: | :--- |
| **1. Multi-step Reasoning** | 4 / 5 | Bài toán có yêu cầu chia nhỏ nhiều bước suy luận nối tiếp nhau không? |
| **2. Tool Interaction** | 5 / 5 | Hệ thống có cần kết nối với MCP Server / Cơ sở dữ liệu bên ngoài không? |
| **3. Dynamic Decision** | 4 / 5 | Bước tiếp theo có phụ thuộc vào kết quả quan sát bước trước không? |
| **4. Long Horizon Goal** | 3 / 5 | Hệ thống có phải giữ mục tiêu xuyên suốt qua nhiều lượt xử lý không? |
| **TỔNG ĐIỂM AGENTIC FIT** | **16/ 20** | *Nếu tổng điểm > 12/20: Bài toán rất phù hợp triển khai Agentic System.* |

---

## 2. TRÍCH XUẤT KẾT QUẢ WATERFALL TRACE LOG (SAU KHI CHẠY TEST SUITE TRÊN API THẬT)

> ⚠️ **YÊU CẦU NGHIỆM THU:** Mở tệp `.env` điền `GEMINI_API_KEY` (hoặc `OPENAI_API_KEY`) để kết nối LLM thật trước khi thực thi `python src/app.py --all`. Bài nộp chỉ dùng Mock Offline Provider sẽ không đạt điểm nghiệm thực tế.

Dán 1 đoạn trích xuất log tiêu biểu từ file `docs/trace_waterfall.json` sinh ra từ phản hồi LLM API thật:

```json
[
  {
    "step": 1,
    "query": "quy chế học vụ VinUni yêu cầu bao nhiêu tín chỉ?",
    "action_type": "FINAL_ANSWER",
    "thought": "Gemini phản hồi trực tiếp bằng văn bản (không cần gọi công cụ).",
    "output": "Số lượng tín chỉ bắt buộc tại VinUni phụ thuộc vào **chương trình đào tạo và ngành học cụ thể** mà sinh viên đang theo học. Thông thường:\n\n- **Chương trình Cử nhân (Quản trị Kinh doanh, Khoa học Máy tính, v.v.):** Thường yêu cầu khoảng **120 – 130+ tín chỉ** (tùy theo từng ngành và chuyên ngành).\n- **Chương trình Kỹ sư / Bác sĩ Y khoa:** Số lượng tín chỉ sẽ cao hơn, phù hợp với khung chương trình đào tạo chuyên sâu và thời gian học tập tương ứng.\n\nChương trình học bao gồm các nhóm học phần:\n1. **Các môn Học thuật Cốt lõi & Đại cương (General Education / Core Curriculum)**\n2. **Các môn Cơ sở Ngành & Chuyên ngành (Major Core & Electives)**\n3. **Thực tập / Đồ án tốt nghiệp / Dự án thực tế (Capstone Project / Internship)**\n\n---\n👉 **Lưu ý:** Nếu bạn muốn tra cứu chi tiết hồ sơ cá nhân và số tín chỉ bạn đã tích lũy/còn thiếu, vui lòng cung cấp **Mã sinh viên** (ví dụ: `SV2026001`) để mình hỗ trợ tra cứu trực tiếp trên hệ thống nhé!",
    "latency_ms": 7122.3
  }
]
```

---

## 3. TỔNG KẾT KẾT QUẢ NGHIỆM THU & NỘP BÀI

- [ ] Đã điền API Key thật trong `.env` và xác nhận Agent chạy mượt mà trên LLM API thật (Gemini/OpenAI).
- **Tổng số Test Cases đã chạy thành công:** 5 / 5 test cases.
- **Số lượt gọi Tool qua MCP Server chính xác:** 5 lượt.
- **Kết quả đẩy Repo nộp bài:** [ ] Đã Commit và Push mã nguồn thành công lên GitHub cá nhân.

---

> ✅ **HOÀN TẤT NỘP BÀI:** Sao chép đường link GitHub Repository cá nhân của bạn và dán vào ô nộp bài trên hệ thống LMS VLearn để hoàn tất Bài Lab 3!
