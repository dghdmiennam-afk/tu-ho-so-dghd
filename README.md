# Tủ hồ sơ Đấu giá Hợp danh Miền Nam · V7.0

Truy cập bản thử nghiệm: https://dghdmiennam-afk.github.io/tu-ho-so-dghd/

## Bố cục

- **Sơ đồ trái**: 6 tầng theo chiều vật lý từ **tầng 1 ở đáy đến tầng 6 ở trên cùng**, mỗi tầng 4 ngăn A–D, tổng 24 ngăn. Nhấp một ngăn để lọc danh sách và làm nổi bật vị trí.
- **Ô đỏ**: Rút · Điều chỉnh vị trí · Lưu trữ; Trả hồ sơ; Thêm hồ sơ; Thiết lập; Lưu · In; Nhật ký.
- **Ô xanh**: Xem trước tác vụ, xác nhận trước khi ghi, hướng dẫn trả lên đỉnh chồng và thông báo kết quả.

## Quy tắc lưu trữ

1. Mặc định **tối đa 20 hồ sơ/ngăn**, thay đổi được trong thẻ **Thiết lập**. Hệ thống ngăn giảm hạn mức xuống dưới số hồ sơ hiện có ở bất kỳ ngăn nào.
2. **Rút**: lưu người/nơi rút; hồ sơ rời chồng và những hồ sơ còn lại được đánh lại thứ tự.
3. **Trả**: trở về đúng ngăn gốc và đặt **trên cùng**, không trả về khe cũ.
4. **Lưu trữ**: chuyển hồ sơ trực tiếp vào ngăn còn chỗ ở **tầng 6** và cấp số `LT-0001`, `LT-0002`... Được phép lưu trữ hồ sơ đang rút mà không cần trả về vị trí cũ. Tầng 6 không nhận hồ sơ thường.
5. **Điều chỉnh**: mũi tên ↑ ↓ trên danh sách ô đỏ chỉ tạo bản xem trước; bắt buộc bấm **Xác nhận** trong ô xanh mới ghi dữ liệu và nhật ký.
6. **Thêm hồ sơ**: chế độ Mặc định ưu tiên hồ sơ cùng năm ở cạnh nhau, hoặc Chỉ định tầng/ngăn. Cấm thêm khi ngăn đã đầy hoặc khóa.
7. **Thiết lập**: xếp lại theo năm nhưng giữ nguyên ngăn khóa, hồ sơ đang rút và đã lưu trữ; khóa/mở khóa ngăn; chỉnh sức chứa; làm trống 24 ngăn có xác nhận đặc biệt. Làm trống không xóa danh mục hồ sơ và nhật ký.
8. **Lưu · In**: in toàn bộ vị trí/trạng thái trên A4 ngang; sao lưu/nhập JSON, xuất `index.html` có dữ liệu được nhúng.

## Dữ liệu và giới hạn bản thử nghiệm

- Danh mục ban đầu gồm **52 hồ sơ năm 2025–2026**, được bố trí thử nghiệm theo từng năm trên tầng 1–5; tầng 6 ban đầu trống.
- Trình duyệt sẽ cố gắng **chuyển dữ liệu V5/V6.1 đã lưu cục bộ** sang cấu trúc mới và giữ một bản sao dữ liệu cũ trong localStorage. Các hồ sơ đang ở tầng 6 theo hệ đánh số cũ không bị tự động cấp số LT.
- GitHub Pages **không có máy chủ lưu hồ sơ**, **không có phân quyền**, và **không đồng bộ giữa thiết bị**. Mọi thay đổi chỉ lưu ở localStorage trên từng trình duyệt. Bản in phản ánh dữ liệu của chính thiết bị đang dùng.
- Repository hiện **Public**: tên hồ sơ, tài sản và ngân hàng có trong mã nguồn công khai cho người có đường dẫn.
- Đây là bản thử nghiệm độc lập; chưa tích hợp hệ thống đấu giá chính, Node.js hay Cloud SQL.

## Triển khai

GitHub Pages dùng `main`, thư mục `/(root)`; có thể xem trạng thái tại [GitHub Actions](https://github.com/dghdmiennam-afk/tu-ho-so-dghd/actions). Nhánh sao lưu trước nâng cấp: `backup/pages-v6-1-before-v7-20261014`.
