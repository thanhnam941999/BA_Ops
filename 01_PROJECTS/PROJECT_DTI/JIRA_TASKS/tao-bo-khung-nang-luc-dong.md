h2. [Feature] Cho phép quản trị viên tự tạo bộ khung năng lực đánh giá mới

*Trạng thái thực tế:* phần khai báo/quản trị bộ khung đã được dev xây dựng xong. Đưa lên đây để có phiếu chính thức trong Jira — vừa phục vụ theo dõi, vừa làm ví dụ trình bày năng lực nền tảng của hệ thống.

h3. Mục tiêu

Hiện tại, mỗi khi có một thông tư/quy định đánh giá mới (như TT18, TT02...), hệ thống phải được lập trình riêng từ đầu cho bộ tiêu chí đó — tốn thời gian phát triển và luôn đi sau chính sách. Tính năng này cho phép *quản trị viên cấp Bộ tự khai báo một bộ khung năng lực đánh giá hoàn toàn mới ngay trên giao diện quản trị, không cần chờ dev code riêng* — rút ngắn thời gian đưa một quy định đánh giá mới vào vận hành.

Đây là năng lực nền tảng: một khi đã có, hệ thống có thể tiếp nhận bất kỳ thông tư đánh giá cá nhân nào trong tương lai (không chỉ TT18/TT02) mà không cần dự án phát triển riêng cho từng thông tư.

h3. Luồng xử lý

# Quản trị viên cấp Bộ chọn "Tạo bộ khung đánh giá mới".
# Khai báo thông tin chung: tên bộ khung, đối tượng áp dụng (giáo viên, CBQL, người học, hoặc đối tượng khác), chọn thang mức độ sử dụng (dùng thang có sẵn hoặc tạo thang mới).
# Xây cấu trúc khung: thêm các nhóm tiêu chí; trong mỗi nhóm thêm các tiêu chí chi tiết.
# Với mỗi tiêu chí, mô tả yêu cầu cần đạt ở từng mức độ của thang đã chọn.
# Thiết lập phạm vi áp dụng: toàn quốc hay riêng theo tỉnh, áp dụng cho kỳ/năm học nào.
# Lưu ở trạng thái nháp để tiếp tục chỉnh sửa, hoặc kích hoạt để đưa vào sử dụng chính thức.
# Sau khi kích hoạt, bộ khung sẵn sàng để triển khai phần đánh giá (tự đánh giá/chấm điểm) tương ứng.

h3. Yêu cầu

* Không giới hạn số lượng bộ khung — hệ thống cho phép nhiều bộ khung tồn tại song song, không ảnh hưởng lẫn nhau (ví dụ TT18 và TT02 chạy đồng thời).
* Một thang mức độ có thể dùng chung cho nhiều bộ khung khác nhau, không cần khai báo lại mỗi lần.
* Bộ khung ở trạng thái nháp không được ảnh hưởng tới dữ liệu đang vận hành thật.
* Không cho xóa/sửa cấu hình phạm vi áp dụng nếu đã có dữ liệu đánh giá thật gắn với cấu hình đó — tránh mất liên kết dữ liệu.
* Chỉ quản trị viên được phân quyền cấp Bộ mới thao tác được tính năng này (không phải quản trị viên trường/Sở).

h3. Kết quả mong đợi

Khi có thông tư/quy định đánh giá mới ban hành, đội nghiệp vụ có thể tự cấu hình và đưa vào vận hành mà không cần chờ một chu kỳ phát triển phần mềm riêng — rút ngắn đáng kể thời gian phản ứng với chính sách mới, đồng thời giảm tải cho đội dev khi số lượng thông tư/bộ tiêu chí tăng theo thời gian.

h3. Cần làm rõ

* Có cần một bước duyệt (và ai duyệt) trước khi bộ khung mới được kích hoạt, hay quản trị viên tạo xong là kích hoạt được luôn?
* Khi một bộ khung đã kích hoạt và đã có dữ liệu đánh giá thật, cần sửa cấu trúc (thêm/bớt tiêu chí) thì xử lý thế nào — có cho sửa tự do không, hay phải tạo phiên bản mới?
