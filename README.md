# StartUpTech Desktop

Bản cài app Desktop của StartUpTech — một cửa sổ riêng mở bản web StartUpTech, đăng nhập bằng tài khoản
StartUpTech như trên web. Repo này chỉ chứa file cài (ở mục **Releases**), không chứa mã nguồn.

## Tải bản mới nhất

| Máy của bạn | Tải | Lần mở đầu tiên |
|---|---|---|
| Windows 10/11 (64-bit) | [**StartUpTech-Setup.exe**](https://github.com/ngphatdat1311/startuptech-desktop/releases/latest/download/StartUpTech-Setup.exe) | Nếu hiện "Windows protected your PC": bấm **More info → Run anyway** |
| macOS 12 trở lên — chip Apple (M1–M4) lẫn Intel | [**StartUpTech.dmg**](https://github.com/ngphatdat1311/startuptech-desktop/releases/latest/download/StartUpTech.dmg) | Kéo StartUpTech vào Applications, mở 1 lần (macOS sẽ chặn), rồi vào **Cài đặt hệ thống → Quyền riêng tư & Bảo mật → Vẫn mở** |
| Ubuntu / Debian (64-bit) | [**StartUpTech-Linux-amd64.deb**](https://github.com/ngphatdat1311/startuptech-desktop/releases/latest/download/StartUpTech-Linux-amd64.deb) | `cd ~/Downloads && sudo apt install ./StartUpTech-Linux-amd64.deb` |
| Linux khác (64-bit) | [**StartUpTech-Linux-x86_64.AppImage**](https://github.com/ngphatdat1311/startuptech-desktop/releases/latest/download/StartUpTech-Linux-x86_64.AppImage) | Cần FUSE 2 (Ubuntu 22.04+: `sudo apt install libfuse2t64`), rồi `chmod +x` file và mở |

Mọi phiên bản cùng mã SHA256 để kiểm tra file: [trang Releases](https://github.com/ngphatdat1311/startuptech-desktop/releases).

## Ghi chú

- **Chưa ký code** (không mua chứng chỉ Apple/Windows) nên hệ điều hành cảnh báo ở lần mở đầu — làm theo cột
  cuối là xong. Từ macOS 15, cách cũ "chuột phải → Open" không còn tác dụng.
- Mac báo **"StartUpTech bị hỏng"** (thường gặp với bản 1.0.0 cũ): mở Terminal, chạy
  `xattr -dr com.apple.quarantine /Applications/StartUpTech.app` rồi mở lại.
- **Cập nhật**: app tự nhắc khi có bản mới — tải về và cài đè lên bản cũ, đăng nhập vẫn giữ nguyên.
- Lần mở đầu sau một thời gian không ai dùng, app hiện "Đang kết nối máy chủ…" khoảng 1 phút — máy chủ miễn phí
  đang khởi động.

Các bản cài được build và phát hành tự động bằng GitHub Actions từ repo mã nguồn (private) của StartUpTech.
