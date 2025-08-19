# shadowB

> Ứng dụng luyện tập tại nhà dạng **một file HTML**, mở là dùng. Không cần cài đặt, dữ liệu lưu **trên máy của bạn**.

---

## 1) Dùng ngay (3 bước)

1. **Mở file** `HomeFit_web_….html` bằng Chrome/Edge/Brave/Cốc Cốc/Firefox/Safari.
2. Vào **Kế hoạch** → chọn 1 gói (Beginner/Fatburn/Mobility/Beauty…) hoặc tự tạo.
3. Bấm **Tập ngay** (hoặc **Ctrl/⌘+K** gõ `Tập` → Enter).

> Mẹo: Trên **Kế hoạch**, bấm **Xuất .ics** để đưa lịch tập vào Google/Apple Calendar.

---

## 2) Điều khiển quan trọng

* **Command Palette**: **Ctrl/⌘+K** → gõ tên trang (*Trang chủ, Tập, Kế hoạch, Thư viện, Cài đặt…*) hoặc lệnh (*Focus Mode, Timer, Xuất .ics*).
* **Phím tắt khi tập**:

  * `Space` phát/tạm dừng • `N` kế tiếp • `P` lùi lại
  * `F` bật/tắt **Focus Mode** (màn hình tối, ít nhiễu)
  * `T` mở **HIIT Timer** (beep + giọng đọc)
  * `↑/↓` tăng/giảm âm lượng thông báo
* **Sticky CTA**: thanh **Tập ngay** nổi ở đầu trang Home/Workout.

---

## 3) Lịch & nhắc tập

* **Xuất toàn bộ lịch**: **Kế hoạch → Xuất .ics** (mặc định 19:00–19:45 mỗi ngày).
* **Thêm từng ngày**: nút **GCal** ngay trên mỗi ô ngày.
* **Đổi giờ mặc định**: trong mã `exportPlanICS()` (tìm `19:00`/`19:45`).

---

## 4) Thư viện & Kế hoạch

* **Thư viện**: ô tìm kiếm → gõ là lọc theo tên/nhóm cơ.
* **Kế hoạch**: lịch được **gom theo tuần** (nếu phần tử ngày có `data-date`) để đỡ dài.
* **Tự tạo plan**: dùng Plan Builder (Beta) hoặc thêm/sửa trong `PLAN_TEMPLATES`.

---

## 5) Dữ liệu & riêng tư

* Lưu tại **localStorage** của trình duyệt; không gửi lên server.
* **Cài đặt** cho phép bật/tắt dark mode, beep/giọng đọc, **Reset** để xóa dữ liệu.

---

## 6) Sự cố thường gặp (cách xử lý nhanh)

* **Ctrl/⌘+K không chuyển trang** → dùng bản đã fix (pro\_fix/cleanpalette). Nếu đã đổi nhãn menu, cập nhật lại nhãn.
* **Không nghe beep/TTS** → bật trong Timer; tăng âm lượng; trên iOS chạm 1 lần để kích hoạt âm.
* **Không mở được `.ics`** → tải file rồi mở bằng Calendar (trên iOS mở trong app Lịch).
* **Video lỗi** → dùng nút *Mở trên YouTube*; kiểm tra mạng.
* **Mất dữ liệu** → do xóa cache. Sắp có **Export/Import JSON** (roadmap).

---

## 7) Tùy chỉnh nhanh (phổ biến)

* **Giờ luyện tập** (toàn bộ): sửa trong `exportPlanICS()`.
* **Nhãn menu**: chỉnh ở `Header/BottomNav` (nếu bạn muốn đổi từ “Kế hoạch” → “Plan”…).
* **Giao diện**: thay màu/bo góc trong khối CSS `clean-ui-patch` và `pro-upgrades-v1-css`.

---

## 8) Tóm tắt tính năng

* **Command Palette** (Ctrl/⌘+K), **phím tắt**, **Focus Mode**.
* **HIIT Timer** có **beep + giọng đọc**, chỉnh work/rest/rounds.
* **Kế hoạch** gom theo tuần, **Xuất `.ics`** + nút **GCal** từng ngày.
* **Thư viện** có tìm kiếm nhanh, **Sticky CTA** trên Home/Workout.
* **Dữ liệu cục bộ**, **không** backend.

---

## 9) Ghi chú an toàn

* Đây **không** thay thế tư vấn y khoa. Ngừng tập nếu đau/chóng mặt.
* Face yoga/massage dùng **lực nhẹ**; vacuum thực hiện khi bụng rỗng và trong ngưỡng an toàn.

> **Xong.** Nếu cần thêm: PWA offline, Export/Import JSON, reschedule thông minh — báo mình bật tiếp.
