# Quy tắc nghiên cứu kênh đối thủ / kênh tham khảo

Áp dụng cho mọi lần chọn kênh đối thủ để phân tích công thức (tiêu đề, thumbnail, kịch bản), cho tất cả các kênh trong `channels/`.

## Quy tắc bắt buộc

1. **Chỉ nghiên cứu kênh đang "sống"** — nghĩa là kênh đăng video đều đặn gần đây, không bị bỏ hoang.
   - Kiểm tra ngày đăng video gần nhất: nếu quá **60 ngày** không đăng video mới, coi như kênh đã ngừng hoạt động → loại khỏi danh sách tham khảo.
   - Kiểm tra nhịp đăng trong 2-3 tháng gần nhất: cần có nhiều video, không có khoảng trống dài (giống lỗi mà chính Soft Chic 60+ từng mắc phải và bị thuật toán "phạt").

2. **Lấy video GẦN ĐÂY có view cao để phân tích, không lấy video cũ ăn may.**
   - Ưu tiên video đăng trong **90 ngày gần nhất** có view/ngày tốt, thay vì chỉ nhìn "video có tổng view cao nhất mọi thời đại" — vì 1 video viral cũ có thể là may mắn nhất thời, không còn phản ánh đúng công thức/thuật toán hiện tại của kênh.
   - Video cũ viral (nếu có) chỉ nên ghi nhận như 1 điểm dữ liệu tham khảo phụ, không dùng làm nền tảng chính để rút công thức.

## Vì sao có quy tắc này
Chính kênh Soft Chic 60+ từng có 1 video viral (65K view) vào tháng đầu tiên, sau đó ngừng đăng ~8 tháng và các video sau đó chỉ đạt 25-200 view. Nếu chỉ nhìn vào con số tổng/video đỉnh mà không kiểm tra kênh còn hoạt động đều hay không, sẽ dễ chọn nhầm kênh "đã chết" hoặc công thức "đã hết hạn" làm chuẩn tham khảo.

## Cách áp dụng khi chạy script
Khi chạy `node scripts/analyze-target-channel.js @handle [channel-slug]` để kéo dữ liệu 1 kênh đối thủ:
- Xem cột `publishedAt` gần nhất trong file JSON kết quả — nếu cách ngày hôm nay hơn 60 ngày, loại kênh này.
- Khi rút "công thức thắng" (tiêu đề, thumbnail, kịch bản), ưu tiên lọc theo `daysSincePublish <= 90` rồi mới sắp xếp theo `viewsPerDay`.
