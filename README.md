# Mule Hazard Map iOS Starter

Source SwiftUI khởi đầu để đồng bộ dữ liệu website Mule Hazard Map qua REST API.

## Cách test nhanh trên Mac

1. Cài **Xcode** từ Mac App Store.
2. Mở Xcode → File → New → Project → iOS → App.
3. Product Name: `MuleHazardMap`.
4. Interface: SwiftUI, Language: Swift.
5. Kéo các thư mục `App`, `Models`, `Services`, `Views`, `Config` vào project.
6. Copy `Config/Config.sample.xcconfig` thành `Config/Config.xcconfig`.
7. Điền:
   - `MHM_API_BASE_URL`
   - `GOONG_API_KEY`
   - `PRODUCT_BUNDLE_IDENTIFIER`
8. Trong Project Settings → Info, dùng `Config/Info.plist` hoặc copy các key permission sang Info tab.
9. Chạy bằng iPhone Simulator hoặc cắm iPhone thật và bấm Run.

## API website app đang kỳ vọng

- `POST /mobile/login`
- `GET /mobile/sync?since=...`
- `POST /checkins`

Base URL ví dụ: `https://domain.com/wp-json/mhm/v1`.

## Test trên iPhone thật

- Cần Mac + Xcode.
- Cần Apple ID đăng nhập trong Xcode.
- Cắm iPhone qua USB hoặc Wi-Fi debugging.
- Chọn thiết bị iPhone → Run.

## Test cho nhiều người

- Đẩy code lên GitHub private repo.
- Dùng Apple Developer Program để upload TestFlight.
- Người test cài app qua TestFlight.
