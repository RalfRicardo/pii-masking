---
title: "Phase 3: Hardening and evaluation"
status: todo
---

# Hardening and evaluation

## Phạm vi

Mốc P3; xem lịch và hợp đồng trong [Function breakdown](./function-breakdown.md).

## Công việc

- [ ] DATA-06 — Version và báo cáo dữ liệu (owner SE4, reviewer ML1).
- [ ] ML-07 — Đánh giá và phân tích lỗi (owner ML1, reviewer SE4).
- [ ] QA-03 — Kiểm thử an toàn redaction độc lập (owner CS2, reviewer SE3).
- [ ] QA-04 — Kiểm thử quyền truy cập (owner CS2, reviewer SE4).
- [ ] QA-05 — Kiểm thử lỗi và tranh chấp tác vụ (owner CS1, reviewer CS2).
- [ ] QA-06 — Hiệu năng và chất lượng sử dụng (owner SE4, reviewer CS2).
- [ ] OPS-04 — Quan sát và kiểm tra sức khỏe (owner SE2, reviewer CS1).

## Thực hiện và kiểm tra

1. Kiểm tra dependency của từng mã trong inventory và chọn assignee thật trong CSV.
2. Đọc acceptance của mã; thống nhất contract và giới hạn chưa chốt trước khi code phần liên quan.
3. Triển khai, kiểm tra ca thành công/lỗi và ghi evidence vào CSV.
4. Reviewer kiểm tra, đồng bộ checkbox khi đạt acceptance; phase chỉ xong khi toàn bộ mã của phase đạt.

## Rủi ro và rollback

Không ghi đè bản gốc hoặc bỏ gate export. Quyết định stack/file code chưa được chọn; owner bổ sung lệnh test thực tế trước triển khai. Rollback theo phiên bản code/model/config; không xóa fixture đánh giá để làm pass.
