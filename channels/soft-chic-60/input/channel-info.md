# Soft Chic 60+

## Trạng thái
Đang cải tiến — kênh đã hoạt động, đang trong quá trình sửa lỗi và tối ưu lại theo dữ liệu nghiên cứu.

## Thông tin kênh
- **Handle:** @SoftChic60
- **Link:** https://www.youtube.com/@SoftChic60/videos
- **Mô tả (tự giới thiệu):** "Soft Chic 60+ – Timeless Style, Confidence & Joy After 60. Welcome to Soft Chic 60+, where we celebrate beauty, confidence, and elegance at every age – especially after 60. Here, you'll find chic fashion tips, beauty advice, wellness inspiration, and lifestyle ideas to help you embrace your golden years with style and purpose."
- **Ngách:** Thời trang phụ nữ Mỹ 60+ (trong ngách rộng hơn 40+/50+/60+)
- **Thị trường mục tiêu:** Mỹ (US), view Mỹ là chính
- **Phương thức sản xuất:** Video AI (ảnh AI-generate + giọng đọc TTS), không phải người thật quay
- **Phong cách thương hiệu:** "Soft chic" — thanh lịch nhẹ nhàng, tông màu ấm/pastel, không quá gắt

## Tóm tắt chẩn đoán (2026-09-03)
- 1.600 subscriber, 60 video, view/ngày trung bình chỉ ~10 — chậm hơn benchmark kênh nhỏ cùng ngách khoảng 2.000 lần.
- Nguyên nhân chính: (1) đứt quãng đăng bài ~8 tháng (2025-09 → 2026-06) làm mất momentum thuật toán, (2) thumbnail dùng ảnh AI phong cách "đi bộ trên phố châu Âu" chung chung, không theo đúng template đã kiểm chứng hiệu quả trong ngách.
- Đã tìm được 2 kênh cùng phong cách sản xuất AI đang thắng đậm để làm chuẩn tham khảo: Chic After 60 (@chicafter60) và Golden Melanin Lifestyle (@goldenmelaninlifestyle) — xem `_shared/reference-channels/`.
- Kết luận: AI không phải rào cản trong ngách này — vấn đề là tính nhất quán khi đăng bài + độ chỉn chu khi thực thi đúng công thức (thumbnail, kịch bản sâu, CTA nhúng giữa video).

## Nội dung thư mục `output/` của kênh này
- `target-channel-softchic60.json` — dữ liệu đầy đủ 60 video hiện tại (view, engagement, ngày đăng...).
- `softchic60-content-plan.xlsx` — file kế hoạch đầy đủ: chẩn đoán, so sánh benchmark, quick-win sửa video cũ, kế hoạch sản xuất mới 2 video/tuần, 5 kênh tham khảo, phân tích sâu 2 kênh AI cùng phong cách.
- `scripts-txt/` — kịch bản đầy đủ (theo template 2 giai đoạn) + 100 prompt tạo hình cho video đầu tiên "7 Sweater Mistakes...".
- `thumbnails/softchic60/` — mẫu thumbnail hiện tại của kênh (dùng để chẩn đoán).

## Việc cần làm tiếp
- Áp dụng 5 quick-win sửa tiêu đề/thumbnail cho video cũ.
- Sản xuất 8 video mới theo kế hoạch 4 tuần (2 video/tuần) trong file xlsx.
- Sau 2-3 tuần, chạy lại `analyze-target-channel.js @SoftChic60` để đối chiếu kết quả với baseline.
- Viết kịch bản + prompt hình cho 7 video còn lại trong kế hoạch, theo đúng quy trình đã dùng cho video 1.
