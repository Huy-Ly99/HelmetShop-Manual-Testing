HelmetShop – Software Requirements Specification
Document Type: Software Requirements Specification (SRS)
Project: HelmetShop
Role: Manual Tester / QA Intern
Version: 1.0
Status: Draft
Date: 27/09/2026
________________________________________
1. Document Overview
1.1 Purpose
Tài liệu này mô tả các yêu cầu chức năng của hệ thống HelmetShop từ góc nhìn của Customer và Admin.
Tài liệu được sử dụng làm cơ sở để:
•	Phân tích yêu cầu.
•	Xác định phạm vi kiểm thử.
•	Xây dựng Test Scenario.
•	Xây dựng Test Case.
•	Chuẩn bị Test Data.
•	Thực hiện Functional Testing.
•	Thực hiện Retest và Regression Testing.
•	Trace Requirement với Test Case và Defect.
________________________________________
2. System Overview
HelmetShop là website bán nón bảo hiểm trực tuyến.
Hệ thống gồm hai nhóm người dùng chính:
Customer
Customer có thể:
•	Xem và tìm kiếm sản phẩm.
•	Xem sản phẩm theo danh mục.
•	Xem chi tiết sản phẩm.
•	Thêm sản phẩm vào giỏ hàng.
•	Cập nhật số lượng sản phẩm.
•	Tiến hành thanh toán.
•	Nhập thông tin đặt hàng.
•	Gửi đơn hàng.
•	Nhận thông báo đặt hàng thành công.
Admin
Admin có thể:
•	Đăng nhập hệ thống quản trị.
•	Xem Dashboard.
•	Quản lý sản phẩm.
•	Xem và quản lý đơn hàng.
•	Liên hệ khách hàng.
•	Cập nhật trạng thái đơn hàng.
•	Xác nhận hàng trả đã về kho.
•	Xóa đơn hàng đã hoàn tất quá trình xử lý.
________________________________________
3. Actors
Actor	Description
Customer	Người sử dụng website để xem sản phẩm và đặt hàng
Admin	Người quản lý sản phẩm và đơn hàng của hệ thống
________________________________________



4. Functional Requirements
4.1 Customer – Trang chủ
ID	Requirement	Priority
REQ-CUS-001	Hệ thống phải hiển thị các sản phẩm mới nhất trên trang chủ.	High
REQ-CUS-002	Hệ thống phải cho phép Customer tìm kiếm sản phẩm.	High
REQ-CUS-003	Hệ thống phải cho phép Customer điều hướng đến các mục/trang khác.	Medium
________________________________________
4.2 Customer – Danh mục sản phẩm
ID	Requirement	Priority
REQ-CUS-004	Hệ thống phải hiển thị danh mục Nón bảo hiểm.	High
REQ-CUS-005	Hệ thống phải hiển thị danh mục Nón 3/4.	High
REQ-CUS-006	Hệ thống phải hiển thị danh mục Nón Fullface.	High
REQ-CUS-007	Hệ thống phải hiển thị danh mục Nón nửa đầu.	High
REQ-CUS-008	Hệ thống phải hiển thị các sản phẩm thuộc danh mục được Customer lựa chọn.	High
REQ-CUS-009	Hệ thống phải cho phép Customer tìm kiếm sản phẩm trong khu vực danh mục.	High
REQ-CUS-010	Hệ thống phải cho phép Customer chọn sản phẩm để chuyển đến Product Detail.	High
REQ-CUS-011	Hệ thống phải cho phép Customer điều hướng đến các mục/trang khác.	Medium
________________________________________
4.3 Customer – Product





ID	Requirement	Priority
REQ-CUS-012	Hệ thống phải hiển thị hình ảnh sản phẩm.	High
REQ-CUS-013	Hệ thống phải hiển thị tên sản phẩm.	High
REQ-CUS-014	Hệ thống phải hiển thị giá sản phẩm.	High
REQ-CUS-015	Hệ thống phải cho phép Customer chọn sản phẩm để xem Product Detail.	High
________________________________________
4.4 Customer – Product Detail
ID	Requirement	Priority
REQ-CUS-016	Hệ thống phải hiển thị thông tin chi tiết của sản phẩm.	High
REQ-CUS-017	Hệ thống phải cho phép Customer tăng số lượng sản phẩm.	High
REQ-CUS-018	Hệ thống phải cho phép Customer giảm số lượng sản phẩm.	High
REQ-CUS-019	Hệ thống phải cho phép Customer thêm sản phẩm vào giỏ hàng.	Critical
REQ-CUS-020	Hệ thống phải cho phép Customer điều hướng đến các mục/trang khác.	Medium
REQ-CUS-021	Hệ thống không cho phép khách hàng thêm sản phẩm vào giỏ hàng khi sản phẩm đã hết hàng.	High
________________________________________
4.5 Customer – Cart
ID	Requirement	Priority
REQ-CUS-022	Hệ thống phải hiển thị các sản phẩm trong giỏ hàng.	Critical
REQ-CUS-023	Hệ thống phải hiển thị số lượng của từng sản phẩm.	High
REQ-CUS-024	Hệ thống phải cho phép Customer tăng số lượng sản phẩm.	High
REQ-CUS-025	Hệ thống phải cho phép Customer giảm số lượng sản phẩm.	High
REQ-CUS-026	Hệ thống phải tính và hiển thị tổng tiền của giỏ hàng.	Critical
REQ-CUS-027	Hệ thống phải cho phép Customer tiếp tục mua sắm.	Medium
REQ-CUS-028	Hệ thống phải cho phép Customer tiến hành thanh toán.	Critical
REQ-CUS-029	Hệ thống không cho phép khách hàng đặt hàng khi sản phẩm trong giỏ hàng không còn đủ tồn kho.	High
REQ-CUS-030	Hệ thống thông báo cho khách hàng khi sản phẩm trong giỏ hàng đã hết hàng hoặc không đủ số lượng tồn kho.	High
________________________________________
4.6 Customer – Checkout
ID	Requirement	Priority
REQ-CUS-031	Hệ thống phải hiển thị checkoutModal sau khi Customer chọn "Tiến hành thanh toán".	High
REQ-CUS-032	Hệ thống phải cho phép Customer nhập họ tên.	High
REQ-CUS-033	Hệ thống phải cho phép Customer nhập số điện thoại.	Critical
REQ-CUS-034	Hệ thống phải cho phép Customer nhập địa chỉ.	Critical
REQ-CUS-035	Hệ thống phải cho phép Customer xác nhận đặt hàng.	Critical
REQ-CUS-036	Hệ thống phải gửi thông tin đặt hàng đến backend khi Customer xác nhận đặt hàng.	Critical
________________________________________
4.7 Customer – Order Success
ID	Requirement	Priority
REQ-CUS-037	Hệ thống phải hiển thị successModal sau khi đơn hàng được tạo thành công.	Critical
REQ-CUS-038	successModal phải hiển thị thông báo đặt hàng thành công.	High
REQ-CUS-039	Hệ thống phải cho phép Customer đóng successModal.	Medium
________________________________________
5. Admin Functional Requirements
5.1 Admin – Login
ID	Requirement	Priority
REQ-ADM-001	Hệ thống phải cho phép Admin nhập tài khoản đăng nhập.	Critical
REQ-ADM-002	Hệ thống phải cho phép Admin nhập mật khẩu.	Critical
REQ-ADM-003	Hệ thống phải cho phép Admin hiện/ẩn mật khẩu.	Medium
REQ-ADM-004	Hệ thống phải hỗ trợ chức năng ghi nhớ đăng nhập nếu chức năng được bật.	Medium
REQ-ADM-005	Hệ thống phải xác thực thông tin đăng nhập của Admin.	Critical
REQ-ADM-006	Hệ thống phải cho phép Admin quay lại trang chủ.	Low
________________________________________
5.2 Admin – Dashboard
ID	Requirement	Priority
REQ-ADM-007	Dashboard phải hiển thị tổng số sản phẩm.	High
REQ-ADM-008	Dashboard phải hiển thị tổng số đơn hàng.	High
REQ-ADM-009	Dashboard phải hiển thị tổng số khách hàng.	High
REQ-ADM-010	Dashboard phải hiển thị tổng doanh thu.	High
REQ-ADM-011	Admin phải có chức năng thêm sản phẩm.	Critical
REQ-ADM-012	Dashboard phải hiển thị thông tin/danh sách sản phẩm hiện có.	High
________________________________________
5.3 Admin – Product Management
Các requirement dưới đây cần được đối chiếu với chức năng thực tế của phiên bản HelmetShop đang được kiểm thử.
ID	Requirement	Priority
REQ-ADM-013	Admin phải có thể xem thông tin sản phẩm.	High
REQ-ADM-014	Admin phải có thể chỉnh sửa thông tin sản phẩm nếu chức năng được hỗ trợ.	Critical
REQ-ADM-015	Admin phải có thể thay đổi hình ảnh sản phẩm nếu chức năng được hỗ trợ.	High
REQ-ADM-016	Admin phải có thể thay đổi giá sản phẩm nếu chức năng được hỗ trợ.	Critical
REQ-ADM-017	Admin phải có thể thay đổi số lượng tồn kho nếu chức năng được hỗ trợ.	Critical
REQ-ADM-018	Admin phải có thể xóa sản phẩm nếu chức năng được hỗ trợ.	High
________________________________________
6. Admin – Order Management
ID	Requirement	Priority
REQ-ADM-019	Hệ thống phải hiển thị tổng số đơn hàng.	High
REQ-ADM-020	Hệ thống phải hiển thị số đơn hàng chưa liên hệ.	High
REQ-ADM-021	Hệ thống phải hiển thị số đơn hàng đã liên hệ.	High
REQ-ADM-022	Hệ thống phải hiển thị doanh thu.	High
REQ-ADM-023	Hệ thống phải hiển thị danh sách đơn hàng.	Critical
REQ-ADM-024	Danh sách đơn hàng phải hiển thị Order ID.	High
REQ-ADM-025	Danh sách đơn hàng phải hiển thị tên khách hàng.	High
REQ-ADM-026	Danh sách đơn hàng phải hiển thị số điện thoại khách hàng.	Critical
REQ-ADM-027	Danh sách đơn hàng phải hiển thị sản phẩm trong đơn hàng.	Critical
REQ-ADM-028	Danh sách đơn hàng phải hiển thị giá trị đơn hàng.	Critical
REQ-ADM-029	Danh sách đơn hàng phải hiển thị trạng thái đơn hàng.	Critical
REQ-ADM-030	Admin phải có thể xem chi tiết đơn hàng.	High
________________________________________
7. Admin – Order Detail

ID	Requirement	Priority
REQ-ADM-031	Chi tiết đơn hàng phải hiển thị Order ID.	High
REQ-ADM-032	Chi tiết đơn hàng phải hiển thị tên sản phẩm.	High
REQ-ADM-033	Chi tiết đơn hàng phải hiển thị số lượng sản phẩm.	High
REQ-ADM-034	Chi tiết đơn hàng phải hiển thị giá sản phẩm.	High
________________________________________
8. Admin – Order Status
Hệ thống phải hỗ trợ quản lý trạng thái đơn hàng theo quy trình nghiệp vụ của HelmetShop.
ID	Requirement	Priority
REQ-ADM-035	Hệ thống cho phép Admin chuyển trạng thái đơn hàng từ "Chưa liên hệ" sang "Đã liên hệ".	High
REQ-ADM-036	Hệ thống hiển thị trạng thái "Đã liên hệ" và cung cấp chức năng "Huỷ hàng" và "Đã nhận tiền" khi đơn hàng ở trạng thái "Đã liên hệ".	High
REQ-ADM-037	Hệ thống cho phép Admin chuyển trạng thái đơn hàng từ "Đã liên hệ" sang "Huỷ hàng".	High
REQ-ADM-038	Hệ thống hiển thị trạng thái "Huỷ hàng" và cung cấp chức năng xoá đơn hàng khi đơn hàng ở trạng thái "Huỷ hàng".	Medium
REQ-ADM-039	Hệ thống cho phép Admin chuyển trạng thái đơn hàng từ "Đã liên hệ" sang "Đã nhận tiền".	High
REQ-ADM-040	Hệ thống hiển thị trạng thái "Đã nhận tiền" và cung cấp chức năng "Trả hàng" khi đơn hàng ở trạng thái "Đã nhận tiền".	High
REQ-ADM-041	Hệ thống cho phép Admin chuyển trạng thái đơn hàng từ "Đã nhận tiền" sang "Trả hàng".	High
REQ-ADM-042	Hệ thống hiển thị trạng thái "Trả hàng" và cung cấp chức năng "Đã về kho" khi đơn hàng ở trạng thái "Trả hàng".	High
REQ-ADM-043	Hệ thống cho phép Admin chuyển trạng thái đơn hàng từ "Trả hàng" sang "Đã về kho".	High
REQ-ADM-044	Hệ thống hiển thị trạng thái "Đã về kho" và cung cấp chức năng "Đã hoàn tiền" khi đơn hàng ở trạng thái "Đã về kho".	High
REQ-ADM-046	Hệ thống hiển thị trạng thái "Đã hoàn tiền" và cung cấp chức năng xoá đơn hàng khi đơn hàng ở trạng thái "Đã hoàn tiền".	Medium
REQ-ADM-047	Hệ thống cho phép Admin xoá đơn hàng.	Medium


________________________________________
9. Order Status Flow
Quy trình trạng thái đơn hàng được sử dụng làm cơ sở để kiểm thử State Transition.
Chưa liên hệ
      │
      ▼
Đã liên hệ
      │
      ▼
Đã nhận tiền
      │
      ├──────────────► Huỷ hàng
      │                    │
      │                    ▼
      │               Đã về kho
      │                    │
      │                    ▼
      │              Hiển thị nút Xóa
      │
      ▼
  Xử lý/Giao hàng
      │
      ▼
  Trả hàng
      │
      ▼
  Huỷ hang ───► Đã về kho ───► Hiển thị nút xoá

Flow trên cần được đối chiếu với implementation thực tế trước khi sử dụng làm Test Case chính thức. Tester không nên giả định trạng thái nếu hệ thống chưa định nghĩa trạng thái đó.
________________________________________
10. Business Rules
BR-001 – Customer không cần tạo tài khoản
Customer có thể thực hiện mua hàng mà không cần đăng ký tài khoản.
BR-002 – Thông tin Checkout
Customer phải cung cấp thông tin cần thiết để Admin có thể liên hệ và xác nhận đơn hàng.
Thông tin bao gồm:
•	Họ tên.
•	Số điện thoại.
•	Địa chỉ.
BR-003 – Đặt hàng
Đơn hàng chỉ được xem là thành công khi hệ thống xử lý việc tạo đơn hàng thành công.
BR-004 – Success Modal
successModal chỉ được hiển thị khi đơn hàng được tạo thành công.
BR-005 – Quản lý trạng thái đơn hàng
Admin chịu trách nhiệm cập nhật trạng thái đơn hàng trong quá trình xử lý.
BR-006 – Đơn hàng trả về
Khi đơn hàng trả đã thực sự về kho, Admin xác nhận trạng thái "Đã về kho".
BR-007 – Xóa đơn hàng
Đơn hàng chỉ hiển thị chức năng xóa sau khi được xác nhận "Đã về kho".
________________________________________
11. Non-Functional Requirements
Các yêu cầu phi chức năng sẽ được kiểm thử bổ sung trong quá trình QA.
NFR-001 – Responsive
Website phải có giao diện sử dụng được trên:
•	Desktop.
•	Tablet.
•	Mobile.
NFR-002 – Usability
Các nút chức năng và thông tin chính phải dễ nhận biết và sử dụng.
NFR-003 – Validation
Các trường nhập liệu quan trọng phải có validation phù hợp.
NFR-004 – Security
Khu vực Admin phải yêu cầu xác thực trước khi truy cập các chức năng quản trị.
NFR-005 – API
Các API phải xử lý request và response đúng theo thiết kế.
NFR-006 – Data Integrity
Thông tin sản phẩm, giỏ hàng và đơn hàng phải được lưu trữ và trả về nhất quán.
