# HeritageVibe AI — Dual-Engine System Architecture

## 1. Tổng Quan Kiến Trúc (Architecture Overview)

HeritageVibe AI được thiết kế theo mô hình **Hybrid Dual-Engine** độc đáo:
- **Client-Side SPA**: Độc lập, không phụ thuộc máy chủ trung gian, hoạt động 100% trên trình duyệt thông qua GitHub Pages.
- **Cognitive Cloud Layer**: Tích hợp trực tiếp Google Gemini 2.5 Flash qua endpoint REST API chính thức của Google Generative AI.
- **Fallback Heuristic Engine**: Đảm bảo trải nghiệm tức thì (Zero-Latency) ngay cả khi không có mạng hoặc chưa cấu hình API Key.

```
┌────────────────────────────────────────────────────────────────────────┐
│                        CLIENT APPLICATION LAYER                        │
│               (Tailwind CSS • Web Audio API • Canvas 2D)               │
├────────────────────────────────────────────────────────────────────────┤
│ • Interactive Mannequin Studio (SVG Vector Rendering Engine)           │
│ • Wardrobe Catalog (54 items: Triều Nguyễn, Lê, 54 Dân Tộc, Streetwear)│
│ • Five Elements Color Matrix (Thủy - Kim - Thổ - Thạch / Mộc - Hỏa)   │
└───────────────────┬────────────────────────────────┬───────────────────┘
                    │                                │
       [Chế độ có API Key]              [Chế độ mặc định Offline]
                    ▼                                ▼
┌──────────────────────────────────────┐ ┌───────────────────────────────┐
│     ĐỘNG CƠ 1: GEMINI LIVE API       │ │  ĐỘNG CƠ 2: HEURISTIC ENGINE  │
│  • Google Gemini 2.5 Flash           │ │  • Dynamic Mathematical Matrix│
│  • Endpoint: v1beta/models/...       │ │  • Violation Circuit Breaker  │
│  • CoT Cultural Reasoning            │ │  • Realtime 54-Item Weights   │
│  • Type-Safe Structured JSON         │ │  • Zero-Latency Client-Side   │
└───────────────────┬──────────────────┘ └───────────────┬───────────────┘
                    │                                    │
                    └─────────────────┬──────────────────┘
                                      ▼
┌────────────────────────────────────────────────────────────────────────┐
│                        REALTIME PRESENTATION LAYER                     │
│  • Circular Authenticity Gauge (80px Animated SVG)                     │
│  • Tri-Layer Cultural Guardrail Shield (APPROVED / REJECTED)          │
│  • Dual-Tone Web Audio Synthesizer (528Hz Bronze Bell / 180Hz Gong)   │
│  • Magazine Lookbook Exporter (1080x1350 Canvas HD)                    │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Động Cơ 1: Google Gemini 2.5 Flash Live API

### 2.1. Cấu hình Kết nối
- **Endpoint**: `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key={API_KEY}`
- **Phương thức**: `POST`
- **Headers**: `Content-Type: application/json`
- **Bảo mật**: API Key được lưu trữ cục bộ trong `localStorage` của trình duyệt người dùng, không bao giờ gửi về máy chủ bên thứ ba.

### 2.2. Structured Response Schema
Mô hình được cấu hình xuất dữ liệu dạng JSON tất định thông qua tham số `generationConfig.responseMimeType: "application/json"`.

---

## 3. Động Cơ 2: Gemini Heuristic Guardrail Engine

### 3.1. Công thức Toán học Điểm Toàn Vẹn (Dynamic Mathematical Formula)
Mỗi món đồ trong kho 54 items mang một chỉ số văn hóa cơ sở `layerScore` (từ 0 đến 100):

```math
\text{Integrity Score} = \text{round}\left( \frac{\text{Score}_{\text{Top}} + \text{Score}_{\text{Bottom}} + \text{Score}_{\text{Shoes}} + \text{Score}_{\text{Accessory}}}{4} \right)
```

### 3.2. Bộ Ngắt Mạch Vi Phạm (Violation Circuit Breaker)
Khi set đồ chứa bất kỳ item nào được đánh dấu cấm kỵ (ví dụ: Áo Croptop EDM, Quần Biker shorts, Quần rách):
- Điểm số lập tức bị phạt tụt xuống dải `12 – 15/100`.
- Kích hoạt âm thanh Chiêng Cảnh Báo 180Hz.
- Viền ma-nơ-canh chuyển sang nét đứt màu đỏ cảnh báo.
- Hiển thị 3 phương án chấn chỉnh văn hóa.

---

## 4. Hệ Thống Âm Thanh Di Sản (Web Audio API Synthesizer)
Hệ thống sử dụng trực tiếp Web Audio API không cần tải file audio ngoài:
- **Chuông Đồng Di Sản (528Hz)**: Tần số solfeggio cổ truyền, tạo cảm giác thanh tịnh khi set đồ đạt chuẩn.
- **Chiêng Cảnh Báo (180Hz)**: Âm hưởng chiêng lệnh cảnh báo khi phát hiện vi phạm quy cách lễ nghi.
