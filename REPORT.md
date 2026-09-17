# Báo cáo Day 5 — điền trực tiếp trong fork của bạn

- Mã học viên theo lớp: D5_012
- Ngày / CVAT local: … *(điền ngày bạn thực làm)*
- Công cụ đã dùng: CVAT (Brush/Polygon), không dùng SAM

## 1. Bài đã nộp

*(Dựa trên kết quả QC thật trong notebook — cell BƯỚC 4, 05, 06, 07)*

| Task | File ZIP đúng tên | Hoàn thành mấy ảnh | Điểm tối đa (coach chấm sau) |
| --- | --- | ---: | ---: |
| easy_semantic | easy_semantic.zip | 3 / 3 | 20 |
| medium_instance | medium_instance.zip (**lỗi export, xem mục 3**) | 3 / 3 | 32 |
| hard_panoptic | hard_panoptic.zip | 2 / 2 | 30 |
| cp1_holes | chưa có | 0 / 1 | 3 |
| cp2_slice | chưa có | 0 / 1 | 3 |
| cp5_occlusion | chưa có | 0 / 1 | 3 |
| cp3_thin | chưa có | 0 / 1 | 3 |
| cp4_curb | chưa có | 0 / 1 | 3 |
| cp6_coverage | chưa có | 0 / 1 | 3 |
| **Tổng tối đa** | | | **100** |

Ghi chú thật từ QC: `medium_instance` đã export nhưng notebook báo **LỖI** ("category ngoài classes.json: building, road, sidewalk, sky, vegetation") — tức file ZIP đang chứa nhãn của task semantic thay vì nhãn xe cộ (bicycle/bus/car/motorcycle/person/truck). Cần export lại từ đúng task trong CVAT trước khi nộp.

## 2. Một quyết định trước khi dùng gợi ý

**Cần bạn tự điền — thông tin này không nằm trong notebook.** Notebook chỉ đọc cấu trúc ZIP (số annotation, loại polygon/RLE...), nó không biết bạn đã chọn vẽ object nào đầu tiên hay quy tắc biên bạn dùng lúc thao tác trong CVAT.

- Ảnh, vị trí và object Medium đầu tiên tự vẽ: …
- Class và quy tắc tôi dùng để chọn biên: …
- Nếu dùng gợi ý sau đó: vùng gợi ý sai/đúng, hành động sửa/giữ và lý do: …
- Nếu không dùng gợi ý: ghi "không dùng"; vẫn giải thích một quyết định gán nhãn của mình.

## 3. Một lỗi tôi tìm thấy và sửa

*(Đây là lỗi thật lấy trực tiếp từ output QC ở cell BƯỚC 05 — bạn có thể dùng luôn hoặc thay bằng lỗi khác nếu có.)*

- Task/ảnh/vùng: medium_instance (cả 3 ảnh: 000000181542.jpg, 000000373353.jpg, 000000458325.jpg)
- Lỗi thuộc loại: sai lớp (category không khớp classes.json của task instance)
- Bằng chứng tôi nhìn thấy: notebook báo `SỬA: category ngoài classes.json: building, road, sidewalk, sky, vegetation` — đây là nhãn của task semantic, không phải nhãn xe cộ mà `medium_instance` yêu cầu

## 4. Ba ca chưa chắc hoặc đã cân nhắc

**Cần bạn tự điền — đây là quan sát trực quan trong CVAT (vùng che khuất, ranh giới mờ...), notebook không thấy được nội dung ảnh nên không thể tạo thay.**

| Ảnh/vị trí | Hai cách hiểu có thể | Quy tắc/chứng cứ | Quyết định hoặc câu hỏi cho coach |
| --- | --- | --- | --- |
| 1 | … | … | … |
| 2 | … | … | … |
| 3 | … | … | … |
