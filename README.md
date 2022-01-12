# V2Ray Heroku

**Để triển khai V2Ray VLESS, hãy chuyển đến (https://github.com/VietNamDVB/v2ray-heroku). **

## Tổng quan

Dự án này được sử dụng để triển khai V2Ray WebSocket trên Heroku, trong phạm vi sử dụng hợp lý, hình ảnh này sẽ không bị cấm do lượng tài nguyên lớn.

Sau khi được triển khai, V2Ray sẽ luôn chạy với phiên bản mới nhất mỗi khi ứng dụng được khởi chạy

## Triển khai

### Bước
 1. Chuyển dự án này vào tài khoản GitHub của riêng bạn (tên người dùng là `example`)
 2. Sửa đổi tên dự án, hãy cẩn thận không bao gồm các từ khóa `v2ray` và` heroku` (tên dự án đã sửa đổi lấy `demo` làm ví dụ)
 3. Sửa đổi `README.md`, thay thế` bclswl0827 / v2ray-heroku` bằng nội dung của riêng bạn (chẳng hạn như `example / demo`)

> [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/VietNamDVB/v2ray-heroku)

4. Quay lại trang chủ của dự án và nhấp vào liên kết ở trên để triển khai V2Ray

### Biến đổi

| Đối số | Mặc định | Diễn giải |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess user ID |
| `AID` | `64` | AlterID，Số từ 0 đến 65535 |
| `WSPATH` | `/` | WebSocket  HTTP |

## Truy cập vào CloudFlare

Hai phương pháp sau có thể kết nối ứng dụng với CloudFlare, có thể cải thiện tốc độ ở một mức độ nhất định.

 1. Liên kết tên miền với ứng dụng và kết nối tên miền với CloudFlare
 2. Reverse proxy thông qua CloudFlare worker

## Để ý

 1. ** Đừng lạm dụng dự án này, có rất ít dịch vụ miễn phí như Heroku, hãy sử dụng và trân trọng **
 2. Nếu sử dụng tên miền để truy cập CloudFlare, vui lòng xem xét bật TLS 1.3
 3. Hầu hết các địa chỉ AWS IPv4 đều bị Twitter chặn
