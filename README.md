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
Nền tảng của MicroService là xây dựng một ứng dụng mà ứng dụng này tổng hợp của nhiều service nhỏ và độc lập có thẻ chạy riêng biệt, phát triển và triển khai độc lập. Microservice có nhiều ưu điểm rỗ rệt so với kiến trúc một khối truyền thống:
+Về tính bảo mật nó sẽ có độ an toàn cao hơn bởi vì mỗi feature nằm ở từng service riêng biệt và mỗi service có cơ chế bảo mật riêng và khác nhau. nên sẽ rất khó sâm nhập vào hết được
+Tính mở rộng thì rõ ràng là microservice sẽ có độ tuỳ biến và mở rộng cao hơn hẳn.
+Có thể sử dụng nhiều database hạn chế được vấn đề phình to của csdl
Tuy nhiên việc testing và deploy còn tương đối phức tạp so với kiến trúc khối.

*Thiết kế MicroService: kích cỡ, phạm vi, tính năng là những điều vô cùng quan trọng trong việc xây dựng ứng dụng với MicroService 
Một số chỉ dẫn khi thiết kế MicroService:
- Single Responsibility Principle (SRP): một service với phạm vi và chức năng giới hạn, tập trung vào một nhiệm vụ giúp quá trình phát triển và triển khai dịch vụ trở nên nhanh chóng hơn.
- Trong quá trình thiết kế, ta nên xác định và giới hạn các services theo chức năng nghiệp vụ thực tế (theo Domain-Driven-Design)
- Đảm bảo microservices có thể phát triển và triển khai độc lập
- Mục tiêu của thiết kế là phạm vi của microservices phục vụ một nghiệp vụ chứ không chỉ đơn giản làm các dịch vụ nhỏ hơn. Kích thước hợp lý của một service là kích thước đủ để đáp ứng yêu cầu của một chức năng trong hệ thống.
- Khác với services trong SOA, một microservice không nên có quá nhiều hàm hay chức năng hỗ trợ xung quanh và định dạng thông báo/ gửi tin (messaging) đơn giản.
- Một cách tốt là có thể bắt đầu với services to có phạm vi rộng rồi chia nhỏ dần (dựa theo nghiệp vụ thực tế của hệ thống)

Liên lạc giữa MicroService: nó yêu cầu có một chế truyền tin đơn giản và nhẹ
-gửi tin đồng bộ- REST, Thrift
-gửi tin bất đồng bộ- AMQP,STOMP, MQTT
-các kiểu tin nhắn- JSON, XML, Thrift, ProtoBuf, Avro
-Service Contracts- định nghĩa service Interfaces- Swagger,RAML
*kết nối microservice:
kết nối và giao tiếp giữa các microservice là cần thiết vì tác vụ gồm nhiều tác động khác nhau lên các services. Một số kiểu mẫu giao tiếp trong microservice như:
- Point-to-Point - kết nối trực tiếp giữa các services: vấn đề của kiểu giao tiếp này là những yêu cầu như xác thực người dùng, điều tiết, giám sát,... phải được xây dựng tại tất cả microservices, việc trên dẫn đến lập các tính năng chung, mỗi microservices có thể trở nên phức tập; không có cách quản lý, kiểm soát giao tiếp giữa các services; thường thì việc kết nối trong microservices được coi là anti-pattern khi áp dụng cho ứng dụng.
- API -Gateway: cổng kết nối API che giấu đi cấu trúc bên trong của ứng dụng, cung cấp các lợi thế như cung cấp một lớp trừu tượng hóa các microservices; định tuyến và chuyển đổi tin nhắn gọn nhẹ ở cấp gateway; một điểm tập trung cho các chức năng chung không mang tính nghiệp vụ kinh doanh như bảo mật, giám sát và điều tiết; giúp microservices trở nên gọn nhẹ vì các chức năng chung không mang tính nghiệp vụ đều chuyển sang Gateway. Vì vậy nó là hoàn toàn phù hợp khi triển khai cổng kết nối API làm điểm kết nối duy nhất với hệ thống ứng dụng trên nền tảng Microservices. Đặc điểm: cổng kết nối API làm nhiệm vụ định tuyến các yêu cầu, kết hợp và chuyển đổi các giao thức, tất cả yêu cầu từ client đều đi qua cổng kết nối API
https://techmaster.vn/posts/33603/xay-dung-microservices-su-dung-cong-ket-noi-api-api-gateway

- Message Broker - người truyền tin trung gian: giao tiếp giữa người gửi/ người nhận được tạo ra bởi message broker qua các tiêu chuẩn truyền tin bất đồng bộ như AMQP, MQTT,...
* Quản lý cơ sở dữ liệu phân tán: đối với kiến trúc một khối truyền thống ứng dụng sẽ lưu trữ cơ sở dữ liệu tập trung duy nhất, còn đối với kiến trúc MicroService các chức năng được tách ra và nếu sử dụng cùng một CSDL thì nó không còn độc lập nữa, do đó mỗi microservice phải có CSDL riêng. Lưu ý: một microservice chỉ có thể truy xuất vào cơ sở dữ liệu của riêng nó mà không có quyền truy xuất vào cơ sở dữ liệu của microservice khác và khi cần phải cập nhật CSDL thì CSDL của microservice khác chỉ nên được cập nhật qua API của những dịch vụ này(không trực tiếp thay đổi cơ sở dữ liệu).
* Quản trị phân tán: trong quản trị SOA, có hai kiểu quản trị phổ biến là:
+ Quản trị khi thiết kế-định nghĩa và kiểm soát việc tạo service, thiết kế và thực thi các chính sách của service.
+ Quản trị khi triển khai/chạy-khả năng đảm bảo các chính sách của service trong quá trình hoạt động
Tuy nhiên, Microservice được xây dựng độc lập và phân tán nên không cần một tiêu chuẩn thiết kế và phát triển chung. Trong đó khả năng quản trị phân tán của microservice thì không cần phải có một hệ quản trị tập trung khi thiết kế; có thể tự quyết định thiết kế và phát triển của nó; kiến trúc ủng hộ và hỗ trợ việc chia sẻ các services chung hay có thể tái sử dụng; một số mặt của quản trị trong quá trình hoạt động có thẻ phát triển ở cấp APT Gateway
*Service Registry & Service Discorvery (Truy Tìm Dịch Vụ): nếu bạn cần xác định được vị trí của một service trong quá trình chạy thì ta dùng tới service registry, nó giữ các thực thể microservice và địa chỉ của chúng. Để tìm các microservice đang tồn tại và địa điểm của chúng, chúng ta cần một quy trình truy tìm dịch vụ. Trong đó ta có hai mô hình là Client-side Discovery và Server-side Discovery.
- Client-side Discovery: với mô hình này, client hay API Gateway lấy thông tin địa điểm của một thực thể service bằng truy vấn service registry.
- Server-side Discovery: với mô hình này, client hay API Gateway gửi yêu cầu lên một component, component này sẽ gọi service registry và quyết định địa điểm của các microservice.
* Deployment: để triển khai dịch vụ thì ta yêu cầu:



Các mặt hạn chế của Microservice







Các mục cần tìm hiểu:
- tìm hiểu chung về MicroService 
- so sánh MicroService với kiến trúc một khối truyền thống
- cách xây dựng một ứng dụng với kiến trúc MicroService
- liên lạc giữa MicroService
- kết nối, giao tiếp giữa các services
-quản trị phân tán
- truy tìm dịch vụ
- deployment
- bảo mật


https://martinfowler.com/articles/microservices.html

Để chia tách một ứng dụng truyền thống thành các Microservice:
- Điều kiện cần: có một kiến trúc cho hệ thống rõ ràng; CI/CD tools; Organization phù hợp để phát triển và vận hành hệ thống.

ngày 26/12


1 Đặt vấn đề
Tại sao ta phải dùng microservices???
Câu chuyện về cái bồn cầu=>https://toidicodedao.com/2017/02/21/tong-quan-micro-service/
Micro là rất nhỏ, service là dịch vụ, vậy microservice nghĩa là… dịch vụ vô cùng nhỏ. Nói đơn giản, microservice là một kiếu kiến trúc phần mềm. Các module trong phần mềm này được chia thành các service rất nhỏ (microservice).
2 Giới thiệu về kiến trúc một khối truyền thống 
(lấy hỉnh ảnh từ chương 1)
Thoát khỏi địa ngục nguyên khối
Kiến trúc của ứng dụng FTGO: FTGO có kiến trúc lục giác, cốt lõi của ứng dụng bao gồm logic nghiệp vụ, xung quanh là các bộ điều hợp triển khai UI và giao diện với các hệ thống bên ngoài, chẳng hạn như các ứng dụng di động và dịch vụ đám mây để thanh toán, nhắn tin và email.
=> đây là ví dụ về phong cách nguyên khối được sử dụng rộng rãi của kiến trúc phần mềm
Tìm hiểu lợi ích của kiến trúc nguyên khối:
- Phát triển đơn giản - IDE và các công cụ dành cho nhà phát triển khác được tập trung vào việc xây dựng một ứng dụng duy nhất.
- Dễ dàng thực hiện các thay đổi căn bản cho ứng dụng - Bạn có thể thay đổi mã và lược đồ cơ sở dữ liệu, xây dựng và triển khai.
- Đơn giản để kiểm tra - Các nhà phát triển đã viết các thử nghiệm đầu cuối đã khởi chạy ứng dụng, gọi API REST và thử nghiệm UI với Selenium.
- Đơn giản để triển khai - Tất cả các nhà phát triển phải làm là sao chép tệp WAR vào máy chủ đã cài đặt Tomcat.
- Dễ dàng chia tỷ lệ - FTGO chạy nhiều phiên bản của ứng dụng đằng sau bộ cân bằng tải.
=> Vậy tại sao hiện nay đối với FTGFO ta lại gọi là địa ngục nguyên khối???
Theo thời gian việc phát triển, thử nghiệm, triển khai và nhân rộng trở nên khó khăn hơn nhiều, vì sao???
Kiến trúc nguyên khối có một hạn chế rất lớn: khi triển khai phát triển làm cho cơ sở mã lớn hơn, các nhóm phát triển nhỏ trở thành nhiều nhóm Scrum, mỗi nhóm hoạt động trên một chức năng cụ thể làm cho FTGO ở trong địa ngục nguyên khối, phất triển chậm và đau đớn.
FTGO là một ứng dụng phức tạp nên việc sửa lỗi, triển khai tính năng mới trở nên khó khăn và tốn thời gian. 
Bên cạnh đó kiến trúc nguyên khối còn khiến cho FTGO phát triển chậm, làm con đường đi từ cam kết đến triển khai dài và gian nan, mở rộng quy mô là khó khăn, việc cung cấp một nguyên khối đáng tin cậy là một thách thức, bị khóa vào ngăn xếp công việc ngày càng lỗi thời( kiến trúc buộc họ phải sử dụng một chồng công nghệ ngày càng trở nên lỗi thời, gây khó khăn cho việc áp dụng các khuôn khổ và ngôn ngữ mới)
=> từ đó FTGO áp dụng kiến trúc microservice để giải cứu!!!
*Kiến trúc microservice
- (tìm hiểu thêm về kiến trúc của microservice theo mô hình chia 3 trục X,Y,Z)
=> kiến trúc microservice là một kiểu kiến trúc có chức năng phân rã một ứng dụng thành một tập hợp các dịch vụ, điều quan trọng của một dịch vụ là có một tập hợp trách nhiệm tập trung, gắn kết.
* tìm hiểu chi tiết về kiến trúc microservice.
- microservice như một dạng modun: tính modun là điều cần thiết khi phát triển các ứng dụng lớn, phức tạp. Microservice sử dụng các dịch vụ như là đơn vị của modun, nên việc bảo toàn tính modun của ứng dụng theo thời gian sẽ dễ dàng hơn
- mỗi dịch vụ có cơ sở dữ liệu riêng: đối với microservice các dịch vụ được ghép nối lỏng lẻo và chỉ giao tiếp qua API, mỗi dịch vụ có kho dữ liệu riêng nên ta có thể tránh được các điểm như nhà phát triển có thể thay đổi lược đồ của dịch vụ mà khồng phải phối hợp nhà phát triển làm việc trên các dịch vụ khác; dịch vụ sẽ không bao giờ bị chặn vì dịch vụ khác khóa cơ sở dữ liệu.
*Tìm hiểu thông qua kiến trúc Microservice FTGO:
*So sánh kiến trúc Microservice và SOA: tuy ta thấy rằng SOA và microservice là các kiểu kiến trúc cấu trúc một hệ thống như một tập hợp các dịch vụ nhưng, ta có bảng so sánh( chương 1 phần 1.4.5)
* Lợi ích và hạn chế của microservice:
- Lợi ích:
+ Nó cho phép phân phối và triển khai liên tục các ứng dụng lớn, phức tạp ( microservice có ba cách cho phép phân phối triển khai là 
.kiểm tra theo yêu cầu của phân phối/ triển khai liên tục: kiểm tra tự động dễ viết hơn nhiều và thực thi nhanh hơn giúp ứng dụng it lỗi hơn
.triển khai theo yêu cầu của việc phân phối triển khai liên tục: mỗi dịch vụ được triển khai độc lập với các dịch vụ khác giúp việc triển khai dễ dàng hơn nhiều
.cho phép các nhóm phát triển có thể tự chủ và kết nối lỏng lẻo: giúp tốc độ phát triển cao hơn
=>đem lại nhiều lợi ích kinh doanh như giảm thời gian đưa ra thị trường, phản ứng nhanh với phản hồi từ khách hàng, cung cấp được dịch vụ đáng tin cậy, làm hài lòng nhân viên hơn vì được làm việc cung cấp các tính năng có giá trị thay vì chữa cháy.
+ Dịch vụ là nhỏ và dễ dàng duy trì.
+ Dịch vụ có khả năng mở rộng độc lập.
+ Cách ly lỗi tốt hơn vì nếu có rò rỉ, gặp lỗi trong một dịch vụ thì chỉ ảnh hưởng đến dịch vụ đó.
+ Kiến trúc microservice cho phép các nhóm được tự chủ.
+ Nó cho phép dễ dàng thử nghiệm và áp dụng các công nghệ mới
- Hạn chế:
+ Tìm đúng bộ dịch vụ là một thách thức: Microservice không có một thuật toán cụ thể, rõ ràng để phân tách một hệ thống thành các dịch vụ. Nếu ta phân tách không chính xác sẽ làm hệ thống trở thành một khối nguyên khối phân tán mà chứa cả nhược điểm của kiến trúc nguyên khối và microservice.
+ Các hệ thống phân tán rất phức tạp, khiến cho việc phát triển, thử nghiệm và triển khai trở nên khó khăn: dịch vụ phải có cơ chế truyền thông liên tiến trình và phải được thiết kế để xử lý lỗi một phần và xử lý dịch vụ từ xa không khả dụng hoặc có độ trễ cao.
+ Triển khai các tính năng trải rộng trên nhiều dịch vụ đòi hỏi sự phối hợp cẩn thận.
+ Quyết định khi nào nên áp dụng kiến ​​trúc microservice là khó khăn.
=> vậy làm sao để quyết định lựa chọn kiểu kiến trúc nào cho phù hợp??? một cách rất tốt đó là sử dụng ngôn ngữ mẫu. Nó là một tập hợp các mẫu giúp bạn kiến trúc một ứng dụng bằng kiến trúc microservice, giúp bạn quyết định có sử dụng kiến trúc microservice không, nếu bạn chọn kiến trúc microservice, ngôn ngữ mẫu sẽ giúp bạn áp dụng hiệu quả.
=> Kết luận: đối với những ứng dụng lớn, phức tạp thì microservice là lựa chọn tốt nhất.
3. Chiến lược phân rã - decomposition
4. Khu dịch vụ vi mô - microxervice chassis
5. Phát triển logic kinh doanh - developing business logic
6. Tìm nguồn cung ứng sự kiện - event sourcing
7. IPC
8. CQRS-MONGODB
https://microservices.io/patterns/data/cqrs.html
9. APT Gateway
Vấn đề: khi là một cấu trúc nguyên khối thì API tiếp xúc với khách hàng là API nguyên khối, nhưng khi triển khai Microservice thì không còn một API nào nữa vì mối dịch vụ đều có API riêng nên đã đặt ra khó khăn trong việc thiết kế API bên ngoài của ứng dụng
Ý tưởng chính của API Gateway là sử dụng một cổng truyền tin gọn nhẹ như một điểm vào chính cho tất cả các khách hàng, người dùng và triển khai những chức năng chung mà không liên quan đến nghiệp vụ đặc thù ở cấp Gateway này.
API Gateway chịu trách nhiệm định tuyến các request, tổng hợp và chuyển đổi giao thức. Nó như một tổng đài để điều phối các request.
Tại sao nên dùng API Gateway: khi ta không sử dụng nó thì client sẽ gửi request trực tiếp tới service cụ thể nào đó và dẫn đến một số rắc rối với client như:
+ Phần code phía client sẽ trở nên phức tạp vì phải tracking nhiều endpoint.
+ Sẽ tạo sự kết nối giữa client và backend. Client cần biết được các services đó đc phân chia như thế nào -> rất khó cho việc maitain của client và refactor service.
+ Mỗi một service sẽ phải handle nhiều vấn đề liên quan như authentiaction, SSL hay client rate limiting.
Tổng quan về mẫu cổng API:
- Cổng API chịu trách nhiệm định tuyến yêu cầu. Bên cạnh đó một API có thể triển khai một số thao tác API bằng cách sử dụng thành phần API. Cổng API còn có thể thực hiện giao thức dịch, có th cũng cấp API RESTful cho các khách bên ngoài
- Kiến trúc cổng API: có kiến trúc mô dun nhiều lớp, bao gồm 2 lớp là lớp API và lớp chung. Lớp API gồm một hoặc nhiều mô dun API độc lập, mỗi modun thực hiện một API cho một khách hàng cụ thể; lớp chung thực hiện chức năng chia sẻ. bao gồm các chức năng cạnh như xác thực.
Mỗi modun API thực hiện hoạt động API theo một trong hai cách: Một số hoạt động API ánh xạ trực tiếp đến hoạt động API dịch vụ duy nhất. Một mô-đun API thực hiện các hoạt động này bằng cách định tuyến các yêu cầu đến hoạt động API dịch vụ tương ứng. Nó có thể định tuyến các yêu cầu bằng cách sử dụng một mô đun định tuyến chung để đọc tệp cấu hình mô tả các quy tắc định tuyến.

Một mô-đun API triển khai các hoạt động API phức tạp hơn khác bằng cách sử dụng thành phần API. Việc triển khai hoạt động API này bao gồm mã tùy chỉnh. Mỗi triển khai hoạt động API xử lý các yêu cầu bằng cách gọi nhiều dịch vụ và kết hợp các kết quả.
Mô hình sở hữu cổng API?
Người chịu trách nhiệm phát triển cổng API và hoạt động của nó, chẳng hạn như:
+ Cho một nhóm riêng chịu trách nhiệm về cổng API
+ Cách tốt hơn là dành cho nhóm khách hàng, nhóm các nhóm API di dộng, web và công cộng, sở hữu modun API hiển thị API của họ, khi họ thay đổi ứng dụng khách, họ có thể thay đổi modun API và không yêu cầu nhóm cổng API thực hiện các thay đổi
* Ưu và nhược điểm của API Gateway
Ưu điểm:
+ Cách ly khách hàng khỏi cách ứng dụng được phân vùng vào microservice
+ Cách ly khách hàng khỏi vấn đề xác định vị trí của các trường hợp dịch vụ
+ Cung cấp API tối ưu cho từng khách hàng
+ Giảm số lượng yêu cầu / roundtrips. Ví dụ: cổng API cho phép khách hàng truy xuất dữ liệu từ nhiều dịch vụ với một chuyến đi khứ hồi. Ít yêu cầu hơn cũng có nghĩa là ít chi phí hơn và cải thiện trải nghiệm người dùng. Cổng API rất cần thiết cho các ứng dụng di động.
+ Đơn giản hóa máy khách bằng cách di chuyển logic để gọi nhiều dịch vụ từ máy khách đến cổng API
+ Dịch từ một giao thức API thân thiện với web công cộng của tiêu chuẩn thành một bất kỳ giao thức nào được sử dụng trong nội bộ
Nhược điểm:
+ Độ phức tạp tăng lên - cổng API là một phần chuyển động khác phải được phát triển, triển khai và quản lý
+ Thời gian phản hồi tăng lên do bước nhảy mạng bổ sung thông qua cổng API - tuy nhiên, đối với hầu hết các ứng dụng, chi phí cho một vòng tròn thêm là không đáng kể.
* Netflix - ví dụ về cổng API:














10. Triển khai dịch vụ với docker - deploying services with docker
11. Tái cấu trúc Microservice- Refactoring to Microservice














observability patterns
effective software testing


