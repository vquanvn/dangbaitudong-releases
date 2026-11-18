# Đăng Bài Tự Động — Phát hành

Kho công khai dành cho bộ cài Windows và thông tin phiên bản. Không lưu mã nguồn, dữ liệu chiến dịch hoặc phiên đăng nhập tại đây.

## Tải ứng dụng

Các bản đã phát hành nằm trong [Releases](https://github.com/vquanvn/dangbaitudong-releases/releases). Nếu chưa có bản phát hành, bộ cài chưa được tải lên.

## Quy trình phát hành

1. Tạo release với tag phiên bản, ví dụ `v1.0.7`.
2. Đính kèm `DangBaiTuDong-Setup-1.0.7.exe` và xuất bản release.
3. Kiểm tra đường dẫn tải bộ cài hoạt động.
4. Sau đó cập nhật `latest.json` tại nhánh `main` theo mẫu dưới đây.

```json
{
  "version": "1.0.7",
  "downloadUrl": "https://github.com/vquanvn/dangbaitudong-releases/releases/download/v1.0.7/DangBaiTuDong-Setup-1.0.7.exe",
  "notes": "Tùy chỉnh prompt viết bài trong ứng dụng và thông báo khi có phiên bản mới."
}
```

Ứng dụng từ bản 1.0.7 kiểm tra thông tin cập nhật khi mở và định kỳ 6 giờ. Khi có phiên bản mới, người dùng bấm thông báo để tải bộ cài và tự cài đặt. Chưa hỗ trợ tự động cài đặt nền. Không công bố `latest.json` trước khi bộ cài tương ứng tải được.
