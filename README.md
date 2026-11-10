# Spotify QR – tự dừng tại 02:30

## Nội dung
- `index.html`: trang GitHub Pages nhúng Spotify track `4SgWyon9zERpSobzDnbaY0`.
- Trang theo dõi `playback_update` từ Spotify iFrame API và gọi `pause()` khi vị trí phát đạt 150.000 ms.

## Đưa lên GitHub Pages
1. Tạo một repository GitHub mới, ví dụ `spotify-qr`.
2. Tải `index.html` lên thư mục gốc của repository.
3. Vào **Settings → Pages**.
4. Ở **Build and deployment**, chọn **Deploy from a branch**.
5. Chọn branch `main`, folder `/ (root)`, rồi Save.
6. Chờ GitHub cấp URL dạng `https://TEN-GITHUB.github.io/spotify-qr/`.
7. Dùng URL đó để tạo QR cuối cùng.

## Lưu ý quan trọng
- Người nghe cần bấm nút Play trong Spotify Embed; trình duyệt thường chặn tự phát âm thanh khi chưa có thao tác người dùng.
- Spotify có thể yêu cầu đăng nhập hoặc giới hạn nghe tùy tài khoản, quốc gia và track. GitHub Pages không thể bỏ qua xác thực của Spotify.
- Bộ đếm dừng dựa trên vị trí phát mà Spotify iFrame API báo về. Hãy thử trên điện thoại thực tế sau khi deploy.
- Mã QR cuối cùng phải trỏ đến URL GitHub Pages đã được deploy, không phải link Spotify trực tiếp.
