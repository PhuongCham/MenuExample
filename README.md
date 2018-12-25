MÔ HÌNH CHẠY NHIỀU LOẠI CƠ SỞ DỮ LIỆU - MULTE DATABASE
là nền tảng xử lý dữ liệu hỗ trợ nhiều mô hình dữ liệu, xác định các tham số về cách tổ chức sắp xếp thông tin trong cơ sở dữ liệu, nó cho phép những nhóm và những người dùng khác đáp ứng các yêu cầu ứng dụng khác nhau mà không cần phải triển khai các hệ thống cơ sở dữ liệu khác nhau. Trái ngược với mô hình cơ sở dữ liệu quan hệ thì nó không lưu trữ dữ liệu thống nhất trong cấu trúc bảng dựa trên hàng vì vậy nó loại bỏ vấn đề phân mảnh và đảm bảo tính nhất quán. Các cơ sở dữ liệu đa mô hình hàng đầu: ArangoDB, OrientDB, MarkLogic, Azure Cosmos DB,FoundationDB, Couchbase, Apache Ignite là một số cơ sở dữ liệu đa mô hình hàng đầu.
Một số chức năng phổ biến của mô hình nhiều loại cơ sở dữ liệu:
-Lưu trữ, sao lưu và khôi phục dữ liệu
-Cơ chế truy vấn và lập chỉ mục: cơ chế lập chỉ mục để đảm bảo truy vấn hiệu quả.
-Giao dịch ACID (Atomicity, Consistency, Isolation, Durability)- nguyên tử, tính nhất quán, cách lý và độ bền: các cơ sở dữ liệu có khả năng chịu lỗi, đảm bảo tính hợp lệ trong trường hợp mất điện hoặc lỗi không mong muốn.
-Tích hợp: cho phép pháp triển các mô hình dữ liệu họ cần trên một mặt duy nhất, có thể tích hợp dữ liệu từ nhiều nguồn và ở nhiều định dạng.
-Các tính năng bảo mật nâng cao: các tính năng bảo mật nâng cao như cơ chế kiểm toán và mã hóa topnotch.
*Tại sao nên sử dụng mô hình sử dụng nhiều loại cơ sở dữ liệu?
-Tính linh hoạt: chúng hợp nhất các loại dữ liệu khác nahu trong một nền tảng duy nhất giúp tối đa hóa tài nguyên
-Chi phí vận hành tối thiểu
- ACID đảm bảo tính nhất quán của dữ liệu
- Các thành phần khác có thể thu nhỏ độc lập
- Cải thiện độ tin cậy.
* Tìm hiểu cụ thể các mô hình hàng đầu
+ ArangoDB: nó có thể kết hợp các mô hình khác nhau và các tính năng của chúng trong một truy vấn vì nó sử dụng một lõi và cùng ngôn ngữ truy vấn cho tất cả các mô hình dữ liệu. Ưu điểm: trình điều khiển JAVA mạnh mẽ(đồng bộ và không đồng bộ), có thể mở rộng AranggoDB bằng Javascript chạy trực tiếp trên máy chủ, có thể sử dụng giao dịch ACID cho các hoạt động truy xuất và sửa đổi dữ liệu ngắn và nhỏ trong ArangoDB
+ OrientDB: là hệ thống quản lý cơ sở dữ liệu NoQuery kết hợp sức mạnh của đồ thị và các mô hình tài liệu, khóa, giá trị,..., nó cung cấp sự an toàn trong tất cả các dữ liệu bí mật qua việc sử dụng xác thực, mật khẩu và dữ liệu tại phần còn lại. OrientDB được viết hoàn toàn bằng Java và có thể chạy trên mọi nền tảng mà không cần cấu hình hoặc cài đặt. 
+ MarkLogic: kết hợp sự linh hoạt của NoQuery với các tính năng doanh nghiệp cứng và các khả năng nâng cao. Nó hỗ trợ JavaScript và JSON phía máy chủ. Bitemporal cho phép các doanh nghiệp giảm thiểu rủi ro bằng cách xem dữ liệu theo thời gian
+ Azure Cosmos DB: tự lập chỉ mục tất cả dữ liệu và cho phép dử dụng API yêu thích
+FoundationDB: được thiết kế để thực hiển xử lý giao dịch
+ Couchbase: xây dựng với công nghệ NoQuery mạnh nhất, nó cực kỳ đơn giản để triển khai và quản lý, tính năng nhân rộng được tích hợp và tự động xảy ra.
+ Ignite: là cơ sở dữ liệu phân tán, bộ nhớ đệm và nền tảng xử lý trung vào bộ nhớ, do đó nó sử dụng RAM làm tầng lưu trữ và xử lý mặc định.
MICROSERVICE - KIẾN TRÚC NHIỀU DỊCH VỤ NHỎ
https://techmaster.vn/posts/34410/microservices-thuc-tien-tu-thiet-ke-den-trien-khai
MicroService chia nhỏ ứng dụng một khối thành nhiều dịch vụ nhỏ, nó chịu ảnh hưởng lớn đên quan hệ ứng dụng và cơ sở dữ liệu, thay vì dùng chung một CSDL giữa các dịch vụ, mỗi dịch vụ sẽ có CSDL riêng, từng dịch vụ nhỏ có thể tùy chọn công nghệ lưu trữ dữ liệu tối ưu nhất.
MicroService tương tự như kiến trúc hướng dịch vụ đều là một tập hợp các dịch vụ.
Ưu điểm của MicroService:
- giảm sự rối rắm của hệ thống lớn
- chia nhỏ dễ quản lý, bảo trì nâng cấp, tự do chọn nâng cấp công nghệ mới.
- dịch vụ nhỏ sẽ định ra ranh giới rõ ràng dưới dạng RPC hay API hướng thông điệp
- thúc đẩy tách rạch ròi các khối chức năng
=>mỗi dịch vụ nhỏ sẽ phát triển dễ hơn, nhanh hơn, dễ viết mã kiểm thử tự động.
Nhược điểm của MicroService: nhược điểm của nó đến từ đặc điểm hệ thống phân tán, việc chia nhỏ dịch vụ làm dẫn đến manh mún, vụn vặt khó kiểm soát
- phải xử lý sự cố khi kết nối chậm, lỗi khi thông điệp không gửi được hoặc thông điệp gửi đến nhiều đích đến vào các thời điểm khác nhau
- việc đảm bảo giao dịch phân tán, cập nhật dữ liệu đúng dắn có nhiều khó khăn
- theo nguyên tắc CAP(consistency-availablity-partiitin tolerance) thì giao dịch phân tán sẽ không thể thỏa mãn( dữ liệu ở điểm khác nhau trong mạng phải giống nhau, yêu cầu gửi đi phải có hồi đáp, hệ thống vẫn hoạt động đc ngay cả khi mạng bị lối)
- cần luôn kiểm tra mức độ ràng buộc giữa các dịch vụ mềm dẻo hơn hay cứng nhắc, lệ thuộc hơn.
- nếu có sự ràng buộc giữa các dịch vụ nhỏ thì việc bảo trì, kiểm thử sẽ phức tạp
=> kiến trúc một khối sẽ hữu hiệu đối với ứng dụng đơn giản it chức năng
*So sánh kiến trúc một khối truyền thống và kiến trúc MicroService:
Nền tảng của MicroService là xây dựng một ứng dụng mà ứng dụng này tổng hợp của nhiều service nhỏ và độc lập có thẻ chạy riêng biệt, phát triển và triển khai độc lập

Thiết kế MicroService: kích cỡ, phạm vi, tính năng là những điều vô cùng quan trọng trong việc xây dựng ứng dụng với MicroService 
Một số chỉ dẫn khi thiết kế MicroService:
- Single Responsibility Principle (SRP): một service với phạm vi và chức năng giới hạn, tập trung vào một nhiệm vụ giúp quá trình phát triển và triển khai dịch vụ trở nên nhanh chóng hơn.
- Trong quá trình thiết kế, ta nên xác định và giới hạn các services theo chức năng nghiệp vụ thực tế (theo Domain-Driven-Design)
- Đảm bảo microservices có thể phát triển và triển khai độc lập
- Mục tiêu của thiết kế là phạm vi của microservices phục vụ một nghiệp vụ chứ không chỉ đơn giản làm các dịch vụ nhỏ hơn. Kích thước hợp lý của một service là kích thước đủ để đáp ứng yêu cầu của một chức năng trong hệ thống.
- Khác với services trong SOA, một microservice không nên có quá nhiều hàm hay chức năng hỗ trợ xung quanh và định dạng thông báo/ gửi tin (messaging) đơn giản.
- Một cách tốt là có thể bắt đầu với services to có phạm vi rộng rồi chia nhỏ dần (dựa theo nghiệp vụ thực tế của hệ thống)








Các mục cần tìm hiểu:
- tìm hiểu chung về MicroService 
- so sánh MicroService với kiến trúc một khối truyền thống
- cách xây dựng một ứng dụng với kiến trúc MicroService
- liên lạc giữa MicroService
- kết nối, giao tiếp giữa các services
- quản lý cơ sở dữ liệu phân tán: đối với kiến trúc một khối truyền thống ứng dụng sẽ lưu trữ cơ sở dữ liệu tập trung duy nhất, còn đối với kiến trúc MicroService các chức năng được tách ra và nếu sử dụng cùng một CSDL thì nó không còn độc lập nữa, do đó mỗi microservice phải có CSDL riêng
-quản trị phân tán
- truy tìm dịch vụ
- deployment
- bảo mật















