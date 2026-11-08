# Mê Đá · Hệ thống Quản lý Lịch làm việc & Nhận ca Trực tuyến

Nền tảng SaaS quản lý lịch làm việc theo tuần, phân ca tự động công bằng, cảnh báo ca trống trực quan và nhận/đổi ca bổ sung 1-click theo thời gian thực dành cho đội ngũ **Mê Đá**.

## 🔗 Truy cập Trực tiếp (GitHub Pages)

- **Trang chủ**: [https://edrichtr.github.io/timetablemeda/](https://edrichtr.github.io/timetablemeda/)
- **Bảng điều phối chính (`medatime.html`)**: [https://edrichtr.github.io/timetablemeda/medatime.html](https://edrichtr.github.io/timetablemeda/medatime.html)

---

## ✨ Tính năng Vận hành Nổi bật

### 1. Công khai Lịch Không Rào cản & Điều phối Trực tiếp (Unconditional Admin Publishing)
- **Xuất bản Bất kỳ lúc nào (Zero Blockers)**: Quản trị viên có thể chuyển đổi linh hoạt giữa trạng thái `Bản nháp (Draft)` và `Đang công khai (Published)` bất cứ lúc nào — kể cả trước hạn chót đăng ký hoặc khi lịch còn các ô trống (`0` người đăng ký).
- **Tùy chỉnh Ô lịch Thời gian thực**: Bấm trực tiếp vào bất kỳ ca nào để gán nhân viên từ danh sách đăng ký (Dropdown / 1-Click Chips), nhập tên nhân sự mới, tự nhận ca hoặc đặt lại trạng thái trống ca.

### 2. Hệ thống Cảnh báo Ca trống Độ tương phản cao (High-Visibility Warning System)
- **Cảnh báo Trực quan Từng Ô (`⚠️ Trống ca / Chưa có người`)**: Các ca chưa có nhân sự được hiển thị với viền nét đứt cảnh báo (`1.5px dashed`), nền Amber/Red tinh tế, chấm tín hiệu nhấp nháy và nút kêu gọi hành động `+ Bấm để nhận ca ngay`.
- **Thanh Chỉ số Sức khỏe Lịch (`Schedule Health Summary Bar`)**: Thống kê thời gian thực **Tổng số ca (21)** | **Đã xếp người (Green Badge)** | **Trống ca / Cảnh báo (Amber/Red Badge)** kèm thanh tiến độ độ phủ phần trăm.

### 3. Nhận Ca Bổ Sung 1-Click & Đổi Ca Khẩn Cấp (`🔄 Cần người thay ca`)
- **Nhận Ca Bổ Sung Trực Tiếp**: Khi lịch đã công khai, nhân viên có thể bấm trực tiếp vào bất kỳ ô `⚠️ Trống ca` nào để nhận ca ngay lập tức (hỗ trợ cả chế độ **⚡ Nhận ca 1-Click**).
- **Tín hiệu Cần Người Thay Ca (`🔄 Cần người thay`)**: Nhân viên đã có lịch (hoặc Quản lý) có thể bật cờ tím nhấp nháy **`🔄 Cần người thay`** ngay trên ca của mình. Thành viên khác chỉ cần bấm vào ca đó để **Nhận thay ca trong 1 chạm**, tự động cập nhật cơ sở dữ liệu và ghi nhận vào lịch sử.

### 4. Bộ lọc "Ca Của Tôi" (My Shifts Filter) & Thống kê Khối lượng Công việc
- Thanh **Staff Filter Pills** ngay dưới thanh tổng quan hiển thị danh sách từng nhân sự kèm tổng số ca trong tuần (`[Tất cả (21)] [Hưng (5 ca)] [Linh (4 ca)]...`).
- Bấm vào tên nhân viên để làm nổi bật toàn bộ ca làm việc của người đó và làm mờ các ô không liên quan (`opacity: 0.22`), giúp xem lịch cá nhân cực nhanh trên điện thoại.

### 5. Xuất Ảnh Lịch Độ Phân Giải Cao (`📸 Xuất ảnh lịch`) & Nhật Ký Hoạt Động (`🕒 Lịch sử nhận/đổi ca`)
- **Xuất ảnh PNG 1-Click**: Tích hợp `html2canvas` giúp tải xuống ảnh chụp bảng lịch sắc nét (`scale: 2`) chỉ với 1 nút bấm để gửi nhanh vào nhóm Zalo / Messenger.
- **Lịch sử Nhận & Đổi ca**: Theo dõi chi tiết thời gian thực các lượt nhận ca bổ sung, báo cần người thay ca, nhận thay ca và công bố lịch.

---

## 🛠 Công nghệ Sử dụng
- **Frontend**: Vanilla HTML5, Modern CSS3 (Custom Properties, Sticky Matrix Grid, Dark/Light Theme), ES2022 Modules.
- **Realtime Database**: Firebase Cloud Firestore (`onSnapshot` đồng bộ tức thì đa thiết bị + bộ nhớ đệm Optimistic UI).
- **Typography & Export**: `Plus Jakarta Sans`, `Inter`, `Be Vietnam Pro`, `JetBrains Mono` & `html2canvas`.
