# Rà soát hồ sơ Lab04 — 13/11/2026

## Nội dung và dữ liệu đã kiểm

- Báo cáo có đủ mục 0–8, tài liệu tham khảo và Bonus B1/B2; các mục cá nhân được biên tập từ ý và các quyết định học viên đã xác nhận.
- assignment.json khớp bộ ảnh tính lại bằng MSSV 2A202603176; không sửa assignment hoặc JSON bên trong ZIP.
- Người chính: 12 ảnh / 20 skeleton. Mặt chính: 8 ảnh / 8 skeleton. Checker: 0 lỗi, 0 cảnh báo.
- Bonus B1: 3 ảnh / 9 skeleton, 0 lỗi / 2 cảnh báo ở 000000213506.jpg; cả hai cảnh báo có giải thích giữ nguyên trong báo cáo.
- Bonus B2: 5 ảnh / 5 mặt, 0 lỗi / 0 cảnh báo; có nhận xét về ảnh không màu/hồng ngoại.
- Ngày rà soát, job 13/14/15/16 đều completed; bốn ZIP khớp toàn bộ tọa độ/cờ nhãn đang lưu trên CVAT sau làm tròn hai chữ số thập phân.
- Review: 10 dòng, đúng 5 ảnh người và 3 ảnh mặt, có hai ảnh back. Phân bố mã: lr_swap=0, vis_flag=5, position=1, missing=1, extra=0, ok=3.
- Đã chèn bốn ảnh thật, đúng tên: label person; người quay lưng 000000157271.jpg; mặt face_196742.jpg; JSON 000000021235.jpg. Giá trị keypoints/num_keypoints trong ảnh JSON khớp ZIP.

## Các lựa chọn đã xác nhận

- 000000469061.jpg: left_shoulder đổi tọa độ; right_eye từ v=2 sang v=1.
- 000000438099.jpg: hai mắt và left_hip đổi từ v=2 sang v=1; hông trái có điều chỉnh vị trí.
- 000000351176.jpg: hai mắt giữ v=1 theo quyết định chủ động của học viên; không ghi thành đã đổi cờ.
- 000000043500.jpg: left_eye giữ v=2; right_eye đổi sang v=1.
- Người áo xanh ở 000000461389.jpg đã được thêm; hai hông outside. Mặt kính râm face_256814.jpg đã đổi đủ tám điểm mắt sang v=1.
- B1 giữ cảnh báo khoảng trải điểm 59,48 px của người cửa sổ và cặp mắt khác phía với các cặp cơ thể của người phụ nữ cạnh xe đạp; lý do và giới hạn phép kiểm có trong báo cáo.

## Giới hạn và bước nộp

- Ảnh 1 đã có nhưng chữ vùng đầu chồng nhau; nên chụp lại để 17 tên điểm đọc rõ ngay trên ảnh. Báo cáo kèm bảng tên điểm theo schema để hỗ trợ đọc, không coi đó là ảnh chụp thay thế.
- Không ghi lại thời gian từng nhóm/CP, số ảnh ở phút 105, số người nhỏ và số poster/gương/màn hình bỏ qua theo nhóm. Báo cáo nói rõ không có thống kê riêng, không tự tạo số 0.
- Kiểm định dạng không chấm OKS, không xác nhận vị trí trùng GT hoặc bảo đảm điểm số.
- Chưa đánh dấu đã commit/push hay nộp LMS. Tên repo hiện thêm hậu tố -Student so với mẫu SUBMISSION.md; cần đối chiếu thông báo của lớp trước khi nộp.
