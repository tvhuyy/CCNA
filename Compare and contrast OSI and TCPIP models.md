## Compare and contrast OSI and TCP/IP models

### 1. Khái niệm giao thức TCP/IP và mô hình OSI :
#### 1.1 **TCP/IP** - Giao thức kiểm soát truyền tải ( Transmission Control Protocol - TCP) và Giao thức Internet (Internet Protocol - IP ). 
- TCP/IP là một chuẩn phổ biến mà các mạng nội bộ và diện rộng có thể giao tiếp, cho phép máy tính kết nối với nhau và cho các ứng dụng gửi dữ liệu đi và về.
- TCP/IP là một họ các giao thức được gọi là họ giao thức IP, bao gồm bốn tầng. Cần nhớ rằng TCP/IP không phải là một giao thức mà thực sự là một họ các giao thức, và bao gồm các giao thức mức thấp khác như IP, TCP, và UDP. UDP nằm ở tầng giao vận, phía trên giao thức IP. Tầng giao vận cung cấp khả năng truyền tin giữa các mạng thông qua các gateway. Nó sử dụng các địa chỉ IP để gửi các gói tin trên Internet hoặc trên mạng thông qua các trình điều khiển thiết bị khác nhau. TCP và UDP là một phần của họ giao thức TCP/IP; mỗi giao thức có những ưu và nhược điểm riêng của nó.
- Giao thức IP là giao thức cơ bản của Internet. TCP và UDP đều là hai giao thức tầng giao thức vận trên cơ sở của giao thức IP.
#### 1.2 Các lớp trong giao thức TCP/IP : 4 lớp
- **Lớp kết nối (link layer)** - Đây là lớp thấp nhất trong ngăn TCP/IP và là một nhóm phương thức vận hành trên một kết nối của máy chủ, thường được biết đến là Ethernet.
- **Lớp Internet (IP)** - Đây là lớp kết nối các mạng nội bộ với nhau.
- **Lớp truyền tải (transport layer) (TCP)** - Đây là lớp điều khiển giao tiếp máy chủ tới máy chủ.
- **Lớp ứng dụng (application layer)** - Lớp ứng dụng là một tập hợp các giao thức cụ thể giao tiếp dữ liệu trên một lớp quá trình tới quá trình. Ví dụ, HTTP là một giao thức ứng dụng là nền tảng của World Wide Web (www).
![alt](https://i.imgur.com/eHHyvPP.gif)
#### 1.3 Mô hình OSI - Mô hình tham chiếu kết nối các hệ thống mở (Open Systems Interconnection).
- Mô hình OSI là một thiết kế dựa vào nguyên lý tầng cấp, lý giải một cách trừu tượng kỹ thuật kết nối truyền thông giữa các máy vi tính và thiết kế giao thức mạng giữa chúng. Mô hình này được phát triển thành một phần trong kế hoạch Kết nối các hệ thống mở (Open Systems Interconnection) do ISO và IUT-T khởi xướng. Nó còn được gọi là Mô hình bảy tầng của OSI.
- mô hình OSI được tổ chức Tổ chức tiêu chuẩn quốc tế - International Standards Organization (ISO) phát triển. Mô hình chia giao tiếp mạng thành 7 lớp. Lớp 1-4 là các lớp cấp thấp thông thường thực hiện các nhiệm vụ di chuyển dữ liệu. Lớp 5-7 là lớp cấp cao có chứa các dữ liệu ở cấp độ ứng dụng. Cách thức vận hành của các network nằm trong một quy tắc chung, đó là chuyển dữ liệu đi. Mỗi một lớp sẽ thực hiện các tác vụ đặc thù và sau đó, chuyển đi các dữ liệu tới lớp tiếp theo.
#### 1.4 Các lớp trong mô hình OSI :
- **Lớp 7 – Application** , lớp trên cùng trong mô hình hỗ trợ các thao tác cho ứng dụng và người dùng cuối. Các đối tác giao tiếp, chất lượng dịch vụ được xác định, xem xét và cân nhắc các xác thực người dùng, quyền riêng tư cũng như xác định bất kỳ ràng buộc nào về cú pháp dữ liệu. Lớp này chỉ cung cấp nền tảng làm việc (framework) mà ứng dụng đó chạy bên trên.
- **Lớp 6 - Presentation** lấy dữ liệu từ lớp Application, cũng cấp khả năng biểu diễn dữ liệu độc lập (ví dụ: mã hóa) và biến đổi các dữ liệu này sang một định dạng chuẩn để các lớp khác có thể hiểu được. Cũng tương tự, lớp Presentation sẽ chuyển hóa các dữ liệu nhận được từ lớp kế tiếp là lớp session thành các dữ liệu mà Application có thể chấp nhận được.
- **Lớp 5 - Session** lớp này thiết lập, quản lý và ngưng kết nối giữa các ứng dụng. Lớp session thiết lập, điều phối và kết thúc các giao tiếp, trao đổi qua lại giữa các ứng dụng ở mỗi đầu. Lớp này xử lý các phối hợp giữa session và connection.
- **Lớp 4 - Transport** sẽ lấy dữ liệu từ các ứng dụng và tích hợp chúng trong cùng một luồng để chuyển giao dữ liệu. Về cơ bản, nó đảm bảo cho một chu trình truyền dữ liệu hoàn chỉnh từ máy gửi đến máy nhận
- **Lớp 3 - Network** cung cấp các công nghệ chuyển mạch và định tuyến, tạo các logic path, hay còn được biết đến là các mạch ảo, giúp truyền dữ liệu từ node này sang node khác. Định tuyến và chuyển tiếp là các chức năng cơ bản của lớp này cũng như address, internetworking, xử lý lỗi, kiểm soát tắc nghẽn và trình tự packet.
- **Lớp 2 - Data Link** tại lớp này các gói dữ liệu sẽ được mã hóa và giải mã thành các bit. Data link cung cấp kiến thức về giao thức truyền tải, quản lý, xử lý các lỗi trong lớp physical, điều khiển luồng và đồng bộ hóa frame. Lớp Data link này được chia thành 2 lớp con: Lớp Media Access Control (MAC) và Logical Link Control (LLC). Lớp MAC sẽ kiểm soát việc truy cập và truyền tải dữ liệu của máy tính trên mạng. Lớp LLC kiểm soát đồng bộ hóa frame, kiểm soát luồng và kiểm tra lỗi.
- **Lớp 1 - Physical** lớp dưới cùng trong mô hình OSI truyền tải bit-stream, xung điện, tín hiệu ánh sáng hoặc radio - thông qua mạng ở cấp độ điện tử và cơ học. Lớp này cung cấp các tài nguyên phần cứng để gửi và nhận dữ liệu trên một carrier, bao gồm xác định cáp, card và các thành phần vật lý. Fast Ethernet, RS232 và ATM là các giao thức với các thành phần trong lớp Physical.

### 2. So sánh các mô hình OSI và TCP/IP :
#### 2.1 Giống nhau :
- Cả 2 mô hình OSI và TCP/IP đều là các mô hình khái niệm có mục đích chung hỗ trợ thảo luận về cách các máy tính giao tiếp với nhau.
- Cả hai đều là các khung để giúp hiểu các khái niệm và công nghệ mạng.
#### 2.2 Khác nhau :
- 1. OSI là một tiêu chuẩn độc lập chung, giao thức, hoạt động như một cổng giao tiếp giữa mạng và người dùng cuối. Mô hình TCP / IP dựa trên các giao thức chuẩn mà Internet đã phát triển. Nó là một giao thức truyền thông, cho phép kết nối các máy chủ qua mạng.
- 2. Trong mô hình OSI, lớp vận chuyển đảm bảo việc phân phối các gói. Trong mô hình TCP / IP, lớp vận chuyển không đảm bảo phân phối các gói. Tuy nhiên, mô hình TCP / IP đáng tin cậy hơn.
- 3. OSI theo cách tiếp cận dọc còn TCP/IP tiếp cận theo chiều ngang.
- 4. Mô hình OSI có lớp Trình bày và lớp Phiên riêng biệt. TCP/IP không có lớp Trình bày hoặc lớp Phiên riêng biệt.
- 5. OSI có lớp vận chuyển được định hướng kết nối còn TCP/IP có lớp vận chuyển là cả kết nối hướng và không kết nối.
- 6. OSI có lớp mạng là cả kết nối hướng và kết nối ít hơn còn TCP/IP có lớp mạng là kết nối ít hơn.
- 7. OSI là một mô hình tham chiếu xung quanh các mạng được xây dựng. Nói chung, nó được sử dụng như một công cụ hướng dẫn. Mô hình TCP/IP, theo cách thức triển khai mô hình OSI.
- 8. Lớp mạng của mô hình OSI cung cấp cả dịch vụ hướng kết nối và dịch vụ không kết nối. Lớp Mạng trong mô hình TCP/IP cung cấp dịch vụ không kết nối.
- 9. Mô hình OSI có vấn đề về việc gắn các giao thức vào mô hình. Mô hình TCP/IP không phù hợp với bất kỳ giao thức nào.
- 10. Các giao thức được ẩn trong mô hình OSI và dễ dàng thay thế khi công nghệ thay đổi còn trong giao thức TCP/IP thay thế là không dễ dàng.
- 11. Mô hình OSI xác định các dịch vụ, giao diện và giao thức rất rõ ràng và phân biệt rõ ràng giữa chúng. Nó là giao thức độc lập. Trong TCP/IP, các dịch vụ, giao diện và giao thức không được phân tách rõ ràng. Nó cũng phụ thuộc vào giao thức.
- 12. mô hình OSI có 7 lớp còn mô hình TCP/IP có 4 lớp.
#### 2.3 So Sánh 2 sơ đồ :
![alt](https://i.imgur.com/90NbNhk.png)
