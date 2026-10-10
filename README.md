# HeritageVibe AI // Nền Tảng Việt Phục & Thổ Cẩm 54 Dân Tộc x Gen Z

> **Dự Án Dự Thi Google AI Arena Vietnam 2026 — Vòng Audition**  
> *Chủ đề:* **Việt Phục Remix – Phối Trang Phục Truyền Thống Theo Phong Cách Gen Z**  
> *Tác giả:* **Ngô Minh Thiên Bảo (Aki / Reukem)** — Lớp 12A1 Trường Vinschool Central Park  
> *Trải nghiệm trực tiếp trên GitHub Pages:* **[https://reukem.github.io/heritagevibe-ai/](https://reukem.github.io/heritagevibe-ai/)**  
> *Mã nguồn GitHub:* **[https://github.com/reukem/heritagevibe-ai](https://github.com/reukem/heritagevibe-ai)**

---

## 🌟 1. Giới Thiệu Tổng Quan (Project Overview)

**HeritageVibe AI** là nền tảng AI Stylist cá nhân hóa đa phương thức, giải quyết bài toán mâu thuẫn cốt lõi giữa:
1. **Khát khao thể hiện cá tính thời trang tự do, năng động của thế hệ Gen Z** (streetwear, baggy pants, cargo, chunky sneakers, headphones Y2K).
2. **Trách nhiệm bảo tồn sự tôn nghiêm, chuẩn mực điển chế của Cổ phục Đại Việt** (*Áo Tấc, Áo Ngũ Thân, Giao Lĩnh, Nhật Bình*) và **tinh hoa thổ cẩm dệt tay của 54 Dân tộc anh em** (*H'Mông, Dao Đỏ, Thái, Ê Đê, Chăm, Tày*).

Nền tảng kết hợp hình tượng khảo cổ chuẩn xác (**Trống Đồng Ngọc Lũ**, **Chim Lạc**, **Văn Mây Như Ý Thời Trần**, **Phượng Hoàng Thời Lê - Nguyễn**) cùng **Phòng Phối Đồ Mannequin Tương Tác Vector SVG**, xuất kết quả dạng **Thẻ Lookbook Ngũ Hành HD** và thẩm định tự động qua **Hệ Thống Khiên Văn Hóa 3 Lớp**.

---

## 🧠 2. Kiến Trúc AI Kép Độc Đáo (Dual-Engine Cultural AI Architecture)

Một trong những băn khoăn phổ biến nhất của người dùng là: *"Liệu hệ thống này chỉ có điểm số dựng sẵn (pre-scored) hay thực sự có AI thẩm định?"*

HeritageVibe AI được kiến trúc theo mô hình **AI Kép 2 Chế Độ (Dual-Engine)** nhằm cân bằng hoàn hảo giữa tính năng AI thế hệ mới từ Google Cloud và trải nghiệm mượt mà không gián đoạn cho người dùng phổ thông:

```
                                  ┌──────────────────────────────────────────────┐
                                  │   Phòng Phối Đồ Mannequin (54 Món Remix)     │
                                  │   (Thượng y + Hạ y + Giày dép + Phụ kiện)    │
                                  └──────────────────────┬───────────────────────┘
                                                         │
                                 ┌───────────────────────┴───────────────────────┐
                                 ▼                                               ▼
                    [CÓ GOOGLE GEMINI API KEY]                      [KHÔNG CẦN GEMINI API KEY]
              ┌─────────────────────────────────────┐         ┌─────────────────────────────────────┐
              │      ĐỘNG CƠ 1: GEMINI LIVE API     │         │   ĐỘNG CƠ 2: GEMINI HEURISTIC MATRIX│
              │       Google Gemini 2.5 Flash       │         │    Dynamic Cultural Rule Engine     │
              │  (Gọi API trực tiếp Google Cloud)   │         │    (Chạy Offline Trong Trình Duyệt) │
              └──────────────────┬──────────────────┘         └──────────────────┬──────────────────┘
                                 │                                               │
                                 └───────────────────────┬───────────────────────┘
                                                         ▼
                                 ┌───────────────────────────────────────────────┐
                                 │   KẾT QUẢ THẨM ĐỊNH THỜI GIAN THỰC (REALTIME) │
                                 │   • Điểm Số Chuẩn Mực Toán Học (0 - 100)      │
                                 │   • Vòng Đo Điểm Circular SVG Gauge (80px)    │
                                 │   • Bảng Màu Ngũ Hành Tương Sinh (Color Hex)  │
                                 │   • Đánh Giá 3 Lớp Guardrail & Đề Xuất Sửa Đổi│
                                 │   • Xuất Thẻ Lookbook HD 1080x1350 PNG        │
                                 └───────────────────────────────────────────────┘
```

### Chế Độ 1: Google Gemini 2.5 Flash Live API (Trực Tiếp Google Cloud)
- **Cơ chế:** Khi người dùng bấm nút `Google Gemini AI` trên thanh điều hướng và dán Google Gemini API Key cá nhân (lưu an toàn trong `localStorage`).
- **Pipeline:** Mỗi lần nhấn *"AI Thẩm Định Set Đồ Này"*, hệ thống gửi toàn bộ metadata của 4 món đồ đang mặc lên endpoint `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent`.
- **Suy luận CoT:** Mô hình **Gemini 2.5 Flash** đối chiếu sâu quy chuẩn *Khâm Định Đại Nam Hội Điển Sự Lệ* và triết lý dệt may vùng cao, đóng gói kết quả dạng **Type-Safe Structured JSON**.

### Chế Độ 2: Gemini Heuristic Guardrail Engine (Mô Hình Quy Tắc Văn Hóa Động Ngoại Tuyến)
- **Cơ chế:** Hoạt động mặc định ngay khi vào trang web, đảm bảo mọi giám khảo hay khách tham quan đều có thể thử nghiệm tức thì mà không cần đăng ký API Key.
- **Tính toán Động (Dynamic Mathematical Calculation - Hoàn toàn KHÔNG PHẢI hardcoded tĩnh!):**
  1. **Công thức tính điểm động:** Mỗi món đồ trong 54 items mang một chỉ số toàn vẹn văn hóa (`layerScore`). Điểm tổng thể được tính toán bằng trung bình cộng ma trận trọng số:
     $$\text{Integrity Score} = \text{round}\left(\frac{\text{Score}_{\text{Thượng Y}} + \text{Score}_{\text{Hạ Y}} + \text{Score}_{\text{Giày}} + \text{Score}_{\text{Phụ Kiện}}}{4}\right)$$
     *Ví dụ:* Áo Ngũ Thân (98đ) + Váy Quấn Ê Đê (97đ) + Sneakers Trắng (94đ) + Trâm Bạc (97đ) $\rightarrow$ Điểm = `96/100` (APPROVED). Nếu đổi sang Bốt combat đinh tán (65đ) $\rightarrow$ Điểm lập tức tụt xuống `89/100`!
  2. **Bộ ngắt vi phạm tức thì (Violation Circuit Breaker):** Nếu set đồ chứa bất kỳ món nào vi phạm cấu trúc (Áo croptop EDM, Quần biker bó sát, Quần rách), điểm số bị phạt tụt dốc xuống `12 – 15/100`, kích hoạt tiếng **Chiêng Cảnh Báo 180Hz**, đổi viền ma-nơ-canh sang đỏ nét đứt và hiển thị 3 đề xuất chấn chỉnh văn hóa.
  3. **Ma trận Bảng màu Ngũ Hành Động:** Trích xuất 4 mã màu HEX thật của 4 món đồ đang mặc (`#C29B38`, `#18181B`, `#FFFFFF`, `#E2E8F0`), phân định 4 nguyên tố *Thủy - Kim - Thổ - Thạch* và viết lời luận giải tương sinh tương khắc.
  4. **Ma-nơ-canh Haute-Couture Vector SVG:** Tự động vẽ các chi tiết đặc trưng (hàng khuy búp xửa, hoa văn sáp ong Mèo Vạc, túi hộp cargo, đai cườm Tây Nguyên, tai nghe Bluetooth...) theo thời gian thực.

---

## 🛡️ 3. Hệ Thống Khiên Văn Hóa 3 Lớp (Tri-Layer Cultural Guardrails)

Dựa trên nguyên tắc *"Tôn trọng nguồn cội - Cởi mở sáng tạo"*, hệ thống thẩm định theo 3 tầng bảo vệ nghiêm ngặt:

1. **Lớp 1: Bất Biến Về Cấu Trúc May (Structural Immutability)**:
   - Bảo toàn 5 thân vạt áo che kín thân thể (ngũ thân tượng trưng tứ thân phụ mẫu ôm bọc lấy con cái).
   - Bảo toàn hàng 5 cúc khuy cài tượng trưng cho Ngũ Thường (*Nhân, Lễ, Nghĩa, Trí, Tín*) và Ngũ Hành.
   - Cấm tuyệt đối: Cắt ngắn tà áo hở rốn, xẻ ngực phản cảm, cào rách vạt vải.
2. **Lớp 2: Tôn Nghiêm Phẩm Hàm & Biểu Tượng Cấm Kỵ (Sacred Demarcation)**:
   - Nghiêm cấm lạm dụng hoa văn hoàng quyền tối cao (*Long văn 5 móng*) hoặc lễ phục tế lễ cung đình (*Nhật Bình hoàng hậu*) vào không gian nhạy cảm (quán bar, vũ trường quẩy rave).
   - Khuyến khích hoa văn mỹ thuật dân gian: Thủy ba (sóng nước), Tứ quý (*Tùng - Cúc - Trúc - Mai*), Vân mây như ý, hoa văn thổ cẩm quả trám, mặt trời, chim muông Tây Bắc.
3. **Lớp 3: Văn Minh Đương Đại (Contemporary Syncretic Modernization)**:
   - Khuyến khích sự lai ghép thẩm mỹ thanh lịch: Chân váy midi xếp ly rẽ quạt, quần baggy suông thanh lịch, quần cargo túi hộp techwear, giày sneakers trắng minimalist, bốt Chelsea da mờ, túi mây tre đan thủ công Chương Mỹ, lụa Vạn Phúc, tơ tằm Bảo Lộc.

---

## 👗 4. Kho Đồ Remix Đa Dạng (54+ Món Y Phục)

Kho đồ gồm 4 nhóm trang phục:
- **Thượng Y (16 món):** Áo Tấc, Áo Ngũ Thân tay chẽn, Áo Giao Lĩnh, Áo Nhật Bình, Áo Tứ Thân, Áo Yếm, Thổ Cẩm H'Mông dệt lanh sáp ong, Áo Cóm Thái khuy bướm Búp Xửa, Áo Chàm Dao Đỏ đính bông len đỏ, Áo Dêch Ê Đê, Áo dài Aw Kamei Chăm, Áo chàm Tày/Nùng, Bomber Jacket thêu Chim Lạc, Blazer Oversized, Corset gấm cách tân, Áo Nhật Bình Croptop EDM (Vi phạm).
- **Hạ Y (13 món):** Chân váy midi xếp ly rẽ quạt, Quần baggy ống rộng streetwear, Quần cargo túi hộp parachute, Quần âu suông Linen, Váy xòe thổ cẩm H'Mông dập ly, Chân váy denim maxi xẻ tà, Váy Thái đai xanh ngọc, Váy quấn Kút Ê Đê, Váy tơ sống chiffon 3 tầng, Quần lụa đen Lãnh Mỹ A, Quần lụa trắng Hà Đông, Quần Biker shorts (Vi phạm), Quần Jeans rách (Vi phạm).
- **Giày Dép (9 món):** Hài thêu sen, Sneakers trắng Minimalist, Chunky sneakers đế bánh mì 6cm, Guốc mộc quai gấm, Guốc mít sơn mài vẽ cá chép thếp vàng, Bốt Chelsea da bò, Sandal quai mảnh, Hài thổ cẩm mũi hếch, Bốt combat đinh tán.
- **Phụ Kiện (11 món):** Túi mây tre đan Chương Mỹ & Khăn vấn lụa, Khăn Piêu Thái, Kiềng bạc H'Mông chạm sóng lúa, Tai nghe chụp tai Bluetooth Gen Z, Túi Tote canvas Trống Đồng, Kính râm Oval Retro, Nón quai thao, Chuỗi ngọc trai & quạt dó, Trâm bạc hoa sen, Đai cườm Tây Nguyên, Kính râm Cyberpunk Neon LED.

---

## 🎨 5. Tính Năng Nổi Bật (Key Features)

* **Phòng Phối Đồ Mannequin Kéo Thả (Drag & Drop + Click-to-Equip):** Người dùng có thể kéo thả trực tiếp món đồ từ tủ đồ thả vào hình nộm hoặc bấm nút "Mặc Vào".
* **Tìm Kiếm & Lọc Chuyên Sâu Thời Gian Thực:** Lọc theo 5 phân nhóm (*Tất Cả*, *Cổ Phục Triều Đình*, *Dân Tộc Vùng Cao*, *Gen Z Streetwear*, *Test Cảnh Báo*) và tìm kiếm theo từ khóa chất liệu, triều đại.
* **Âm Vang Di Sản (Web Audio API Synthesizer):** Tích hợp chuông đồng cổ (*Bronze Bell 528Hz hài âm*) khi phối đồ hợp chuẩn và chiêng cảnh báo (*Warning Gong 180Hz*) khi phát hiện vi phạm lễ giáo, kèm 4 cột sóng âm equalizer nhảy múa theo thời gian thực.
* **Xuất Thẻ Lookbook HD (Canvas-to-PNG):** Nút xuất ảnh độ phân giải 1080x1350 phong cách bìa tạp chí Vogue/Elle Heritage, sẵn sàng chia sẻ lên Instagram, TikTok, Facebook.
* **Tạo Prompt Ảnh AI Đa Nền Tảng:** Hỗ trợ tạo và sao chép câu lệnh tạo ảnh chuyên sâu cho Google Flow, Midjourney v6, Flux.1 để render trang phục cổ phục tách nền trong suốt.

---

## 🚀 6. Hướng Dẫn Sử Dụng Nhanh (Quick Start)

1. Mở trang web tại: **[https://reukem.github.io/heritagevibe-ai/](https://reukem.github.io/heritagevibe-ai/)**
2. **Thử nghiệm 3 Bộ Mẫu Nhanh (Preset Buttons):**
   - **Case 1 (Cổ Phục Chuẩn Mực 98đ):** Áo Tấc Xanh Thiên Thanh + Chân Váy Midi + Hài Thêu Sen + Túi Mây Tre Đan.
   - **Case 2 (Cảnh Báo Vi Phạm 12đ):** Áo Nhật Bình Croptop Xé Rách + Quần Biker Shorts + Combat Boots.
   - **Case 3 (Thổ Cẩm Vùng Cao 96đ):** Áo Thổ Cẩm H'Mông + Quần Baggy Kaki + Kiềng Bạc + Chunky Sneakers.
3. Tự do sáng tạo trang phục từ kho **54 món đồ** và nhấn **"AI Thẩm Định Set Đồ Này"** để xem AI phân tích!
4. *(Tùy chọn)* Bấm **"Google Gemini AI"** ở góc trên bên phải để kết nối trực tiếp Gemini 2.5 Flash API Key của bạn.

---

## 📄 7. Bản Quyền & Dự Thi

- **Cuộc thi:** Google AI Arena Vietnam 2026
- **Tác giả:** Ngô Minh Thiên Bảo (Aki / Reukem) — Lớp 12A1 Vinschool Central Park
- **Email:** `baongoplayzgame@gmail.com`
