# TASKS — PROJECT_DTI

> Bảng theo dõi tổng quan. Các task đã sẵn sàng đưa vào Jira (viết chi tiết theo format riêng) nằm ở [`JIRA_TASKS/`](JIRA_TASKS/README.md).

## Epic: Tổng quát hóa khung đánh giá (TT18 + TT02)

| Việc | Trạng thái | Ghi chú |
|---|---|---|
| Xây phần quản trị khung đánh giá dùng chung (danh mục đối tượng, thang mức độ, cấu trúc khung, phạm vi áp dụng) | ✅ Hoàn thành | Dev đã build và tự kiểm tra xong |
| Đưa dữ liệu TT18 hiện có + dữ liệu TT02 vào mô hình dùng chung | ⏳ Đã chuẩn bị, chưa chạy chính thức | Chờ xác nhận thời điểm chuyển đổi |
| Cập nhật lại menu/điều hướng cho phù hợp cấu trúc mới | ⏳ Đã chuẩn bị, chưa áp dụng chính thức | Việc kỹ thuật thuần túy, dev tự quyết định thời điểm |
| Phần nộp bài — chấm điểm — kết quả — minh chứng cho TT02 | ❌ Chưa bắt đầu | **Blocker:** chưa chốt hình thức đánh giá TT02 (xem REQUIREMENTS.md R2) |
| Luồng "CBQL trả lại yêu cầu GV chỉnh sửa" (TT18) | ❌ Chưa làm | Còn thiếu so với quy trình đã thống nhất |

## Việc cần BA quyết định / làm rõ trước khi dev tiếp tục

- [ ] **Chốt hình thức đánh giá TT02** — đây là việc quan trọng nhất đang chặn tiến độ. Cần xác định: ai tự đánh giá, ai chấm/xác nhận, có cấp duyệt trung gian không (tương tự việc TT18 đã chốt "GV tự đánh giá → CBQL đánh giá lại").
- [ ] Xác nhận minh chứng TT18 bắt buộc hay tùy chọn (R1, Q3 trong DECISIONS.md).
- [ ] Xác nhận mốc deadline hiện tại cho phần tổng quát hóa (mốc gốc "tháng 7/2026" của TT18 đã qua).
- [ ] Cập nhật tiến độ mới nhất từ giữa tháng 8/2026 đến nay.

## Bài học rút ra (đề xuất đưa vào LESSONS_LEARNED.md)

- Khi thiết kế 1 mô hình dùng chung cho nhiều thông tư, nên chốt **hình thức đánh giá** (ai làm gì, quy trình) sớm cho mọi thông tư liên quan trước khi build phần khung — tránh tình trạng phần khai báo đã xong nhưng phần vận hành bị chặn vì thiếu quyết định nghiệp vụ.
