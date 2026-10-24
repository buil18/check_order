# Lịch sử thay đổi

## Chưa phát hành
- Dự kiến: thêm loại đơn ST, tìm cả SO/S5/S6 bằng một chức năng trên JDE, tra cứu SAP theo nhiều ô.

## 1.0 – bản hiện tại
- Quy tắc trạng thái: thêm Last Status 900 vào nhóm "đã xác nhận" (đơn 900 → 999).
- Hộp thư: nút **Xóa** từng đơn và **Xóa tất cả**. Bookmark GR và JDE gửi lại được sau khi xóa.
- SAP Fetch: chỉ tự lấy đơn mới. Không quét lại đơn cũ khi bật lại bookmark. Mỗi đơn thử một lần, SAP không có dữ liệu thì dừng, lấy lại bằng nút **lấy lại**.
- JDE Capture: tự điền mã đơn vào ô Order Number, tự bấm Find, lấy danh sách đơn từ clipboard, có nút **Dừng tự động**.
- Hộp thư tự động (Apps Script) nối 3 bookmark. JDE chặn nhận dữ liệu nên JDE gửi bằng biểu mẫu ẩn.
- Quy tắc đã xác nhận: Last 574 hoặc 620, hoặc Next 620 (574→620, 912→620, 620→999).
- Quy tắc chờ SUP xác nhận: Next 545.
- Nút **Đối soát lại** trên dữ liệu lần copy gần nhất.
- Bảng thời gian: đếm số lần copy, dán và thời gian từng bước.
- Font hệ thống tự nhiên, chữ in chìm "Logistics Hoc Mon – Designed by Tien Loi".
- Nguồn glassRUN khi không có JDE, chặn nếu dòng thiếu số lượng.
