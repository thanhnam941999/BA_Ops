# JIRA Tasks — PROJECT_DTI

Mỗi file trong thư mục này là 1 task, viết sẵn theo format chuẩn để copy thẳng vào Jira: **Tiêu đề / Mục tiêu / Luồng xử lý / Yêu cầu / Kết quả mong đợi / Cần làm rõ** (chỉ xuất hiện khi thật sự thiếu thông tin). Không đi vào giải pháp kỹ thuật — phần đó dev tự quyết định khi triển khai.

**Định dạng:** nội dung bên trong mỗi file task dùng cú pháp **Jira wiki markup** (Jira Server/Data Center nội bộ VNPT — không phải Markdown), để copy nguyên văn dán thẳng vào ô mô tả Jira là ra đúng heading/danh sách:
- Heading → `h3. Tên mục` (không phải `### Tên mục`)
- Danh sách gạch đầu dòng → `* mục`
- Danh sách số → `# mục`
- In đậm → `*chữ*`
- (File `README.md` này thì viết Markdown bình thường vì chỉ đọc nội bộ, không paste vào Jira.)

Đây là task ở mức có thể lên Jira (không phải bảng theo dõi tổng quan — bảng đó xem ở `../TASKS.md`).

## Quy ước đặt tên file

`<tên-ngắn-gọn-không-dấu>.md`, ví dụ: `tao-bo-khung-nang-luc-dong.md`

## Danh sách

| File | Loại | Trạng thái |
|---|---|---|
| [tao-bo-khung-nang-luc-dong.md](tao-bo-khung-nang-luc-dong.md) | Feature | Đã xây xong (phiếu ghi nhận lại để đưa vào Jira) |
