# PROJECT_DTI — Nền tảng Chuyển đổi số Giáo dục (VNPT-IT/DES)

> Góc nhìn BA — không đi vào chi tiết kỹ thuật (dev tự xử lý phần đó).

## 1. Tổng quan

Nền tảng phục vụ đánh giá & quản lý chuyển đổi số giáo dục phổ thông, do VNPT-IT/DES phát triển cho Bộ GD&ĐT / Sở-Phòng GD / nhà trường.

**3 mảng nghiệp vụ:**

| Mảng | Mô tả | Trạng thái |
|---|---|---|
| CDS — Đánh giá chuyển đổi số cơ sở giáo dục | Trường tự đánh giá mức độ CĐS theo bộ tiêu chí Bộ GD ban hành/năm học; Sở/Phòng đánh giá ngoài | Đang vận hành |
| TT18 — Khung năng lực số (KNS) cho GV & CBQL | GV/CBQL tự đánh giá năng lực số cá nhân | Đang vận hành v1, còn thiếu luồng "gửi lại yêu cầu chỉnh sửa" |
| TT02 — Khung đánh giá "người học" | Đánh giá năng lực số cho đối tượng người học | Phần khung/danh mục xong; phần nộp bài — chấm — kết quả CHƯA làm |

## 2. Trọng tâm hiện tại: tổng quát hóa TT18 + TT02

**Vấn đề:** TT18 ban đầu được xây riêng biệt cho chính nó. Khi TT02 xuất hiện, nếu tiếp tục làm riêng cho từng thông tư thì mỗi lần có quy định mới lại phải làm lại từ đầu.

**Hướng đi đã chọn:** xây một mô hình đánh giá cá nhân dùng chung — một hệ quản trị có thể phục vụ nhiều loại khung đánh giá (GV/CBQL theo TT18, người học theo TT02, và các thông tư tương lai) thay vì làm riêng từng thông tư.

**Đã xong:** phần quản trị khung đánh giá dùng chung — danh mục loại đối tượng, thang mức độ, cấu trúc khung (nhóm tiêu chí/tiêu chí/rubric), phạm vi áp dụng.

**Chưa làm:** phần nộp bài, chấm điểm, kết quả, minh chứng cho TT02 — đang chờ chốt **hình thức đánh giá của TT02** (ai đánh giá, quy trình ra sao — tương đương việc TT18 đã chốt "GV tự đánh giá → CBQL đánh giá lại").

## 3. Stakeholder

| Vai trò | Bên |
|---|---|
| Ban hành chính sách | Bộ GD&ĐT (TT18, TT02, bộ tiêu chí CĐS) |
| Duyệt / đánh giá ngoài | Sở/Phòng GD&ĐT |
| Người dùng chính | Nhà trường: GV, CBQL (Hiệu trưởng/Phó HT/Tổ trưởng/Tổ phó chuyên môn) |
| Phát triển | VNPT-IT/DES |

## 4. Cần làm rõ

- [ ] Số hiệu đầy đủ + ngày hiệu lực của TT02
- [ ] Hình thức đánh giá TT02 (ai tự đánh giá, ai chấm/duyệt) — quyết định này đang chặn phần còn lại
- [ ] Deadline cho phần tổng quát hóa TT18/TT02 (TT18 gốc có deadline "hoàn thành tháng 7/2026" — đã qua, cần xác nhận đây có còn là mốc áp dụng hay không)
- [ ] Tiến độ gần nhất (từ giữa tháng 8/2026 đến nay) chưa được cập nhật vào đây
