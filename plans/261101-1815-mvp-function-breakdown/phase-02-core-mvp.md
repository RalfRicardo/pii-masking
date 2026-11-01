---
title: "Phase 2: Core product MVP"
status: todo
---

# Core product MVP

## Phạm vi

Mốc P2; xem lịch và hợp đồng trong [Function breakdown](./function-breakdown.md).

## Công việc

- [ ] FE-01 — Đăng nhập và đăng xuất (owner SE1, reviewer CS2).
- [ ] FE-02 — Tải PDF lên (owner SE1, reviewer SE2).
- [ ] FE-03 — Danh sách tài liệu và tác vụ (owner SE1, reviewer SE2).
- [ ] FE-04 — Hiển thị tiến trình và lỗi theo trang (owner SE1, reviewer SE2).
- [ ] FE-05 — PDF viewer (owner SE1, reviewer SE3).
- [ ] FE-06 — Overlay vùng PII (owner SE1, reviewer SE3).
- [ ] FE-07 — Danh sách và lọc kết quả PII (owner SE1, reviewer SE2).
- [ ] FE-08 — Duyệt gợi ý (owner SE1, reviewer SE2).
- [ ] FE-09 — Khoanh vùng thủ công (owner SE1, reviewer SE3).
- [ ] FE-10 — Xác nhận duyệt tài liệu (owner SE1, reviewer SE2).
- [ ] FE-11 — Xuất và tải kết quả (owner SE1, reviewer CS2).
- [ ] FE-12 — Xóa tài liệu (owner SE1, reviewer CS2).
- [ ] BE-01 — Quản lý tài khoản demo (owner SE2, reviewer CS1).
- [ ] BE-02 — Quản lý phiên truy cập (owner SE2, reviewer CS1).
- [ ] BE-03 — Phân quyền tài liệu và artifact (owner CS1, reviewer CS2).
- [ ] BE-04 — Tiếp nhận và kiểm tra PDF (owner SE2, reviewer CS1).
- [ ] BE-05 — Lưu và truy xuất tài liệu (owner SE2, reviewer CS1).
- [ ] BE-06 — Điều phối pipeline (owner SE2, reviewer CS1).
- [ ] BE-07 — Thử lại và chống tác vụ trùng (owner SE2, reviewer CS1).
- [ ] BE-08 — Lưu và đọc quyết định duyệt (owner SE2, reviewer CS1).
- [ ] BE-09 — Khóa snapshot đã duyệt (owner SE2, reviewer CS1).
- [ ] BE-10 — Điều phối xuất và tải an toàn (owner SE2, reviewer CS1).
- [ ] BE-11 — Vòng đời và xóa dữ liệu (owner SE2, reviewer CS1).
- [ ] BE-12 — Nhật ký xử lý (owner CS1, reviewer CS2).
- [ ] OCR-01 — Kiểm tra và phân loại trang (owner SE3, reviewer SE4).
- [ ] OCR-02 — Trích xuất văn bản native (owner SE3, reviewer CS2).
- [ ] OCR-03 — Render và tiền xử lý OCR (owner SE3, reviewer SE4).
- [ ] OCR-04 — Nhận dạng chữ in tiếng Anh (owner SE3, reviewer CS2).
- [ ] OCR-05 — Chuẩn hóa văn bản cho ML (owner SE3, reviewer ML1).
- [ ] OCR-06 — Khôi phục thứ tự đọc (owner SE3, reviewer CS2).
- [ ] OCR-07 — Chuẩn hóa tọa độ PDF (owner SE3, reviewer SE4).
- [ ] OCR-08 — Đánh giá chất lượng trang (owner SE3, reviewer ML1).
- [ ] OCR-09 — Hợp nhất native và OCR (owner SE3, reviewer SE4).
- [ ] DATA-04 — Bộ tài liệu PDF chuẩn (owner SE4, reviewer SE3).
- [ ] DATA-05 — Bộ ca redaction đối kháng (owner CS2, reviewer CS1).
- [ ] ML-01 — Baseline có thể tái lập (owner ML1, reviewer SE4).
- [ ] ML-02 — Chuẩn bị dữ liệu huấn luyện (owner ML1, reviewer SE4).
- [ ] ML-03 — Suy luận phát hiện PII (owner SE2, reviewer ML1).
- [ ] ML-04 — Luật bổ trợ theo chính sách (owner SE4, reviewer ML1).
- [ ] ML-05 — Fine-tune và quản lý checkpoint (owner ML1, reviewer SE4).
- [ ] ML-06 — Kết hợp ML và luật (owner SE4, reviewer ML1).
- [ ] ML-08 — Ánh xạ entity thành vùng (owner SE3, reviewer SE1).
- [ ] RED-01 — Kiểm tra snapshot và vùng xóa (owner CS1, reviewer CS2).
- [ ] RED-02 — Hợp nhất vùng và padding (owner CS1, reviewer CS2).
- [ ] RED-03 — Redaction nội dung native (owner SE4, reviewer CS2).
- [ ] RED-04 — Redaction ảnh và lớp OCR (owner SE4, reviewer CS2).
- [ ] RED-05 — Làm sạch dữ liệu ẩn (owner CS1, reviewer CS2).
- [ ] RED-06 — Ghi PDF sạch và bảo toàn nội dung (owner SE4, reviewer CS2).
- [ ] RED-07 — Artifact export bất biến (owner SE4, reviewer CS2).
- [ ] VER-01 — Kiểm tra text còn sót (owner CS2, reviewer SE3).
- [ ] VER-02 — Kiểm tra ảnh và OCR đầu ra (owner CS2, reviewer SE3).
- [ ] VER-03 — Kiểm tra cấu trúc và dữ liệu ẩn (owner CS2, reviewer CS1).
- [ ] VER-04 — Kiểm tra độ toàn vẹn đầu ra (owner CS2, reviewer SE3).
- [ ] VER-05 — Tổng hợp kiểm tra và báo cáo (owner CS2, reviewer CS1).
- [ ] VER-06 — Quét PII còn sót (owner CS2, reviewer ML1).
- [ ] QA-02 — E2E luồng sản phẩm (owner SE1, reviewer CS2).
- [ ] OPS-02 — Triển khai demo có đăng nhập (owner SE2, reviewer CS1).
- [ ] OPS-03 — Giới hạn tài nguyên xử lý (owner CS1, reviewer CS2).

## Thực hiện và kiểm tra

1. Kiểm tra dependency của từng mã trong inventory và chọn assignee thật trong CSV.
2. Đọc acceptance của mã; thống nhất contract và giới hạn chưa chốt trước khi code phần liên quan.
3. Triển khai, kiểm tra ca thành công/lỗi và ghi evidence vào CSV.
4. Reviewer kiểm tra, đồng bộ checkbox khi đạt acceptance; phase chỉ xong khi toàn bộ mã của phase đạt.

## Rủi ro và rollback

Không ghi đè bản gốc hoặc bỏ gate export. Quyết định stack/file code chưa được chọn; owner bổ sung lệnh test thực tế trước triển khai. Rollback theo phiên bản code/model/config; không xóa fixture đánh giá để làm pass.
