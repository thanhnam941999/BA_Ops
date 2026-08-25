# REQUIREMENTS — PROJECT_DTI

## R1. TT18 — Khung năng lực số (KNS) cho GV & CBQL

**Hiệu lực:** 12/05/2026. **Mục tiêu hoàn thành ban đầu:** tháng 7/2026 (cần xác nhận trạng thái thực tế).

**Cấu trúc GV:** 6 miền năng lực → 20 năng lực thành phần → 3 mức (Cơ bản / Thành thạo / Nâng cao)
1. Tổ chức dạy học trong môi trường số
2. Kiểm tra, đánh giá
3. Trao quyền cho người học
4. Kĩ năng công nghệ số
5. Phát triển chuyên môn
6. Trí tuệ nhân tạo (AI)

**Cấu trúc CBQL:** khung RIÊNG hoàn toàn — 5 miền, 24 năng lực (không phải "20 NL của GV cộng thêm"; AI được gộp vào mục Kĩ năng công nghệ số, không tách miền riêng cho CBQL).

**Đối tượng:** GV phổ thông + CBQL cơ sở giáo dục (ưu tiên). Mầm non: đã có dữ liệu chuẩn bị sẵn nhưng chưa kích hoạt sử dụng.

**Quy trình đánh giá:**
```
GV tự đánh giá (draft) → GV gửi → CBQL được phân công đánh giá lại/xác nhận → kết quả chính thức lưu hệ thống
```
Phòng/Sở chỉ xem báo cáo tổng hợp, không có bước duyệt thêm.

**Mô hình phân công:** 1 CBQL phụ trách N giáo viên (gán thủ công), 1 GV chỉ thuộc 1 CBQL tại 1 thời điểm.

**Minh chứng:** hiện để tùy chọn cho v1 — **chưa chốt** có bắt buộc hay không (xem DECISIONS.md).

**Còn thiếu:** luồng "CBQL trả lại yêu cầu GV chỉnh sửa" — hiện GV gửi rồi là CBQL chấm luôn, chưa có bước trả về để sửa lại.

## R2. TT02 — Khung đánh giá "người học"

**Cần làm rõ:** số hiệu đầy đủ, cơ quan/ngày ban hành.

**Cấu trúc (dựa theo văn bản TT02 đã nghiên cứu):**
- Đối tượng: người học
- Thang đánh giá: 8 bậc, gộp thành 4 nhóm mức độ
- 6 nhóm tiêu chí, 24 tiêu chí chi tiết
- Hiện mới ở dạng khung nháp, **chưa kích hoạt áp dụng**

**Cần chốt gấp:** hình thức đánh giá TT02 — ai tự đánh giá, ai chấm/xác nhận, quy trình ra sao. Đây là quyết định nghiệp vụ đang chặn toàn bộ phần triển khai còn lại (nộp bài, chấm điểm, kết quả, minh chứng).

## R3. Định hướng tổng quát hóa (chung cho TT18 + TT02 + các thông tư tương lai)

**Mục tiêu:** một mô hình đánh giá cá nhân dùng chung, để khi có thông tư mới không phải xây lại từ đầu — chỉ cần khai báo: loại đối tượng, thang mức độ, cấu trúc khung (nhóm tiêu chí/tiêu chí/rubric theo từng mức), phạm vi áp dụng (tỉnh/kỳ).

**Đã có:** phần khai báo/quản trị khung nói trên — dùng được cho cả TT18 và TT02.

**Chưa có:** phần vận hành (nộp bài — chấm điểm — kết quả — minh chứng) theo mô hình dùng chung. TT18 hiện vẫn chạy quy trình riêng của nó (xem R1); phần dùng chung mới dừng ở giai đoạn khai báo khung.

## R4. Nguyên tắc nghiệp vụ chung (áp dụng cho các luồng đánh giá CĐS/TT18/TT02)

- Tự đánh giá và đánh giá ngoài/đánh giá lại là 2 luồng kết quả độc lập — không gộp chung, chỉ liên kết về mặt nghiệp vụ (bước sau chỉ bắt đầu khi bước trước đã được duyệt/gửi).
- Khi 1 tỉnh/đơn vị không có cấu hình riêng thì áp dụng theo cấu hình mặc định toàn quốc.
- Trường/GV/CBQL không tự chọn bộ tiêu chí — hệ thống tự xác định theo phạm vi áp dụng đã được Bộ/Sở cấu hình sẵn.
- Mọi thay đổi trạng thái/điểm số phải lưu vết đầy đủ, phục vụ tra cứu khi có tranh chấp/khiếu nại.
