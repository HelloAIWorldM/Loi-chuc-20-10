# Google Stitch Design System Blueprint: 20/10 • Tri Ân Mẹ Yêu ✨

> **Dự án**: Website Chúc Mừng Ngày Phụ Nữ Việt Nam 20/10 Dành Cho Mẹ  
> **Phương pháp luận**: Google Stitch "Vibe Design" & Anti-AI-Slop Editorial Craft  
> **Thư mục triển khai**: `Chucme2010/`

---

## 1. Triết lý Thiết kế (Design Philosophy)

- **Cảm xúc chủ đạo**: Ấm áp, thiêng liêng, trang nhã, biết ơn sâu sắc (Mẫu tử tình thâm).
- **Loại bỏ**: Mọi yếu tố liên quan đến bang hội game, Discord, xưng hô tỷ muội/huynh đệ.
- **Tập trung**: Tôn vinh hình ảnh người Mẹ — bến đỗ bình an của cuộc đời, tình yêu thương vô bờ bến và những hy sinh thầm lặng.
- **Tiêu chuẩn Stitch**:
  - Không dùng các layout cẩu thả hay màu neon chói gắt.
  - Sử dụng hệ lưới Bento Box thanh lịch với viền phát sáng đa tầng (Multi-layered Obsidian Glow).
  - Trải nghiệm tương tác xúc giác: Lau lớp sương ấm mờ ảo trên kính để hé lộ bức tâm thư và kích hoạt pháo hoa trái tim rực rỡ.

---

## 2. Bảng Màu & Visual Tokens (Color Hierarchy)

Tuân thủ nguyên tắc cân bằng thị giác 60-30-10:

| Token | Giá trị Hex / RGBA | Vai trò & Ý nghĩa |
|---|---|---|
| `--noir-deep` | `#08020a` | Nền đêm huyền bí, tạo chiều sâu cho ánh sáng |
| `--noir-surface` | `#14051a` | Bề mặt nền chuyển sắc cực quang ấm |
| `--noir-card` | `rgba(24, 7, 28, 0.78)` | Kính mờ Bento Obsidian Glass |
| `--gold-champagne`| `#f5d596` | Màu vàng kim ánh trăng quý phái |
| `--gold-glow` | `rgba(245, 213, 150, 0.45)` | Ánh hào quang ấm áp bao bọc lời chúc |
| `--rose-maternal` | `#e8437f` | Sắc hoa mẫu đơn & hoa hồng biểu trưng tình mẹ |
| `--rose-glow` | `rgba(232, 67, 127, 0.38)` | Vầng hào quang tỏa dịu dàng |
| `--silk-warm` | `#fffaf2` | Màu lụa trắng kem cho typography chính |
| `--text-body` | `#f0e3f5` | Chữ đọc dễ chịu, tương phản đạt chuẩn WCAG AAA |

---

## 3. Hệ Thống Typography (Stitch Editorial Scale)

1. **Display & Numbers**: `'Cinzel', serif` (Weights 600, 700, 800) — Số "20 · 10" và huy hiệu vinh danh.
2. **Tiêu đề cảm xúc**: `'Playfair Display', serif` (Italic 600, Bold 800) — Tiêu đề "Tri Ân Mẹ Yêu", "Bến Đỗ Bình An".
3. **Thư pháp & Tên gọi**: `'Dancing Script', cursive` (Semi-bold 700) — "Gửi Mẹ Yêu Dấu Của Con 🌸".
4. **Văn bản nội dung**: `'Montserrat', sans-serif` (300, 400, 500, 600) — Đọc rõ trên mọi màn hình di động Retina và màn hình 4K.

---

## 4. Kiến Trúc Thành Phần Giao Diện (Component Architecture)

```
[BODY - Nền Cực Quang Mẫu Tử (Maternal Warm Aurora)]
 ├── [Canvas Pháo Hoa Trái Tim & Bụi Sao (Fireworks Engine)]
 ├── [MAIN #stage]
 │    ├── <header class="master-header">
 │    │    ├── Badge: VIETNAMESE WOMEN'S DAY • 20.10
 │    │    ├── H1: 20 · 10 (Chuyển sắc vàng kim - hồng thược dược)
 │    │    └── Subtitle: "Tri Ân Người Phụ Nữ Tuyệt Vời Nhất Của Con"
 │    │
 │    ├── <div class="artwork-stage"> (Centerpiece SVG)
 │    │    ├── Vòng hào quang đa lớp thở nhịp nhàng (Breathe animation)
 │    │    └── SVG Độc Bản: Đóa Mẫu Đơn Kim Liên & Trái Tim Phát Sáng
 │    │
 │    ├── <div id="wishesGrid"> (Curated Wish Cards)
 │    │    ├── 6 Thẻ lời chúc dát vàng (Desktop bố trí 2 bên, Mobile chạy Marquee mượt mà)
 │    │    │    • Bình an một đời • Nụ cười luôn nở
 │    │    │    • Sức khỏe dồi dào • An nhiên tự tại
 │    │    │    • Mẹ là bầu trời • Là điểm tựa bình yên
 │    │    │    • Trẻ mãi không già • Vạn sự như ý
 │    │    │    • Cả đời vì con • Nay hãy vì chính mẹ
 │    │    │    • Tình mẹ bao la • Đong đầy yêu thương
 │    │
 │    └── <section class="letter-bento" id="letterCard">
 │         ├── Con dấu sơn son dát vàng: "MẪU TÂM • TRI ÂN MẸ"
 │         ├── Tiêu đề: "Gửi Mẹ Yêu Dấu Của Con 🌸"
 │         ├── Nội dung bức tâm thư hiếu nghĩa cảm động
 │         ├── Chữ ký: "Mãi yêu Mẹ • Đứa con bé bỏng của Mẹ"
 │         └── Nhóm nút bấm:
 │              ├── [Lau Lại Kính ❄️]
 │              ├── [Thả Tim Tri Ân ❤️]
 │              └── [Chép Lời Chúc 📋]
 │
 ├── [DIV #fogWrapper] (Lớp sương kính tương tác)
 │    ├── <canvas id="fogCanvas"> (Mô phỏng sương đọng nước chân thực)
 │    └── Lời nhắc: "Kính mờ sương ấm... chạm gạt để mở lời chúc gửi Mẹ ✨"
 │
 ├── [BUTTON #btnAudio] (Điều khiển âm nhạc du dương)
 └── [DIV #toast] (Thông báo phản hồi tức thì)
```

---

## 5. Kịch Bản Tương Tác & Hiệu Năng (Interaction & Performance)

1. **Hiệu ứng lau sương (Fog Wipe)**:
   - Sử dụng cọ Radial Gradient mềm mại, nội dung tẩy bằng `destination-out`.
   - Thuật toán nội suy bước gạt (interpolation) tránh hiện tượng đứt nét khi vuốt nhanh trên iPhone/Android.
   - Khi diện tích lau đạt 45% -> Kính tự động tan biến trong hiệu ứng mượt mà và khai mở tràng pháo hoa trái tim 3 cụm liên tiếp.

2. **Auto-Fireworks Heart Engine**:
   - Tọa độ tạo hình trái tim dựa trên phương trình tham số:
     $$x = 16 \sin^3(t), \quad y = -(13 \cos(t) - 5 \cos(2t) - 2 \cos(3t) - \cos(4t))$$
   - Tia lửa có vệt đuôi tàn (trail history) và tâm sáng nhấp nháy.
   - Điều tiết chu kỳ bắn 3.8s - 5s luân phiên 3 vùng trời, trần số lượng hạt giới hạn để bảo đảm 60 FPS chuẩn.

3. **Responsive Mobile 100%**:
   - Sử dụng CSS Marquee tăng tốc phần cứng (`transform: translate3d`) cho thẻ lời chúc trên màn hình nhỏ, tuyệt đối không giật lag.
   - Tương thích notch tai thỏ `env(safe-area-inset-*)` trên iOS.
