## Phân loại mạng máy tính :

### 1. Theo khoảng cách địa lý :
- Mạng cục bộ - LAN (local area network).
- Mạng đô thị - MAN (metropolitan area network).
- Mạng diện rộng - WAN ( wide area network).
- Mạng toàn cầu - GAN (global are network).

### 2. Theo kỹ thuật chuyển mạch :
#### 2.1 Mạng chuyển mạch kênh : 
khi có 2 thực thể cần kết nối với nhau thì chúng sẽ thiết lập 1 "kênh" cố định và được duy trì cho đến khi 1 trong 2 bên ngắt liên lạc. Các dữ liệu chỉ được truyền theo con đường cố định đó.

![a](https://i.imgur.com/ai2KxKF.png)

Nhược điểm : 
		- Tốn thời gian để thiết lập kết nối giữa 2 thực thể.
		- Hiệu suất sử dụng đường truyền thấp.

#### 2.2 Mạng chuyển mạch thông báo :
- Thông báo (message) là một đơn vị thông tin của người dùng có khuôn dạng được quy định trước. Mỗi thông báo đều có chứa vùng thông tin điều khiển trong đó chỉ rõ địa chỉ đích đến của thông báo. Căn cứ vào thông tin này mà mỗi nút trung gian có thể chuyển đến nút kế tiếp dựa vào địa chỉ đích.
- Tùy vào điều kiện mạng mà các thông báo khác nhau có thể đi theo đường truyền khác nhau.
	![a](https://i.imgur.com/ijPempk.png)

- Ưu điểm so với mạng chuyển mạch kênh :

	-	Hiệu suất đường truyền cao vì không bị chiếm dụng băng thông độc quyền.
	-	giảm đc tình trạng tắc nghẽn mạng vì mỗi nút có thể lưu trữ thông báo cho đến khi kênh truyền rỗi.
	-	Có thể điều khiển việc truyền tin bằng cách sắp xếp độ ưu tiên cho các thông báo.
	-	Có thể tăng hiệu suất sử dụng dải thông bằng cách gán địa chỉ quảng bá để gửi đi đồng thời tới nhiều đích.

- Nhược điểm :

	-	Không hạn chế kích thước của các thông báo, dẫn đến phí tổn lưu trữ tạm thời cao, ảnh hưởng đến thời gian hồi đáp và chất lượng truyền tin.
	-	thích hợp cho chuyển thư tín điện tử hơn là các áp dụng thời gian thực.

#### 2.3 Mạng chuyển mạch gói :
- Mỗi thông báo được chia làm nhiều phần nhỏ hơn được gọi là các gói tin có khuôn dạng quy định trước. Mỗi gói tin có chứa thông tin điều khiển, trong đó có địa chỉ nguồn và đích của gói tin. Các gói tin của một thông báo có thể đi theo nhiều đường khác nhau. Khi tới đích có thể không đúng thứ tự.
	![a](https://i.imgur.com/YwWGeeY.png)
- Mạng chuyển mạch thông báo và chuyển mạch gói có phương pháp giống nhau.
- Nhưng cũng có nhiều điểm khác : Các gói tin được giới hạn kích thước sao cho các nút mạng có thể xử lí toàn bộ các gói tin trong bộ nhớ mà không cần lưu trữ tạm thời trên đĩa. Cần phải có cơ chế đánh dấu gói tin và phục hồi gói tin bị thất lạc hoặc truyền bị lỗi trên các nút.

### 3. Phân loại theo kiến trúc mạng :
- Có thể phân loại mạng máy tính theo kiến trúc mạng (topo và giao thức).
- một số mạng thường dùng : mạng SNA của IBM, mạng ISO, mạng TCP/IP,...
