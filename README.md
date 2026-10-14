# Bản đồ tủ hồ sơ — Đấu giá Hợp danh Miền Nam

Ứng dụng web tĩnh để tìm vị trí hồ sơ lưu trữ vật lý trên tủ 24 ngăn, mô phỏng chồng hồ sơ từ dưới lên và thao tác rút/trả túi hồ sơ.

## Sử dụng

Sau khi bật GitHub Pages, địa chỉ truy cập là:

https://dghdmiennam-afk.github.io/tu-ho-so-dghd/

**Bật GitHub Pages:** mở [Settings → Pages](https://github.com/dghdmiennam-afk/tu-ho-so-dghd/settings/pages), trong **Build and deployment**, chọn **Deploy from a branch**, Branch **main**, thư mục **/(root)**, rồi **Save**. Đợi GitHub hiển thị thông báo trang đã triển khai trước khi truy cập.

## Dữ liệu và giới hạn

- `index.html` có dữ liệu danh mục hồ sơ được nhúng sẵn. Do repository đang **Public**, bất kỳ ai cũng có thể đọc được nội dung tệp và dữ liệu ban đầu.
- Các thao tác trên website lưu vào **localStorage của chính trình duyệt**. Điện thoại và máy tính **không tự đồng bộ**; reload cùng trình duyệt vẫn giữ bản đã sửa.
- Khi cần đưa vị trí cập nhật vào mã nguồn để các thiết bị tải bản mặc định mới, dùng nút **Tải index.html mới (Up GitHub)** và cập nhật lại tệp trong repository. Các thiết bị đã có bản lưu localStorage cũ sẽ tiếp tục dùng bản cũ cho đến khi xóa dữ liệu lưu cục bộ của site.
- Nút **JSON** xuất bản sao dữ liệu để sao lưu.
- Chưa tích hợp xác thực tài khoản, cơ sở dữ liệu hoặc Google Sheets; đây là bản thử nghiệm giao diện độc lập, không liên quan hệ thống đấu giá đang vận hành.
