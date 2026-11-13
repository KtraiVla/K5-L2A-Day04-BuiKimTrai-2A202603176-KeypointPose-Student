# Chụp 4 ảnh minh chứng Lab04 — từng bước

Mỗi ảnh chỉ cần chụp đúng phần làm bằng chứng, không cần chụp cả màn hình hoặc gửi lại toàn bộ ảnh gốc. Thư mục lưu: D:\VinUni-AI in Action\Lab04\K5-L2A-Day04-BuiKimTrai-2A202603176-KeypointPose-Student\report\individual\images.

## Cách chụp chung trên Windows 11

Mở đúng nội dung, nhấn **Win + Shift + S**, chọn khung chữ nhật rồi kéo vùng cần chụp. Mở ảnh vừa chụp trong Snipping Tool (qua thông báo hoặc ứng dụng), nhấn **Ctrl + S**, chọn thư mục images nói trên, đặt đúng tên và lưu kiểu PNG. Nguồn thao tác: [Microsoft Support](https://support.microsoft.com/en-us/windows/apps/use-snipping-tool-to-capture-screenshots).

## 1_label_person.png — label mẫu

CVAT → Projects → d04-keypoint → Constructor → biểu tượng sửa của label person. Chỉ mở để xem. Căn khung cho thấy tên label person và trọn skeleton với tên điểm; vùng đầu/mắt/tai càng đọc rõ càng tốt. Không di chuyển điểm mẫu chỉ để chụp. Chụp rồi Cancel để đóng chế độ xem nếu không chỉnh label. Bạn đã có ảnh này, nhưng có thể chụp lại rõ hơn.

## 2_nguoi_quay_lung.png — người quay lưng đã gán

1. Mở [job người, frame 6](http://localhost:8080/tasks/13/jobs/13?frame=6), kiểm tên ảnh **000000351176.jpg**.
2. Chọn người chơi tennis quay lưng. Phóng to vừa đủ để thấy người và các điểm đã gán; các điểm occluded hiển thị vòng rỗng/nét đứt, outside không xuất hiện.
3. Nếu được, để cả bảng điểm/Parts bên phải trong vùng chụp. Chụp phần người quay lưng và nhãn, không cần cả trang web.
4. Lưu **2_nguoi_quay_lung.png**. Nguồn ảnh trong báo cáo: COCO 2017, ảnh chụp nhãn CVAT của học viên.

## 3_mat_phong_to.png — một mặt 13 điểm

1. Mở [job mặt, frame 0](http://localhost:8080/tasks/14/jobs/14?frame=0), kiểm tên ảnh **face_145751.jpg**.
2. Phóng to khuôn mặt để nhìn rõ các điểm khóe/mí mắt, mũi và miệng. Giữ đủ 13 điểm trong hình; đừng chỉ cắt một mắt.
3. Chụp khuôn mặt đã gán cùng điểm, lưu **3_mat_phong_to.png**. Có thể dùng một mặt khác trong bộ đã giao nếu hiển thị rõ hơn.
4. Nguồn ảnh: COCO 2017, ảnh chụp nhãn CVAT của học viên.

## 4_json_export.png — đoạn JSON thật từ ZIP

Trợ lý đã tách JSON nguyên bản từ ZIP persons ra thư mục hỗ trợ ngoài repo, đồng thời tạo bản xem một annotation của **000000021235.jpg**. Bản xem giữ nguyên mọi giá trị được hiển thị, chỉ sắp xếp mỗi bộ x,y,v thành một dòng cho dễ đọc. Không thay đổi ZIP nộp.

1. Mở file JSON bản xem được gửi trong chat bằng Notepad hoặc trình soạn thảo.
2. Để thấy dòng keypoints, các bộ ba bên trong và dòng num_keypoints=17; thu nhỏ chữ nếu cần.
3. Chụp vùng văn bản đó, lưu **4_json_export.png** vào thư mục images.
4. Ghi nguồn: đoạn annotation COCO Keypoints xuất từ BuiKimTrai_persons.zip, định dạng lại để hiển thị; dữ liệu không đổi.

## Tự kiểm ảnh trước khi báo đã xong

- Đúng bốn tên file PNG; không bị thành .png.png hoặc .jpg.
- Ảnh đọc được chữ/điểm, không bị hộp thoại che nội dung.
- Ảnh 2 thấy người quay lưng, ảnh 3 thấy mặt 13 điểm, ảnh 4 thấy keypoints và num_keypoints.
- Sau khi có ảnh thật, chèn chúng vào mục 6 và cập nhật trạng thái; không dùng hình dựng overlay thay ảnh chụp CVAT.
