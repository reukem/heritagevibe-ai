# HeritageVibe AI — Prompt Engineering Strategy & Guardrail Protocol

## 1. Triết Lý Thiết Kế Prompt (Prompt Design Philosophy)

Hệ thống prompt của HeritageVibe AI được thiết kế nhằm giải quyết bài toán mâu thuẫn giữa:
1. **Khát vọng sáng tạo cá nhân (Individual Expression)** của Gen Z.
2. **Tính tôn nghiêm và chuẩn mực lịch sử (Cultural Fidelity & Preservation)** của di sản trang phục Việt Nam.

---

## 2. Các Kỹ Thuật Prompting Cốt Lõi

### 2.1. Persona & Role Priming
Thiết lập Gemini đóng vai trò kép:
- **Nhà Nghiên Cứu Di Sản & Điển Chế Cổ Phục Việt Nam**: Nắm vững các thư tịch cổ như *Khâm Định Đại Nam Hội Điển Sự Lệ*, *Ngàn Năm Áo Mũ*, cùng truyền thống dệt thổ cẩm của 54 dân tộc.
- **Giám Đốc Sáng Tạo / Thời Trang Đương Đại (Contemporary Creative Director)**: Am hiểu ngôn ngữ thẩm mỹ Gen Z (Streetwear, Minimalism, Y2K, Techwear).

### 2.2. Semantic XML Delimitation
Toàn bộ system instruction và đầu vào được đóng gói trong các thẻ XML phân định rõ ràng để triệt tiêu hiện tượng Instruction Drift:
```xml
<system_instruction>
  <role>Cultural Heritage Stylist AI</role>
  <tri_layer_guardrail_protocol>
    <layer_1_structure>Bảo toàn 5 thân vạt áo, 5 khuy cài Ngũ Thường.</layer_1_structure>
    <layer_2_sacred>Cấm lạm dụng Long văn ngũ trảo, phẩm hàm hoàng tộc.</layer_2_sacred>
    <layer_3_contemporary>Khuyến khích mix-match phụ kiện văn minh, thanh lịch.</layer_3_contemporary>
  </tri_layer_guardrail_protocol>
</system_instruction>

<user_outfit_input>
  <!-- Payload dữ liệu 4 món đồ của người dùng -->
</user_outfit_input>
```

### 2.3. Zero-Tolerance Negative Constraints
Định nghĩa tường minh các giới hạn cấm kỵ:
- Không bao giờ cấp phép cho tà áo cổ phục bị cắt ngắn hở rốn thành croptop.
- Không bao giờ cho phép in ấn biểu tượng linh thiêng hoàng tộc vào không gian nhạy cảm (quán bar, vũ trường).
- Không chấp thuận trang phục cào rách, hở hang thiếu tôn nghiêm.

### 2.4. Few-Shot In-Context Calibration
Cung cấp các cặp mẫu chuẩn hóa:
- **Mẫu Approved (98đ)**: Áo Tấc xanh thiên thanh + Chân váy midi xếp ly + Hài thêu sen + Túi mây tre đan.
- **Mẫu Rejected (12đ)**: Áo Nhật Bình cắt croptop + Quần biker bó sát + Combat boots đinh tán.

---

## 3. Quy Trình Kiểm Thử & Tinh Chỉnh (Iterative Evaluation)

1. **Synthetic Stress-Testing**: Thử nghiệm với 50 kịch bản biên cố tình phá hoại văn hóa.
2. **Precision Benchmark**: Đo lường tỷ lệ chặn đứng vi phạm đạt 100%, tỷ lệ phê duyệt sáng tạo văn minh > 95%.
3. **Resilience & Fallback**: Khi kết nối API gặp sự cố, hệ thống chuyển giao liền mạch sang Heuristic Engine.
