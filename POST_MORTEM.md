# 🏛️ Post-Mortem: Hành Trình HeritageVibe AI Tại Google AI Arena Vietnam 2026

> **Dự án:** HeritageVibe AI (Việt Phục Remix Engine)  
> **Tác giả:** Ngô Minh Thiên Bảo ([reukem](https://github.com/reukem)) — Học sinh Lớp 12A1, Trường Vinschool Central Park  
> **Cuộc thi:** Google AI Arena Vietnam 2026 (Đồng tổ chức bởi Google & Đại học Quốc gia Hà Nội - VNU)  
> **Chủ đề thi:** *Việt Phục Remix – Phối Trang Phục Truyền Thống Theo Phong Cách Gen Z*  
> **Cổng nộp bài:** `https://ai-arena-vietnam.vnu.edu.vn/dashboard/audition`  
> **Hạn chót Audition:** 23:59:59 Thứ Bảy, ngày 10/10/2026 (Asia/Ho_Chi_Minh)  
> **Kết quả:** Không qua vòng Audition (Eliminated) & Hoàn toàn không nhận được phản hồi từ BTC (Ghosted)  
> **Trạng thái nền tảng:** 100% Live, Mã nguồn mở & Triển khai công khai tại [https://reukem.github.io/heritagevibe-ai/](https://reukem.github.io/heritagevibe-ai/)

---

## 📋 1. Tổng Quan & Bối Cảnh Thực Tế (The Underdog Context)

Khi đăng ký tham dự **Google AI Arena Vietnam 2026**, mục tiêu của tác giả là đưa giải pháp công nghệ phục vụ bảo tồn di sản văn hóa Việt Nam: giải quyết mâu thuẫn giữa mong muốn thể hiện cá tính thời trang của thế hệ trẻ (Gen Z) với chuẩn mực tôn nghiêm của Cổ phục Đại Việt và thổ cẩm 54 dân tộc.

Tuy nhiên, có một thực tế chênh lệch rất lớn về bối cảnh tham gia:

1. **Học sinh Cấp 3 Đơn độc vs. Đội thi Đại học Chuyên nghiệp:**
   - Trong khi hầu hết các đội thi tham gia Google AI Arena là sinh viên đại học chuyên ngành Công nghệ Thông tin, Khoa học Máy tính đến từ các trường đại học hàng đầu (ĐHQG Hà Nội, Bách Khoa, RMIT, VinUni...) với đội hình từ 3–5 thành viên kèm giảng viên cố vấn;
   - **HeritageVibe AI** được kiến trúc, thiết kế đồ họa SVG, lập trình frontend, tích hợp mô hình ngôn ngữ lớn và hoàn thiện hồ sơ kỹ thuật bởi **duy nhất một học sinh lớp 12 (17 tuổi)** trong các khung giờ tự học ngoài giờ lên lớp.

2. **Khối lượng công việc đã thực thi trong Sprint Audition:**
   - **Interactive Mannequin Studio (Vector SVG 60 FPS):** Xây dựng bộ ma-nơ-canh tương tác vector động 4 lớp (Thượng y, Hạ y, Giày dép, Phụ kiện), tự động render đường nét khuy búp xửa, nếp dập ly, túi hộp cargo, đai cườm Tây Nguyên mà không cần dùng bất kỳ framework đồ họa nặng nề nào.
   - **Kho Dữ Liệu 54 Món Y Phục Di Sản & Streetwear:** Thu thập, chuẩn hóa thuộc tính lịch sử từ *Khâm Định Đại Nam Hội Điển Sự Lệ*, *Đại Việt Sử Ký Toàn Thư*, trang phục 54 dân tộc (H'Mông, Dao, Thái, Ê Đê, Chăm, Tày) đến thời trang đường phố Gen Z.
   - **Kiến Trúc AI Kép (Dual-Engine Cultural AI):**
     - *Động cơ 1 (Gemini 2.5 Flash Live API):* Tích hợp trực tiếp Google Cloud Generative Language API với System Instruction phân tầng và Type-Safe Structured JSON Schema.
     - *Động cơ 2 (Gemini Heuristic Guardrail Engine):* Bộ quy tắc văn hóa động chạy ngoại tuyến trong trình duyệt bằng công thức toán học ma trận trọng số, tích hợp engine hiển thị công thức LaTeX KaTeX.
   - **Tri-Layer Cultural Guardrail Protocol:** Bộ 3 tầng khiên văn hóa tự động phát hiện và ngăn chặn mọi hành vi biến dạng cấu trúc (croptop rách vạt) hoặc xúc phạm phẩm hàm (lạm dụng long văn ngũ trảo vào sàn nhảy EDM).
   - **Web Audio API Synthesizer:** Tự phát triển bộ tổng hợp âm thanh Harmonics chuông đồng cổ truyền 528Hz khi phối đồ đạt chuẩn và chiêng cảnh báo Warning Gong 180Hz khi vi phạm.
   - **Xuất Lookbook Card HD 1080x1350 PNG:** Kết xuất hình ảnh đồ họa bìa tạp chí văn hóa bằng HTML5 Canvas 2D phục vụ chia sẻ mạng xã hội.

Toàn bộ giải pháp đã được đóng gói thành một Single-Page Application hoàn chỉnh, sẵn sàng trải nghiệm trực tiếp trên web và bàn giao kèm hồ sơ kỹ thuật chi tiết 152 dòng (`SUBMISSION_DOSSIER.md`) cùng bản thiết kế prompt 11 trang trước hạn chót quy định.

---

## 🚫 2. Thực Tế Nghiệt Ngã & Trải Nghiệm "Ghosted" Từ Ban Tổ Chức

Sau khi hoàn thành nộp bài đúng hạn (23:59:59 ngày 10/10/2026), quá trình chấm thi và công bố kết quả của vòng Audition đã diễn ra theo cách khiến người tham gia không khỏi thất vọng:

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                     TIMELINE & TRẢI NGHIỆM THỰC TẾ                         │
├─────────────────────────────────────────────────────────────────────────────┤
│ • 10/10/2026: Nộp bài thành công lên cổng ai-arena-vietnam.vnu.edu.vn        │
│ • Tuần 1-2:   Chờ đợi thông báo kết quả qua email theo cam kết cuộc thi     │
│ • Kết quả:    HOÀN TOÀN KHÔNG CÓ BẤT KỲ EMAIL NÀO TỪ BAN TỔ CHỨC.           │
│               - Không có email thông báo kết quả trúng tuyển hay trượt.     │
│               - Không có email cảm ơn tham gia.                             │
│               - Không có bảng điểm tiêu chí hay nhận xét từ Hội đồng.       │
│ • Phát hiện:  Thí sinh phải tự truy cập lại website dashboard của cuộc thi  │
│               mới thấy trạng thái tài khoản bị đánh dấu "Không lọt vào vòng │
│               trong" một cách âm thầm và lạnh lùng.                         │
└─────────────────────────────────────────────────────────────────────────────┘
```

### Điểm Đáng Trách Trong Khâu Tổ Chức:
1. **Sự thiếu minh bạch và tôn trọng công sức thí sinh:**  
   Đối với một cuộc thi mang thương hiệu của Google kết hợp cùng một đại học quốc gia, việc gửi một email thông báo tự động (kèm lời cảm ơn và trạng thái bài thi) là tiêu chuẩn tối thiểu trong quản trị sự kiện công nghệ. Việc hoàn toàn "im hơi lặng tiếng" (ghosting) hàng trăm thí sinh đã bỏ ra hàng tuần lễ tâm huyết là hành xử thiếu chuyên nghiệp.
2. **Thiếu phản hồi kỹ thuật (No Rubric Feedback):**  
   Không có bất kỳ dữ liệu nào cho biết bài thi bị trừ điểm ở đâu: do tiêu chí chấm thiên vị các đề tài đại học khác? Do giới hạn số lượng? Hay do giải pháp thuần web client-side không nằm trong "khẩu vị" của hội đồng? Thí sinh hoàn toàn không nhận được bài học cải thiện nào từ chính ban giám khảo.

---

## 💡 3. Nhìn Nhận Khách Quan & Bài Học Tự Rút Ra (Self-Reflection)

Dù thất vọng về khâu tổ chức, nhìn lại bài thi một cách công tâm và khách quan dưới góc độ kỹ thuật:

### Những mặt còn hạn chế có thể là nguyên nhân không hợp thị hiếu:
1. **Thiếu Backend phức tạp (Pure Client-Side Architecture):**  
   Để tối ưu hóa trải nghiệm mượt mà, không phụ thuộc server và chi phí vận hành bằng 0 cho người dùng phổ thông, dự án chọn kiến trúc Single-Page Application (HTML/JS/Tailwind) kết hợp gọi thẳng Client REST API. Các hội đồng học thuật tại các trường đại học thường có xu hướng ưu tiên các kiến trúc có backend phức tạp (Python FastAPI, Docker, Microservices, Vector Database chuyên biệt như Pinecone/Milvus), ngay cả khi giải pháp thuần client có tính ứng dụng thực tế cao hơn.
2. **Định dạng sản phẩm là Web tương tác thay vì báo cáo nghiên cứu hàn lâm:**  
   Bài thi tập trung vào việc tạo ra một sản phẩm sống (living product) mà người dùng chạm vào dùng được ngay, có âm thanh, có ma-nơ-canh và xuất ảnh thẻ lookbook. Tuy nhiên, ở các vòng chấm sơ khảo đại học, các bài thi dạng nghiên cứu lý thuyết hoặc mô hình ML fine-tune riêng biệt thường dễ ghi điểm theo tiêu chí học thuật hơn.
3. **Vị thế thí sinh tự do (Solo Independent High Schooler):**  
   Không có trường đại học bảo trợ danh nghĩa, không có giảng viên hướng dẫn đứng tên cùng, việc một học sinh lớp 12 tự nộp bài thi solo ở một sân chơi chủ yếu dành cho sinh viên đại học luôn là một bất lợi tự nhiên về mặt nhận diện.

---

## 🌟 4. Giá Trị Thực Sự Vượt Qua Khuôn Khổ Cuộc Thi

Thất bại ở một cuộc thi không định nghĩa giá trị của sản phẩm:

| Tiêu Chí | Kết Quả Trong Cuộc Thi | Giá Trị Thực Tế Ngoài Đời |
| :--- | :--- | :--- |
| **Trạng thái bài thi** | Bị loại ở vòng Audition (Không lọt vào chung kết) | Nền tảng hoạt động 100% không một lỗi runtime |
| **Email phản hồi** | Bị ghosted, không có thông báo | Mã nguồn mở hoàn toàn, minh bạch trên GitHub |
| **Trải nghiệm người dùng** | Giám khảo có thể chỉ lướt qua vài phút | Hàng chục bộ trang phục được phối, chuông đồng 528Hz ngân vang thực sự |
| **Tác động văn hóa** | Bị gạt khỏi danh sách giải thưởng | Bảo tồn chuẩn mực Cổ phục Đại Việt & Thổ cẩm 54 dân tộc cho thế hệ trẻ |

### Lời Kết:
**HeritageVibe AI** ra đời không phải chỉ để tìm kiếm một tấm giấy chứng nhận hay vài dòng khen ngợi từ một ban tổ chức thiếu chu đáo. Dự án ra đời vì tình yêu với Cổ phục Việt Nam, niềm đam mê với trí tuệ nhân tạo và mong muốn chứng minh rằng: **Một học sinh phổ thông Việt Nam hoàn toàn có thể tự tay thiết kế và lập trình nên một sản phẩm AI văn hóa có chiều sâu kỹ thuật và thẩm mỹ cao.**

Mã nguồn của HeritageVibe AI sẽ mãi được lưu trữ công khai tại kho lưu trữ này như một minh chứng cho tinh thần tự lực, bền bỉ và tình yêu di sản bất diệt.

---

*Hồ Chí Minh, tháng 10 năm 2026*  
**Ngô Minh Thiên Bảo ([reukem](https://github.com/reukem))**  
*Lead Architect & Builder, HeritageVibe AI*
