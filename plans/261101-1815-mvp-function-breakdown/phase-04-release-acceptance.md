---
title: "Phase 4: Release acceptance"
status: todo
---

# Release acceptance

## Phạm vi

Mốc P4; xem lịch và hợp đồng trong [Function breakdown](./function-breakdown.md).

## Công việc

- [ ] QA-07 — Nghiệm thu phát hành (owner CS2, reviewer CS1).
- [ ] OPS-05 — Phát hành, rollback và dọn dữ liệu (owner SE2, reviewer CS1).

## Thực hiện và kiểm tra

1. Kiểm tra dependency của từng mã trong inventory và chọn assignee thật trong CSV.
2. Đọc acceptance của mã; thống nhất contract và giới hạn chưa chốt trước khi code phần liên quan.
3. Triển khai, kiểm tra ca thành công/lỗi và ghi evidence vào CSV.
4. Reviewer kiểm tra, đồng bộ checkbox khi đạt acceptance; phase chỉ xong khi toàn bộ mã của phase đạt.

## Rủi ro và rollback

Không ghi đè bản gốc hoặc bỏ gate export. Quyết định stack/file code chưa được chọn; owner bổ sung lệnh test thực tế trước triển khai. Rollback theo phiên bản code/model/config; không xóa fixture đánh giá để làm pass.
