# Mini guideline — bài làm cá nhân

> Điền nội dung này trước khi bắt đầu gán nhãn. Giữ lại các quyết định sau khi self-QC.

## Định nghĩa lớp

| Lớp | Định nghĩa của bạn | Ví dụ/điểm phân biệt |
| --- | --- | --- |
| `car` | Xe con, sedan, SUV, taxi và xe bán tả | Không xếp xe tải chở hàng vào nhóm này |
| `truck` | Xe tải chở hàng, xe đầu kéo | Phân biệt với xe bán tải hoặc cabin nhỏ thuộc car |
| `bus` | Xe buýt, minibus chở khách | Không xếp van chở hàng hoặc chở người vào nhóm này |
| `van` | Xe van, minivan chở hàng hoặc chở người | Phân biệt với xe buýt lớn thuộc bus và xe con thông thường thuộc car |

## Quy tắc chung

- Box bám sát vật thể nghĩa là: Bao quanh sát đường viền phần phương tiện nhìn thấy, hạn chế khoảng trống thừa
- Vật thể bị che khuất: Vẫn gán nhãn nếu phần nhìn thấy đủ để nhận diện loại phương tiện
- Vật thể bị cắt bởi rìa ảnh: Box kéo đến sát rìa ảnh, không mở rộng ra ngoài khung hình
- Vật thể rất nhỏ/mơ hồ: Không tự đoán class nếu không đủ căn cứ nhận diện; ghi lại tên ảnh và hỏi người hướng dẫn
- Mỗi phương tiện hợp lệ có một bounding box riêng
- Xe đang đỗ vẫn được gán nhãn
- Các phương tiện chồng lấn được gán box riêng trên phần có thể quan sát
- Không gán nhãn người đi bộ, xe đạp, xe máy, biển báo và đèn giao thông
- Không gán nhãn phương tiện chỉ xuất hiện trong hình phản chiếu hoặc quảng cáo
## Ghi lại quyết định cho ít nhất ba ca mơ hồ

| Ảnh | Tình huống | Quyết định cuối | Lý do theo schema |
| --- | --- | --- | --- |
| `drive_.001` | Nhiều xe phía bên nhìn được và có thể đánh label cho xe nhwung gold file không có | Tiếp tục đánh label cho nhwungx xe có thể nhìn được còn thiếu | Đã ghi ở gạch đầu dòng 5,6,7 phần quy tắc chung |
| `drive_004` | Xe xám và xe đỏ ở góc phải trên đền có thể nhìn thấy và nhận diện loại phương tiện | Tiếp tục label cho hai xe  | Đã ghi ở gạch đầu dòng 2,3 phần quy tắc chung |
| `drive_010` | 2 xe xám ở góc phải và xe đỏ ở góc trái có thể nhìn thấy và nhận diện loại phương tiện | Tiếp tục label cho 3 xe | Đã ghi ở gạch đầu dòng 2,3 phần quy tắc chung |
