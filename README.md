# PII Detection & Secure PDF Redaction MVP

Dự án MVP phát hiện PII (Personally Identifiable Information) và xóa nhạy cảm an toàn trên tài liệu PDF (Native, Scanned, Mixed).

## 👥 Danh sách thành viên & Phân công trách nhiệm

| Thành viên | Vai trò | Chuyên môn | Trách nhiệm chính | Số task |
| :--- | :---: | :---: | :--- | :---: |
| **Nguyễn Đinh Phú Vinh** | `SE2` | ICT | **Backend & System Lead**: API, Job Queue, Database, Docker server, tích hợp Model Serving; đồng thiết kế kiến trúc model | **16** |
| **Dương Minh Đức** | `SE1` | ICT | **Frontend**: Giao diện Web, PDF viewer, reviewer overlay, khoanh vùng PII thủ công | **13** |
| **Đỗ Minh Tấn** | `SE4` | ICT | **Data & PDF Engine**: Xây dựng Regex, chuẩn bị dataset, thuật toán bóc tách/xóa triệt để vector stream PDF | **12** |
| **Nguyễn Tuấn Vinh** | `SE3` | ICT | **Document / OCR**: Bóc tách text native, tích hợp OCR engine, tính toán tọa độ bounding box | **11** |
| **Hoàng Thị Kiều Ly** | `CS2` | CS | **Security Verification**: Pentest độc lập, tạo fixture đối kháng rà soát leak dữ liệu PDF sau xuất | **10** |
| **Nguyễn Quang Anh** | `CS1` | CS | **Security Engineering**: Chính sách PII, phân quyền RBAC, audit log, resource isolation | **9** |
| **Nguyễn Đăng Đạt** | `ML1` | ICT | **Machine Learning Lead**: Trực tiếp chạy Colab Pro, fine-tune checkpoint model NER, đánh giá F1/Recall | **4** |

---

## 📋 Tài liệu kế hoạch & Backlog chi tiết

Mọi người theo dõi chi tiết công việc, acceptance criteria và dependencies tại thư mục [`plans/261101-1815-mvp-function-breakdown/`](./plans/261101-1815-mvp-function-breakdown/):

* **[Function Backlog CSV](./plans/261101-1815-mvp-function-breakdown/function-backlog.csv)**: Bảng theo dõi 75 work packages, assignee, reviewer, priority, status.
* **[Function Breakdown](./plans/261101-1815-mvp-function-breakdown/function-breakdown.md)**: Đặc tả chi tiết từng mã công việc và tiêu chuẩn nghiệm thu (Acceptance Criteria).
* **[Kế hoạch tổng thể (Plan)](./plans/261101-1815-mvp-function-breakdown/plan.md)**: Mục tiêu và quy định làm việc của dự án.
* **Các Phase triển khai**:
  * [Phase 1: Contracts & Data Foundations](./plans/261101-1815-mvp-function-breakdown/phase-01-start.md)
  * [Phase 2: Core MVP](./plans/261101-1815-mvp-function-breakdown/phase-02-core-mvp.md)
  * [Phase 3: Hardening & Evaluation](./plans/261101-1815-mvp-function-breakdown/phase-03-hardening-evaluation.md)
  * [Phase 4: Release Acceptance](./plans/261101-1815-mvp-function-breakdown/phase-04-release-acceptance.md)
