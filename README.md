# Báo cáo 
## Cơ chế hoạt động của internet
Khi chúng ta cần truy cập vào nội dung một trang web nào đấy, máy tính sẽ gửi yêu cầu qua máy chủ.
Máy chủ là nơi sẽ lưu trữ toàn bộ nội dung cũng như thông tin các trang web, nó hoạt động như là ổ cứng của máy tính.
Khi yêu cầu được gửi đến máy chủ thì nó sẽ xuất dữ liệu cũng như thông tin của mình vừa yêu cầu 
## Giải thích về protocol của HTTP/HTTPS
#### HTTP 
Là giao thức truyền tải siêu văn bản có thể dưới dạng 
* Văn bản 
* Âm thanh
* Hình ảnh
* Video 
=> Từ Web Server tới trình duyệt web của người dùng và ngược lại 

HTTP có bộ giao thức TCP/IP
HTTP truy cập website sẽ hoạt động theo mô hình 
* Server (máy chủ )
* Client (máy khách)

Khi truy cập trang web với giao thức HTTP,  trình duyệt sẽ kết nối theo kiểu client và server
Có thể hiểu mình là client sẽ có nhu cầu truy cập vào một trang web nào đấy thì sẽ thông qua địa chỉ là IP (là tên miền DNS cung cấp) sẽ gửi yêu cầu của mình 
đến Server, sao khi Server nhận được sẽ trả ra các nội dung của trang web đấy : 

* Văn bản 
* Ảnh 
* Video 
* Âm thanh ...

Trong quá trình trao đổi thông tin,Server sẽ mặc định thừa nhận địa chỉ IP chính là website của mình 
mà không cần qua sự xác thực và những thông tin ấy cũng không có sự bảo mật hay là mang tính chất mã hoá. 
Đó cũng là nguyên nhân sẽ dẫn đến một số hậu quả như là hacker tấn công đánh cắp thông tin người dùng 

### HTTPS
Cũng như HTTP là một giao thức truyền tải siêu văn bản nhưng mang tính chất của sự an toàn.
Thực tế cũng có thể nói đây là giao thức HTTP nhưng được tích hợp thêm sự bảo mật SSL hoặc TLS (hiện tại đây là các tiêu chuẩn bảo mật hàng đầu), có sự mã hóa
và thêm tính bảo mật. 
## Browser 
### Cơ chế hoạt động
Web browser còn được gọi là trình duyệt của internet 
* The user interface : bao gồm thanh địa chỉ, nút back/ forward, bookmarking, menu...
*  The browser engine: thực hiện các hành động tương tác giữa UI (giao diện người dùng) và rendering engine (công cụ dựng hình).
*  The rendering engine : chịu trách nhiệm hiển thị nội dung yêu cầu.
*  Networking : gửi và nhận yêu cầu phản hồi qua mạng thông qua các giao thức như HTTP
*  UI backend : là giao diện chung nhưng không phụ thuộc vào 1 nền tảng cụ thể nào cả 
*  JavaScript interpreter: sử dụng để phân tích và thực thi mã Javascript. 
*  Data storage: để browsers lưu các loại dữ liệu cục bộ, chẳng hạn như cookie.
Web browser gửi và nhận thông tin từ các thành phần của web. Thông tin nhận được sẽ được hiển thị 
lên trên trình duyệt. Dữ liệu sẽ được truyền với giao thức siêu văn bản (HTTP) 

### Sự khác nhau giữa các browser 
#### Google Chrome
Web browser phổ biến nhất. Sự phổ biến của Chrome có thể được giải thích với 1 số lý do cơ bản
* Tốc độ duyệt web nhanh
* Dễ dàng tích hợp với tài khoản Google cá nhân

#### Safari
* Safari có mặt ở một số thiết bị của Apple : Mac,iPad và iPhone
* Safari là Web browser di động phổ biến nhất ở Mỹ

#### Microsoft Edge (trước đây là Internet Explorer)

* Trình duyệt hàng đầu mới của Microsoft.
*  Web browser này là tiêu chuẩn cho mọi thiết bị sử dụng hệ điều hành Windows của Microsoft.
*  Edge được xây dựng trên nền tảng trình duyệt Chromium
*  Nền tảng này cũng làm nền tảng cho Chrome và các trình duyệt khác.

#### Mozilla Firefox 

* Từng là trình duyệt phổ biến ở Mỹ 
*  Firefox gần đây đã mất thị phần vào tay Chrome và Safari.
*  Mặc dù độ phổ biến giảm Firefox vẫn tự hào có một lượng nhỏ và trung thành trong khi cung cấp 
các tính năng trình duyệt tương tự như các đối thủ cạnh tranh thống trị hơn của nó.

#### Opera
* Không phải là trình duyệt phổ biến nhất 
*  Opera xây dựng sự ổn định cho người dùng trong nhiều năm qua. 
*  Chẳng hạn như proxy và trình chặn quảng cáo được tích hợp sẵn


#### Trình duyệt an toàn Avast
* Tất cả các trình duyệt liệt kê ở trên dều có chế độ duyệt web riêng tư . 
*  Avast có tính năng mặc định cho trình duyệt web trở nên an toàn và riêng tư
*  Danh sách bảo mật về quyền riêng tư 
 * Tích hợp chống lừa đảo  
 * Theo dõi web và lấy dấu vân tay trình duyệt 
 * Có sự trình chặn quảng cáo tích hợp và cung cấp các cảnh báo bảo mật tự động dễ dàng được thiết lập

### Cơ chế hoạt động của DNS và domain
#### DNS 
* Khi muốn truy cập 1 trang web có địa chỉ là allgrow-labo.jp
* Người dùng gửi yêu cầu tìm kiếm địa chỉ IP với tên miền allgrow-labo.jp tới Name Server cục bộ
* Máy chủ domain cục bộ sẽ tìm kiếm trong kho dữ liệu xem có cơ sở dữ liệu chuyển đổi từ tên miền sang địa chỉ IP của tên miền mà người dùng yêu cầu hay không.
*  Nếu "có" thì nó sẽ gửi trả lại địa chỉ IP của máy có tên miền đó
*  Nếu "không có" nó sẽ hỏi lên các máy chủ tên miền ở mức cao nhất (ROOT). Máy chủ tên miền 
 có mức cao nhất là ROOT sẽ chỉ cho máy chủ tên miền cục bộ địa chỉ quản lý có đuôi ".jp"
*  Máy chủ tên miền cục bộ gửi yêu cầu đến máy chủ quản lý tên miền Nhật Bản ".jp" tìm tên miền "allgrow-labo.jp"
*  Máy chủ tên miền cục bộ sẽ hỏi máy chủ quản lý tên miền "jp" địa chỉ IP của tên miền "allgrow-labo.jp" và gửi trả lại cho máy chủ tên miền cục bộ.
*  Máy chủ tên miền cục bộ gửi thông tin đến máy của người dùng.
* Người dùng sử dụng địa chỉ IP này kết nối đến server chứa website có địa chỉ .


#### Domain 
* Domain là một địa chỉ của trang web cụ thể, khi nhập một tên miền của 1 doanh nghiệp nào đấy vào thanh tìm kiếm, Google sẽ đưa chúng ta đến trang web mà địa chỉ vừa mới được nhập 

### Giải thích về hosting server
#### Khái niệm về hosting : 
* Hosting có nghĩa là "cung cấp host".Các định nghĩa về hosting đầy đủ phải là hosting service, nhưng thông thường được viết tắt là hosting.

#### Hoạt động của Hosting
* Hosting sẽ cung cấp cho client 1 server lưu trữ  
* khi website hoạt động trên internet sẽ giúp truyền tải các nội dung, tập tin từ phía server lên trình duyệt giúp người dùng đọc và hiểu được thông tin trên website. 
