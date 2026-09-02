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

**In scope**

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
**Out of scope**

- Công thức tính cước cụ thể.
- Tiêu chí ưu tiên tài xế.
- Thời gian tài xế phải phản hồi.
- Chính sách hủy chuyến.
- Cách xử lý khi mất kết nối mạng.
- Thời gian lưu trữ dữ liệu.

Bước 5: Xác định các Bussiness Requiredment:
|  |

Bước 6: Xác định Business Process:

Bước 7: Functional requiredment (FR):
- FR01: Xác định vị trí khách.
- FR02: Tìm tài xế sẵn có.

Bước 8: Xác định Bussiness Ruler:
| Mã | Bussiness Rule | Nội dung |
|:---|---|---|

Bước 9: Mô hình hóa dữ liệu (Xác định thực thể ERD): 

Bước 10: Xác định các non-requiredment:

Bước 11: Tiến hành thiết kế các Usecase:

Bước 12: Đặc tả Usecase:

Bước 13: Tiêu chí chấp nhận Acceptance Criteria (AC):

Bước 14: Truy xuất nguồn gốc yêu cầu (Requirement Traceability):




