**Bước 1: Xác định business context, Xác định business broblem.**

- Business Context: Công ty ABC cung cấp dịch vụ đặt xe trực tuyến và đang có nhu cầu xây dựng CAB System mới nhằm phục vụ khách hàng, tài xế và nhân viên vận hành, đồng thời đảm bảo khả năng mở rộng trong tương lai.

- Business Problem: Hệ thống hiện tại còn phụ thuộc nhiều vào thao tác thủ công, khó theo dõi chuyến đi, quản lý thanh toán chưa tập trung và khó mở rộng, dẫn đến hạn chế trong hoạt động vận hành và khả năng phát triển lâu dài của doanh nghiệp.

**Bước 2: Xác định những stacholders.**

| Stacholders | Chức năng |
|:---|---|
| **Khách hàng** | Đăng ký, đặt xe, theo dõi chuyến, thanh toán, xem lịch sử và đánh giá tài xế. |
| **Tài xế** | Quản lý hồ sơ/phương tiện, nhận chuyến, cập nhật trạng thái và vị trí trong quá trình chạy xe. |
| **Nhân viên vận hành** | Quản lý khách hàng, tài xế, phương tiện, chuyến đi; xử lý sự cố và tra cứu giao dịch. |
| **Ban lãnh đạo** | Theo dõi báo cáo về số chuyến, doanh thu, tỷ lệ hoàn thành/hủy và hiệu quả tài xế. |
| **Nhà cung cấp thanh toán bên ngoài** | Hỗ trợ xử lý các giao dịch thanh toán điện tử. |
| **Nhà cung cấp dịch vụ thông báo** | Cung cấp các kênh gửi thông báo cho khách hàng và tài xế. |
| **Business Analyst** | Làm rõ yêu cầu, phạm vi, quy trình, quy tắc nghiệp vụ và các vấn đề chưa được xác định. |

**Bước 3: Xác định các Business Goal (BG).**

| **Mã** | **Business Goal** | **Mục tiêu** |
|:---|---|---|
| **BG01** | Xây dựng nền tảng đặt xe trực tuyến mới | Thay thế những hạn chế của hệ thống hiện tại và hỗ trợ toàn bộ quy trình đặt xe. |
| **BG02** | Nâng cao hiệu quả phân công tài xế | Tự động tìm và ưu tiên tài xế phù hợp, gần khách hàng; tiếp tục tìm tài xế khác khi bị từ chối hoặc không phản hồi. |
| **BG03** | Nâng cao trải nghiệm khách hàng | Cho phép khách hàng đặt xe, theo dõi trạng thái chuyến, biết tài xế và thời gian dự kiến đến, xem lịch sử và đánh giá. |
| **BG04** | Quản lý tập trung hoạt động vận hành | Hỗ trợ nhân viên quản lý khách hàng, tài xế, phương tiện, chuyến đi và giao dịch trên một hệ thống. |
| **BG05** | Hỗ trợ thanh toán và quản lý doanh thu | Tính cước, hỗ trợ tiền mặt và thanh toán điện tử, đồng thời quản lý lịch sử giao dịch. |
| **BG06** | Đảm bảo khả năng mở rộng hệ thống | Cho phép phục vụ số lượng lớn người dùng và dễ dàng bổ sung dịch vụ, phương thức thanh toán, kênh thông báo và thành phần kỹ thuật mới. |
| **BG07** | Đảm bảo tính ổn định và bảo mật | Hệ thống hoạt động ổn định khi tải cao, bảo vệ dữ liệu và kiểm soát quyền truy cập. |
| **BG08** | Cung cấp dữ liệu phục vụ quản lý | Cung cấp báo cáo về số chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế. |

**Bước 4: Xác định scope của project.**

**In scope:**

**1. Quản lý khách hàng:**
- Đăng ký, đăng nhập.
- Cập nhật thông tin cá nhân.
- Xem lịch sử chuyến đi.
  
**2. Đặt xe**
- Nhập điểm đón, điểm đến.
- Lựa chọn loại xe.
- Gửi yêu cầu đặt xe.
- Theo dõi trạng thái chuyến đi.
  
**3. Quản lý tài xế**
- Đăng ký/tạo tài khoản.
- Quản lý hồ sơ và phương tiện.
- Cập nhật trạng thái hoạt động.
- Cập nhật vị trí.
  
**4. Tìm và phân công tài xế**  
- Xác định tài xế phù hợp.
- Ưu tiên tài xế gần khách hàng.
- Xử lý trường hợp tài xế từ chối hoặc không phản hồi.
- Thông báo khi không tìm được tài xế.
  
**5. Quản lý chuyến đi**
- Tài xế nhận/từ chối chuyến.
- Cập nhật trạng thái: đến điểm đón → đón khách → đang di chuyển → hoàn thành.
- Lưu thông tin chuyến đi.
  
**6. Tính cước và thanh toán**
- Tính số tiền phải trả.
- Thanh toán tiền mặt hoặc điện tử.
- Tích hợp nhà cung cấp thanh toán bên ngoài.
- Xử lý khi thanh toán điện tử thất bại.

**7. Thông báo**
- Thông báo trạng thái đặt xe/chuyến đi.
- Thông báo chuyến mới cho tài xế.
- Thông báo kết quả thanh toán.
- Thiết kế để có thể mở rộng thêm kênh thông báo.

**8. Quản trị và vận hành**
- Quản lý khách hàng, tài xế, phương tiện, chuyến đi.
- Theo dõi chuyến đang diễn ra.
- Xử lý chuyến bị lỗi.
- Tra cứu lịch sử giao dịch.
- Phân quyền nhân viên.

**9. Báo cáo**
- Số lượng chuyến.
- Doanh thu.
- Tỷ lệ hoàn thành/hủy.
- Hiệu quả hoạt động của tài xế.

**10. Bảo mật và khả năng mở rộng**
- Xác thực người dùng.
- Phân quyền.
- Bảo vệ dữ liệu cá nhân, vị trí và giao dịch.
- Lưu vết các thao tác quan trọng.
- Hỗ trợ mở rộng độc lập các thành phần hệ thống.
  
**Out of scope:**

- Công thức tính cước cụ thể.
- Tiêu chí ưu tiên tài xế.
- Thời gian tài xế phải phản hồi.
- Chính sách hủy chuyến.
- Cách xử lý khi mất kết nối mạng.
- Thời gian lưu trữ dữ liệu.

**Bước 5: Xác định các Bussiness Requiredment**

| **Mã** | **Business Requirement** |
|:---|---|
| **BR01** | Hệ thống phải cung cấp nền tảng đặt xe trực tuyến cho khách hàng, tài xế và nhân viên vận hành. |
| **BR02** | Hệ thống phải hỗ trợ khách hàng tạo và theo dõi yêu cầu đặt xe từ lúc yêu cầu được tạo đến khi chuyến hoàn thành. |
| **BR03** | Hệ thống phải tự động tìm và phân công tài xế phù hợp, ưu tiên tài xế gần khách hàng và có trạng thái sẵn sàng. |
| **BR04** | Hệ thống phải có cơ chế tiếp tục tìm tài xế khác khi tài xế được đề xuất không phản hồi hoặc từ chối chuyến. |
| **BR05** | Hệ thống phải hỗ trợ thực hiện chuyến, tính cước và thanh toán bằng tiền mặt hoặc phương thức điện tử. |
| **BR06** | Hệ thống phải tích hợp với nhà cung cấp thanh toán bên ngoài và không lưu trực tiếp thông tin nhạy cảm của thẻ/tài khoản thanh toán. |
| **BR07** | Hệ thống phải cung cấp thông báo cho khách hàng và tài xế về các sự kiện quan trọng trong quá trình đặt và thực hiện chuyến. |
| **BR08** | Hệ thống phải hỗ trợ nhân viên vận hành quản lý khách hàng, tài xế, phương tiện và chuyến đi. |
| **BR09** | Hệ thống phải cung cấp báo cáo hoạt động kinh doanh, bao gồm số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế. |
| **BR10** | Hệ thống phải đảm bảo bảo mật, xác thực và phân quyền đối với người dùng và các thao tác quản trị. |
| **BR11** | Hệ thống phải có khả năng mở rộng để phục vụ số lượng lớn khách hàng/tài xế và bổ sung dịch vụ, phương thức thanh toán, kênh thông báo trong tương lai. |
| **BR12** | Hệ thống phải hoạt động ổn định khi nhu cầu tăng cao và cho phép triển khai các chức năng mới từng phần mà hạn chế ảnh hưởng đến hệ thống hiện tại. |


**Bước 6: Xác định Business Process**

| **Mã** | **Business Process** | **Nội dung** |
|:---|---|---|
| **BP01** | Đặt xe | Khách hàng tạo yêu cầu đặt xe. |
| **BP02** | Tìm & phân công tài xế | Hệ thống tìm tài xế phù hợp và xử lý trường hợp từ chối/không phản hồi. |
| **BP03** | Thực hiện chuyến | Tài xế đến đón, đón khách, di chuyển và hoàn thành chuyến. |
| **BP04** | Tính cước & thanh toán | Hệ thống tính tiền và xử lý thanh toán tiền mặt/điện tử. |
| **BP05** | Thông báo | Gửi thông báo về trạng thái đặt xe, tài xế, chuyến đi và thanh toán. |
| **BP06** | Quản lý vận hành | Nhân viên quản lý khách hàng, tài xế, phương tiện, chuyến đi và xử lý sự cố. |
| **BP07** | Báo cáo | Cung cấp dữ liệu về chuyến, doanh thu, hủy chuyến và hiệu quả tài xế. |

**Bước 7: Xác định Functional requiredment (FR)**

| **Mã** | **Functional Requirement** | **Mô tả** |
|:---|---|---|
| **FR01** | Quản lý tài khoản khách hàng | Cho phép khách hàng đăng ký, đăng nhập và cập nhật thông tin cá nhân. |
| **FR02** | Tạo yêu cầu đặt xe | Cho phép khách hàng nhập điểm đón, điểm đến, chọn loại xe và gửi yêu cầu đặt xe. |
| **FR03** | Theo dõi chuyến đi | Cho phép khách hàng theo dõi trạng thái chuyến, tài xế nhận chuyến và thời gian dự kiến tài xế đến. |
| **FR04** | Tìm kiếm tài xế | Hệ thống xác định tài xế phù hợp dựa trên vị trí, trạng thái sẵn sàng và các tiêu chí vận hành. |
| **FR05** | Phân công tài xế | Gửi yêu cầu chuyến đến tài xế phù hợp và tiếp tục tìm tài xế khác nếu tài xế không phản hồi hoặc từ chối. |
| **FR06** | Quản lý trạng thái tài xế | Cho phép tài xế cập nhật trạng thái hoạt động và chuyển sang trạng thái sẵn sàng nhận chuyến. |
| **FR07** | Nhận và xử lý chuyến | Cho phép tài xế nhận hoặc từ chối chuyến được hệ thống đề xuất. |
| **FR08** | Cập nhật trạng thái chuyến | Cho phép tài xế cập nhật: đã đến điểm đón → đã đón khách → đang di chuyển → hoàn thành chuyến. |
| **FR09** | Quản lý vị trí tài xế | Lưu thông tin vị trí tài xế để hỗ trợ tìm tài xế gần khách hàng và dự kiến thời gian đến. |
| **FR10** | Tính cước | Xác định số tiền khách hàng phải trả sau khi chuyến đi hoàn thành. |
| **FR11** | Thanh toán | Hỗ trợ thanh toán bằng tiền mặt hoặc phương thức điện tử và xử lý kết quả giao dịch. |
| **FR12** | Xử lý thanh toán thất bại | Thông báo cho khách hàng khi thanh toán điện tử thất bại và cho phép xử lý lại theo chính sách doanh nghiệp. |
| **FR13** | Gửi thông báo | Gửi thông báo về tiếp nhận đặt xe, tài xế nhận chuyến, tài xế đến, hoàn thành chuyến và kết quả thanh toán. |
| **FR14** | Quản lý dữ liệu vận hành | Nhân viên có thể quản lý khách hàng, tài xế, phương tiện và chuyến đi. |
| **FR15** | Giám sát & xử lý sự cố | Nhân viên vận hành xem chuyến đang diễn ra, trạng thái tài xế, xử lý chuyến lỗi và tra cứu lịch sử giao dịch. |
| **FR16** | Phân quyền quản trị | Kiểm soát các thao tác quản trị để nhân viên thông thường không thực hiện được thao tác nhạy cảm. |
| **FR17** | Báo cáo | Cung cấp báo cáo về số lượng chuyến, doanh thu, tỷ lệ hoàn thành, tỷ lệ hủy và hiệu quả tài xế. |
| **FR18** | Lịch sử chuyến đi | Cho phép khách hàng xem lịch sử chuyến và số tiền phải trả. |
| **FR19** | Đánh giá tài xế | Cho phép khách hàng đánh giá tài xế sau khi chuyến hoàn thành. |

**Bước 8: Xác định Bussiness Rules**
| Mã | Bussiness Rule | Quy tắc |
|:---|---|---|
| **BRL01** | Xác thực người dùng | Khách hàng và tài xế phải được xác thực trước khi sử dụng các chức năng yêu cầu tài khoản. |
| **BRL02** | Tài xế sẵn sàng | Tài xế phải ở trạng thái sẵn sàng nhận chuyến khi hệ thống xem xét phân công. |
| **BRL03** | Ưu tiên tài xế | Hệ thống ưu tiên tài xế phù hợp và gần khách hàng. |
| **BRL04** | Tài xế không phản hồi/từ chối | Nếu tài xế được đề xuất không phản hồi hoặc từ chối, hệ thống phải tiếp tục tìm tài xế khác. |
| **BRL05** | Không tìm được tài xế | Nếu không tìm được tài xế phù hợp, hệ thống phải thông báo rõ ràng cho khách hàng. |
| **BRL06** | Cập nhật trạng thái chuyến | Tài xế cập nhật chuyến theo các trạng thái: đã đến điểm đón → đã đón khách → đang di chuyển → hoàn thành. |
| **BRL07** | Tính tiền | Sau khi chuyến hoàn thành, hệ thống phải xác định số tiền khách hàng phải trả. |
| **BRL08** | Thanh toán điện tử | Thanh toán điện tử phải được thực hiện thông qua nhà cung cấp thanh toán bên ngoài và hệ thống CAB không lưu thông tin nhạy cảm của thẻ/tài khoản. |
| **BRL09** | Thanh toán thất bại | Nếu thanh toán điện tử thất bại, hệ thống phải thông báo cho khách hàng và cho phép xử lý lại theo chính sách doanh nghiệp. |
| **BRL10** | Phân quyền | Các thao tác quản trị phải được kiểm soát quyền truy cập; nhân viên thông thường không được thực hiện các thao tác nhạy cảm. |
| **BRL11** | Bảo vệ dữ liệu | Thông tin cá nhân, phương tiện, vị trí và giao dịch phải được bảo vệ. |
| **BRL12** | Lưu vết | Các thao tác quan trọng phải được lưu vết để phục vụ kiểm tra khi xảy ra sự cố. |

**Bước 9: Mô hình hóa dữ liệu (Xác định thực thể ERD)**

**Bước 10: Xác định các Non-functional Requiredment**

| Mã | Non-functional Requiredment | Yêu cầu |
|:---|---|---|
| **NFR01** | Hiệu năng & khả năng chịu tải | Hệ thống phải hoạt động ổn định khi nhu cầu sử dụng tăng cao. |
| **NFR02** | Khả năng mở rộng | Các thành phần có thể mở rộng độc lập khi tải tăng. |
| **NFR03** | Tính sẵn sàng | Lỗi ở một chức năng như thanh toán hoặc thông báo không được làm toàn bộ hệ thống đặt xe ngừng hoạt động. |
| **NFR04** | Khả năng bảo trì | Cho phép triển khai chức năng mới từng phần và hạn chế ảnh hưởng đến các chức năng đang hoạt động. |
| **NFR05** | Bảo mật | Phải xác thực khách hàng và tài xế trước khi sử dụng các chức năng yêu cầu tài khoản. |
| **NFR06** | Phân quyền | Các thao tác quản trị phải được kiểm soát quyền truy cập. |
| **NFR07** | Bảo vệ dữ liệu | Bảo vệ thông tin cá nhân, phương tiện, vị trí và dữ liệu giao dịch. |
| **NFR08** | Audit / Logging | Lưu vết các thao tác quan trọng để phục vụ kiểm tra khi xảy ra sự cố. |
| **NFR09** | Khả năng mở rộng tích hợp | Có thể bổ sung các kênh thông báo, phương thức thanh toán và nhà cung cấp dịch vụ mới mà không phải thay đổi toàn bộ hệ thống. |
| **NFR10** | Khả năng phát triển lâu dài | Kiến trúc hệ thống phải đủ linh hoạt để thay đổi hoặc thay thế một số thành phần kỹ thuật trong tương lai. |

**Bước 11: Tiến hành thiết kế các Usecase**

**Bước 12: Đặc tả Usecase**

**Bước 13: Tiêu chí chấp nhận Acceptance Criteria(AC)**

**Bước 14: Truy xuất nguồn gốc yêu cầu (Requirement Traceability)**




