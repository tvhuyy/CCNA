## Compare and contrast IPv4 address types: Unicast Broadcast Multicast

### 1. IPv4 ( Internet Protocol version 4) :
- **IPv4** là phiên bản thứ tư trong quá trình phát triển của các giao thức Internet (IP). Đây là phiên bản đầu tiên của IP được sử dụng rộng rãi. IPv4 cùng với IP v6 (giao thức Internet phiên bản 6) là nòng cốt của giao tiếp internet. Hiện tại, IPv4 vẫn là giao thức được triển khai rộng rãi nhất trong bộ giao thức của lớp internet.
- **IPv4** là giao thức hướng dữ liệu, được sử dụng cho hệ thống chuyển mạch gói (tương tự như chuẩn mạng Ethernet ). Đây là giao thức truyền dữ liêu hoạt động dựa trên nguyên tắc tốt nhất có thể, trong đó, nó không quan tâm đến thứ tự truyền gói tin cũng như không đảm bảo gói tin sẽ đến đích hay việc gây ra tình trạng lặp gói tin ở đích đến. Việc xử lý vấn đề này dành cho lớp trên của chồng giao thức TCP/IP. Tuy nhiên, IPv4 có cơ chế đảm bảo tính toàn vẹn dữ liệu thông qua sử dụng những gói kiểm tra
- **IPv4** sử dụng 32bit để đánh địa chỉ và được chia làm 4 octet( mỗi octet có 8bit tương đương với 1byte), mỗi octet được cách nhau bằng dấu chấm.
- Mỗi một địa chỉ IPv4 có 2 thành phần chính : Địa chỉ của mạng (network ID) và địa chỉ của máy (host ID).
![alt](https://i.imgur.com/hMRqvmF.png)

### 2. phân loại và so sánh các loại địa chỉ IPv4 :
| loại địa chỉ | so sánh  |
|--|--|
| Unicast (1-1) | Thuộc loại địa chỉ 1 host liên lạc với 1 host |
| Multicast (1-nhiều) |Thuộc loại 1 host liên lạc được đồng thời 1 nhóm host. Chủ yếu dùng trong các giao thức định tuyến và các dịch vụ  |
|Broadcast (1-all)|Loại địa chỉ dùng bởi các ứng dụng và host để gửi thông tin tới tất cả các máy trong network mà IP đó thuộc


