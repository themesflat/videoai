# videoai

Dữ liệu nghiên cứu & sản xuất nội dung YouTube cho nhiều kênh thời trang phụ nữ lớn tuổi (thị trường Mỹ, video AI).

## Cấu trúc thư mục

```
channels/                      # Mỗi kênh 1 folder riêng
  <ten-kenh>/
    input/
      channel-info.md          # Mô tả kênh: ngách, đối tượng, thị trường, phong cách thương hiệu, trạng thái
    output/                    # Toàn bộ dữ liệu nghiên cứu + sản xuất riêng cho kênh này
      target-channel-*.json    # Dữ liệu video hiện tại của kênh (nếu đã hoạt động)
      *-content-plan.xlsx      # Chẩn đoán + kế hoạch sản xuất
      scripts-txt/             # Kịch bản đầy đủ + prompt tạo hình từng video
      thumbnails/               # Ảnh thumbnail mẫu để đối chiếu

_shared/                       # Dữ liệu dùng chung cho nhiều kênh
  niche-research/               # Nghiên cứu tổng quan ngách (206 video / 121 kênh, công thức chung)
  reference-channels/           # Dữ liệu kênh đối thủ/tham khảo (vd Chic After 60, Golden Melanin Lifestyle)
  templates/                    # Template lệnh viết content (2 giai đoạn) và lệnh tạo hình ảnh
```

## Danh sách kênh hiện tại
1. **Soft Chic 60+** (`channels/soft-chic-60/`) — kênh đang hoạt động, đang trong quá trình cải tiến.
2. **Trendy & Timeless** (`channels/trendy-and-timeless/`) — kênh mới, chuẩn bị làm, đang chờ điền thông tin mô tả.
3. **Viva Estilo** (`channels/viva-estilo/`) — kênh đang hoạt động, thời trang phụ nữ **tiếng Tây Ban Nha** 50+/60+/70+. Nội dung/tiêu đề viết bằng tiếng Tây Ban Nha. Nghiên cứu đối chiếu chỉ giới hạn khán giả tiếng Anh + tiếng Tây Ban Nha. Xuất Excel: chỉ khi người dùng ra lệnh, mỗi tuần 2 tiêu đề.

Khi thêm kênh mới: tạo folder `channels/<ten-kenh-viet-thuong-khong-dau>/input/channel-info.md`, điền mô tả kênh, rồi bắt đầu nghiên cứu — dữ liệu đầu ra sẽ lưu vào `channels/<ten-kenh>/output/`.
