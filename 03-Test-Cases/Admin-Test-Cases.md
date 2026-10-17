# Admin Test Cases – HelmetShop

Các test case dưới đây được trình bày theo mẫu Markdown chi tiết. `Actual Result`, `Status` và `Evidence` cần được cập nhật sau khi thực thi thực tế.

> **Lưu ý:** Status mặc định là `NOT RUN`. Không đánh dấu PASS/FAIL trước khi chạy test. Với các yêu cầu chưa rõ hoặc trùng lặp, xem ghi chú ở cuối file.

## TS-ADM-LOGIN-001 – Kiểm tra nhập tài khoản admin

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-001 |
| **Title** | Kiểm tra nhập tài khoản admin |
| **Requirement** | REQ-ADM-001 |
| **Priority** | Medium |
| **Preconditions** | Đang ở trang đăng nhập admin |
| **Test Data** | Tài khoản hợp lệ: admin@example.com |
| **Steps** | 1. Mở trang đăng nhập admin.<br>2. Nhập tài khoản hợp lệ vào ô tài khoản.<br>3. Quan sát giá trị trong ô. |
| **Expected Result** | Ô tài khoản nhận và hiển thị đúng giá trị đã nhập; không tự thay đổi hoặc cắt mất ký tự hợp lệ. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-LOGIN-002 – Kiểm tra nhập mật khẩu admin

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-002 |
| **Title** | Kiểm tra nhập mật khẩu admin |
| **Requirement** | REQ-ADM-002 |
| **Priority** | Medium |
| **Preconditions** | Đang ở trang đăng nhập admin |
| **Test Data** | Mật khẩu hợp lệ của tài khoản test |
| **Steps** | 1. Mở trang đăng nhập admin.<br>2. Nhập mật khẩu vào ô mật khẩu.<br>3. Quan sát ô nhập. |
| **Expected Result** | Ô mật khẩu nhận giá trị; mặc định ký tự mật khẩu được che; không hiển thị mật khẩu dạng văn bản rõ. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-LOGIN-003 – Kiểm tra chức năng ẩn/hiện mật khẩu

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-003 |
| **Title** | Kiểm tra chức năng ẩn/hiện mật khẩu |
| **Requirement** | REQ-ADM-003 |
| **Priority** | Low |
| **Preconditions** | Đang ở trang đăng nhập admin |
| **Test Data** | Mật khẩu: Test@12345 |
| **Steps** | 1. Nhập mật khẩu.<br>2. Nhấn biểu tượng hiện mật khẩu.<br>3. Quan sát giá trị.<br>4. Nhấn lại để ẩn. |
| **Expected Result** | Khi chọn hiện, mật khẩu được hiển thị đúng; khi chọn ẩn, mật khẩu được che lại; giá trị không bị thay đổi. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-LOGIN-004 – Kiểm tra ghi nhớ đăng nhập khi chức năng được bật

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-004 |
| **Title** | Kiểm tra ghi nhớ đăng nhập khi chức năng được bật |
| **Requirement** | REQ-ADM-004 |
| **Priority** | Medium |
| **Preconditions** | Chức năng ghi nhớ đăng nhập được cấu hình và hiển thị |
| **Test Data** | Tài khoản admin test hợp lệ |
| **Steps** | 1. Chọn Ghi nhớ đăng nhập.<br>2. Đăng nhập thành công.<br>3. Đóng và mở lại trình duyệt.<br>4. Kiểm tra trạng thái phiên đăng nhập. |
| **Expected Result** | Hành vi đúng với yêu cầu đã định nghĩa: duy trì phiên hoặc ghi nhớ thông tin được phép; không lưu mật khẩu dạng rõ. Nếu không có checkbox/chưa có yêu cầu cụ thể, đánh dấu Blocked và xác nhận requirement. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |
| **Notes** | Cần xác nhận chính xác ý nghĩa 'Ghi nhớ đăng nhập' và điều kiện chức năng được bật. |

## TS-ADM-LOGIN-005 – Kiểm tra xác thực thông tin đăng nhập admin

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-005 |
| **Title** | Kiểm tra xác thực thông tin đăng nhập admin |
| **Requirement** | REQ-ADM-005 |
| **Priority** | High |
| **Preconditions** | Đang ở trang đăng nhập admin |
| **Test Data** | 1) Tài khoản/mật khẩu hợp lệ; 2) sai mật khẩu; 3) tài khoản không tồn tại |
| **Steps** | 1. Nhập thông tin hợp lệ và nhấn Đăng nhập.<br>2. Đăng xuất.<br>3. Nhập sai mật khẩu và gửi.<br>4. Thử tài khoản không tồn tại. |
| **Expected Result** | Thông tin hợp lệ: đăng nhập thành công và chuyển đến trang admin. Thông tin sai: không đăng nhập; hiển thị thông báo phù hợp, không tiết lộ thông tin nhạy cảm. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-LOGIN-006 – Kiểm tra quay về trang chủ từ trang đăng nhập

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-LOGIN-006 |
| **Title** | Kiểm tra quay về trang chủ từ trang đăng nhập |
| **Requirement** | REQ-ADM-006 |
| **Priority** | Low |
| **Preconditions** | Đang ở trang đăng nhập admin |
| **Test Data** | Không áp dụng |
| **Steps** | 1. Mở trang đăng nhập admin.<br>2. Nhấn liên kết/nút quay về trang chủ. |
| **Expected Result** | Điều hướng về trang chủ website; trang chủ tải thành công. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-DASH-001 – Kiểm tra tổng số sản phẩm hiện có

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-001 |
| **Title** | Kiểm tra tổng số sản phẩm hiện có |
| **Requirement** | REQ-ADM-007 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; biết số sản phẩm trong dữ liệu test |
| **Test Data** | Có N sản phẩm đang được tính theo quy tắc hệ thống |
| **Steps** | 1. Mở Dashboard.<br>2. Ghi nhận số sản phẩm thực tế trong dữ liệu.<br>3. So sánh với số hiển thị. |
| **Expected Result** | Tổng số sản phẩm hiển thị đúng theo quy tắc đếm đã định nghĩa; không bị sai lệch hoặc hiển thị NaN/undefined. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-DASH-002 – Kiểm tra tổng số đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-002 |
| **Title** | Kiểm tra tổng số đơn hàng |
| **Requirement** | REQ-ADM-008 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; biết tổng đơn trong dữ liệu test |
| **Test Data** | Có N đơn hàng |
| **Steps** | 1. Mở Dashboard.<br>2. Đối chiếu số đơn trong dữ liệu với số trên Dashboard. |
| **Expected Result** | Tổng số đơn hàng hiển thị chính xác theo quy tắc tính của hệ thống. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-DASH-003 – Kiểm tra tổng số khách hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-003 |
| **Title** | Kiểm tra tổng số khách hàng |
| **Requirement** | REQ-ADM-009 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có dữ liệu khách hàng để đối chiếu |
| **Test Data** | Có N khách hàng theo định nghĩa hệ thống |
| **Steps** | 1. Mở Dashboard.<br>2. Đối chiếu số khách hàng hiển thị với dữ liệu nguồn. |
| **Expected Result** | Tổng số khách hàng khớp dữ liệu và quy tắc đếm đã định nghĩa. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-DASH-004 – Kiểm tra tổng doanh thu

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-004 |
| **Title** | Kiểm tra tổng doanh thu |
| **Requirement** | REQ-ADM-010 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có đơn hàng ở các trạng thái khác nhau |
| **Test Data** | Các đơn có giá trị và trạng thái đã biết |
| **Steps** | 1. Mở Dashboard.<br>2. Tính doanh thu theo quy tắc nghiệp vụ được xác nhận.<br>3. So sánh với số hiển thị. |
| **Expected Result** | Doanh thu khớp quy tắc tính doanh thu đã thống nhất; định dạng tiền tệ dễ đọc. Nếu chưa xác định trạng thái nào được tính doanh thu, cần làm rõ requirement. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |
| **Notes** | Cần xác nhận quy tắc tính doanh thu và các trạng thái được tính. |

## TS-ADM-DASH-005 – Kiểm tra chức năng thêm sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-005 |
| **Title** | Kiểm tra chức năng thêm sản phẩm |
| **Requirement** | REQ-ADM-011 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có quyền quản lý sản phẩm |
| **Test Data** | Tên, giá, số lượng hợp lệ; ảnh hợp lệ nếu bắt buộc |
| **Steps** | 1. Mở khu vực quản lý sản phẩm.<br>2. Nhấn Thêm sản phẩm.<br>3. Nhập dữ liệu hợp lệ.<br>4. Lưu.<br>5. Tìm sản phẩm vừa tạo. |
| **Expected Result** | Sản phẩm được tạo thành công; thông báo rõ ràng; dữ liệu lưu đúng và sản phẩm xuất hiện trong danh sách. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-DASH-006 – Kiểm tra hiển thị danh sách sản phẩm hiện có

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-DASH-006 |
| **Title** | Kiểm tra hiển thị danh sách sản phẩm hiện có |
| **Requirement** | REQ-ADM-012 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có sản phẩm trong hệ thống |
| **Test Data** | Danh sách gồm nhiều sản phẩm với dữ liệu đã biết |
| **Steps** | 1. Mở khu vực quản lý sản phẩm.<br>2. Quan sát danh sách và các thông tin chính.<br>3. Đối chiếu một vài bản ghi với dữ liệu nguồn. |
| **Expected Result** | Danh sách hiển thị các sản phẩm theo thiết kế; thông tin không bị thiếu/sai; trạng thái rỗng được xử lý khi không có sản phẩm. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-001 – Kiểm tra xem thông tin sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-001 |
| **Title** | Kiểm tra xem thông tin sản phẩm |
| **Requirement** | REQ-ADM-013 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; sản phẩm tồn tại |
| **Test Data** | Một sản phẩm đã có dữ liệu |
| **Steps** | 1. Mở danh sách sản phẩm.<br>2. Chọn xem chi tiết một sản phẩm. |
| **Expected Result** | Trang/khung chi tiết hiển thị đúng thông tin sản phẩm đã chọn. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-002 – Kiểm tra chỉnh sửa thông tin sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-002 |
| **Title** | Kiểm tra chỉnh sửa thông tin sản phẩm |
| **Requirement** | REQ-ADM-014 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; sản phẩm tồn tại |
| **Test Data** | Cập nhật tên/mô tả bằng giá trị hợp lệ |
| **Steps** | 1. Mở chức năng chỉnh sửa sản phẩm.<br>2. Thay đổi một hoặc nhiều trường hợp lệ.<br>3. Lưu.<br>4. Mở lại sản phẩm. |
| **Expected Result** | Thông tin được cập nhật và lưu chính xác; danh sách/chi tiết phản ánh dữ liệu mới. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-003 – Kiểm tra thay đổi hình ảnh sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-003 |
| **Title** | Kiểm tra thay đổi hình ảnh sản phẩm |
| **Requirement** | REQ-ADM-015 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; sản phẩm tồn tại |
| **Test Data** | Ảnh hợp lệ theo định dạng/kích thước cho phép |
| **Steps** | 1. Mở chỉnh sửa sản phẩm.<br>2. Chọn ảnh hợp lệ.<br>3. Lưu.<br>4. Tải lại trang và kiểm tra ảnh. |
| **Expected Result** | Ảnh mới được tải lên và hiển thị đúng sau khi tải lại; ảnh cũ được thay thế theo yêu cầu. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-004 – Kiểm tra thay đổi giá sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-004 |
| **Title** | Kiểm tra thay đổi giá sản phẩm |
| **Requirement** | REQ-ADM-016 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; sản phẩm tồn tại |
| **Test Data** | Giá hợp lệ: 250000 |
| **Steps** | 1. Mở chỉnh sửa sản phẩm.<br>2. Nhập giá mới hợp lệ.<br>3. Lưu.<br>4. Kiểm tra chi tiết sản phẩm ở admin và giao diện khách hàng nếu có. |
| **Expected Result** | Giá mới được lưu và hiển thị chính xác ở các vị trí liên quan; định dạng tiền tệ đúng. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-005 – Kiểm tra thay đổi số lượng tồn kho

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-005 |
| **Title** | Kiểm tra thay đổi số lượng tồn kho |
| **Requirement** | REQ-ADM-017 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; sản phẩm tồn tại |
| **Test Data** | Số lượng mới: 20 |
| **Steps** | 1. Mở chỉnh sửa sản phẩm.<br>2. Nhập số lượng tồn kho hợp lệ.<br>3. Lưu.<br>4. Tải lại và kiểm tra. |
| **Expected Result** | Số lượng tồn kho được lưu chính xác; không chấp nhận giá trị ngoài quy tắc như số âm hoặc số thập phân nếu chỉ cho phép số nguyên. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-PM-006 – Kiểm tra xoá sản phẩm

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-PM-006 |
| **Title** | Kiểm tra xoá sản phẩm |
| **Requirement** | REQ-ADM-018 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; sản phẩm có thể xoá |
| **Test Data** | Một sản phẩm test không dùng cho test khác |
| **Steps** | 1. Mở danh sách sản phẩm.<br>2. Chọn xoá sản phẩm test.<br>3. Xác nhận nếu có hộp thoại.<br>4. Tìm lại sản phẩm. |
| **Expected Result** | Sản phẩm bị xoá/ẩn theo thiết kế; thông báo kết quả rõ ràng; sản phẩm không còn trong danh sách. Không xoá dữ liệu dùng chung. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-001 – Kiểm tra tổng số đơn hàng trong trang Order

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-001 |
| **Title** | Kiểm tra tổng số đơn hàng trong trang Order |
| **Requirement** | REQ-ADM-019 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có dữ liệu đơn hàng |
| **Test Data** | Có N đơn hàng |
| **Steps** | 1. Mở trang Order.<br>2. Đối chiếu số tổng hiển thị với dữ liệu nguồn. |
| **Expected Result** | Tổng số đơn hàng hiển thị chính xác theo quy tắc đếm. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-002 – Kiểm tra số đơn hàng chưa liên hệ

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-002 |
| **Title** | Kiểm tra số đơn hàng chưa liên hệ |
| **Requirement** | REQ-ADM-020 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có đơn ở trạng thái Chưa liên hệ |
| **Test Data** | Có N đơn Chưa liên hệ |
| **Steps** | 1. Mở trang Order.<br>2. Ghi nhận bộ đếm Chưa liên hệ.<br>3. Đối chiếu với danh sách/dữ liệu. |
| **Expected Result** | Bộ đếm bằng số đơn thuộc trạng thái Chưa liên hệ. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-003 – Kiểm tra số đơn hàng đã liên hệ

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-003 |
| **Title** | Kiểm tra số đơn hàng đã liên hệ |
| **Requirement** | REQ-ADM-021 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có đơn ở trạng thái Đã liên hệ |
| **Test Data** | Có N đơn Đã liên hệ |
| **Steps** | 1. Mở trang Order.<br>2. Ghi nhận bộ đếm Đã liên hệ.<br>3. Đối chiếu với danh sách/dữ liệu. |
| **Expected Result** | Bộ đếm bằng số đơn thuộc trạng thái Đã liên hệ. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-004 – Kiểm tra doanh thu trong trang Order

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-004 |
| **Title** | Kiểm tra doanh thu trong trang Order |
| **Requirement** | REQ-ADM-022 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có đơn hàng với trạng thái/giá trị đã biết |
| **Test Data** | Các đơn có tổng tiền đã biết |
| **Steps** | 1. Mở trang Order.<br>2. Tính doanh thu theo quy tắc nghiệp vụ đã thống nhất.<br>3. So sánh với giá trị hiển thị. |
| **Expected Result** | Doanh thu khớp quy tắc tính được phê duyệt; nếu chưa xác định đơn huỷ/hoàn tiền có được tính hay không thì cần làm rõ. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |
| **Notes** | Cần xác nhận quy tắc tính doanh thu, đặc biệt đơn huỷ/hoàn tiền. |

## TS-ADM-OM-005 – Kiểm tra danh sách đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-005 |
| **Title** | Kiểm tra danh sách đơn hàng |
| **Requirement** | REQ-ADM-023 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có đơn hàng |
| **Test Data** | Nhiều đơn hàng ở các trạng thái khác nhau |
| **Steps** | 1. Mở trang Order.<br>2. Quan sát danh sách.<br>3. Đối chiếu các đơn mẫu với dữ liệu nguồn. |
| **Expected Result** | Danh sách hiển thị đúng các đơn hàng và thông tin được thiết kế; xử lý đúng trường hợp danh sách rỗng hoặc nhiều bản ghi. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-006 – Kiểm tra hiển thị Order ID

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-006 |
| **Title** | Kiểm tra hiển thị Order ID |
| **Requirement** | REQ-ADM-024 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; có đơn hàng |
| **Test Data** | Một đơn hàng có ID xác định |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Tìm đơn test.<br>3. Kiểm tra Order ID. |
| **Expected Result** | Order ID hiển thị đúng và gắn với đúng đơn hàng; không trùng hoặc bị cắt mất phần quan trọng. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-007 – Kiểm tra hiển thị tên khách hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-007 |
| **Title** | Kiểm tra hiển thị tên khách hàng |
| **Requirement** | REQ-ADM-025 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn hàng có tên khách hàng |
| **Test Data** | Tên khách hàng test: Nguyen Van A |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Tìm đơn test.<br>3. Kiểm tra tên khách hàng. |
| **Expected Result** | Tên khách hàng khớp dữ liệu đơn hàng. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-008 – Kiểm tra hiển thị số điện thoại khách hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-008 |
| **Title** | Kiểm tra hiển thị số điện thoại khách hàng |
| **Requirement** | REQ-ADM-026 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn hàng có số điện thoại |
| **Test Data** | Số điện thoại test đã lưu trong đơn |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Tìm đơn test.<br>3. Kiểm tra số điện thoại. |
| **Expected Result** | Số điện thoại hiển thị đúng theo dữ liệu đã lưu và định dạng; không bị mất chữ số đầu. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-009 – Kiểm tra hiển thị sản phẩm trong đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-009 |
| **Title** | Kiểm tra hiển thị sản phẩm trong đơn hàng |
| **Requirement** | REQ-ADM-027 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn có ít nhất một sản phẩm |
| **Test Data** | Đơn test có sản phẩm và số lượng đã biết |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Kiểm tra thông tin tóm tắt sản phẩm hoặc mở chi tiết. |
| **Expected Result** | Sản phẩm gắn với đơn hiển thị đúng; tên/số lượng không bị nhầm sang đơn khác. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-010 – Kiểm tra hiển thị giá trị đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-010 |
| **Title** | Kiểm tra hiển thị giá trị đơn hàng |
| **Requirement** | REQ-ADM-028 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn hàng có tổng tiền |
| **Test Data** | Đơn test có tổng tiền đã biết |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Tìm đơn test.<br>3. So sánh giá trị hiển thị với tổng tiền của đơn. |
| **Expected Result** | Giá trị đơn hàng khớp dữ liệu và được định dạng tiền tệ đúng. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-011 – Kiểm tra hiển thị trạng thái đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-011 |
| **Title** | Kiểm tra hiển thị trạng thái đơn hàng |
| **Requirement** | REQ-ADM-029 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có đơn ở nhiều trạng thái |
| **Test Data** | Chưa liên hệ, Đã liên hệ, Huỷ hàng, Đã nhận tiền, Trả hàng, Đã về kho, Đã hoàn tiền (nếu có) |
| **Steps** | 1. Mở danh sách đơn hàng.<br>2. Kiểm tra trạng thái của từng đơn mẫu. |
| **Expected Result** | Mỗi đơn hiển thị đúng trạng thái hiện tại; nhãn trạng thái nhất quán với trang chi tiết. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OM-012 – Kiểm tra mở chi tiết đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OM-012 |
| **Title** | Kiểm tra mở chi tiết đơn hàng |
| **Requirement** | REQ-ADM-030 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; có đơn hàng |
| **Test Data** | Một Order ID hợp lệ |
| **Steps** | 1. Mở trang Order.<br>2. Chọn một đơn hàng để xem chi tiết. |
| **Expected Result** | Mở đúng trang/khung chi tiết của đơn đã chọn; dữ liệu Order ID và thông tin liên quan chính xác. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OD-001 – Kiểm tra hiển thị Order ID trong chi tiết

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OD-001 |
| **Title** | Kiểm tra hiển thị Order ID trong chi tiết |
| **Requirement** | REQ-ADM-031 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn hàng tồn tại |
| **Test Data** | Order ID của đơn test |
| **Steps** | 1. Mở chi tiết đơn test.<br>2. Kiểm tra Order ID. |
| **Expected Result** | Order ID hiển thị đúng và khớp đơn được mở. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OD-002 – Kiểm tra hiển thị tên sản phẩm trong chi tiết

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OD-002 |
| **Title** | Kiểm tra hiển thị tên sản phẩm trong chi tiết |
| **Requirement** | REQ-ADM-032 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn có sản phẩm |
| **Test Data** | Đơn test có tên sản phẩm xác định |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra tên sản phẩm. |
| **Expected Result** | Tên sản phẩm hiển thị đúng với sản phẩm đã đặt. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OD-003 – Kiểm tra hiển thị số lượng sản phẩm trong chi tiết

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OD-003 |
| **Title** | Kiểm tra hiển thị số lượng sản phẩm trong chi tiết |
| **Requirement** | REQ-ADM-033 |
| **Priority** | Medium |
| **Preconditions** | Đã đăng nhập admin; đơn có sản phẩm |
| **Test Data** | Số lượng đã đặt: 2 |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra số lượng của từng sản phẩm. |
| **Expected Result** | Số lượng hiển thị đúng với số lượng đã đặt. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OD-004 – Kiểm tra hiển thị giá sản phẩm trong chi tiết

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OD-004 |
| **Title** | Kiểm tra hiển thị giá sản phẩm trong chi tiết |
| **Requirement** | REQ-ADM-034 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn có sản phẩm |
| **Test Data** | Giá tại thời điểm đặt hàng đã biết |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra đơn giá và thành tiền nếu có. |
| **Expected Result** | Giá hiển thị đúng theo dữ liệu đơn hàng; nếu hệ thống lưu giá tại thời điểm đặt, không tự đổi theo giá sản phẩm hiện tại. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-001 – Chuyển trạng thái từ Chưa liên hệ sang Đã liên hệ

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-001 |
| **Title** | Chuyển trạng thái từ Chưa liên hệ sang Đã liên hệ |
| **Requirement** | REQ-ADM-035 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn ở trạng thái Chưa liên hệ |
| **Test Data** | Một đơn test trạng thái Chưa liên hệ |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn hành động Đã liên hệ.<br>3. Xác nhận nếu được yêu cầu.<br>4. Tải lại trang. |
| **Expected Result** | Trạng thái đổi thành Đã liên hệ và vẫn giữ sau khi tải lại; hành động tiếp theo phù hợp trạng thái mới. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-002 – Kiểm tra trạng thái và hành động sau khi Đã liên hệ

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-002 |
| **Title** | Kiểm tra trạng thái và hành động sau khi Đã liên hệ |
| **Requirement** | REQ-ADM-036 |
| **Priority** | High |
| **Preconditions** | Đơn vừa được chuyển sang Đã liên hệ |
| **Test Data** | Một đơn trạng thái Đã liên hệ |
| **Steps** | 1. Mở/tải lại chi tiết đơn.<br>2. Kiểm tra nhãn trạng thái.<br>3. Kiểm tra các hành động Huỷ hàng và Đã nhận tiền. |
| **Expected Result** | Hiển thị trạng thái Đã liên hệ; các hành động Huỷ hàng và Đã nhận tiền xuất hiện/khả dụng đúng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-003 – Chuyển trạng thái từ Đã liên hệ sang Huỷ hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-003 |
| **Title** | Chuyển trạng thái từ Đã liên hệ sang Huỷ hàng |
| **Requirement** | REQ-ADM-037 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn ở trạng thái Đã liên hệ |
| **Test Data** | Một đơn test trạng thái Đã liên hệ |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn Huỷ hàng.<br>3. Xác nhận nếu có.<br>4. Tải lại trang. |
| **Expected Result** | Trạng thái chuyển thành Huỷ hàng và được lưu; không chuyển nhầm sang trạng thái khác. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-004 – Kiểm tra trạng thái Huỷ hàng và hành động xoá đơn

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-004 |
| **Title** | Kiểm tra trạng thái Huỷ hàng và hành động xoá đơn |
| **Requirement** | REQ-ADM-038 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái Huỷ hàng |
| **Test Data** | Một đơn test đã huỷ |
| **Steps** | 1. Mở chi tiết đơn đã huỷ.<br>2. Kiểm tra trạng thái.<br>3. Kiểm tra hành động xoá đơn. |
| **Expected Result** | Trạng thái Huỷ hàng hiển thị đúng; hành động xoá đơn xuất hiện/khả dụng đúng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-005 – Chuyển trạng thái từ Đã liên hệ sang Đã nhận tiền

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-005 |
| **Title** | Chuyển trạng thái từ Đã liên hệ sang Đã nhận tiền |
| **Requirement** | REQ-ADM-039 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn ở trạng thái Đã liên hệ |
| **Test Data** | Một đơn test trạng thái Đã liên hệ |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn Đã nhận tiền.<br>3. Xác nhận nếu có.<br>4. Tải lại trang. |
| **Expected Result** | Trạng thái chuyển thành Đã nhận tiền và được lưu; hành động tiếp theo phù hợp trạng thái mới. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-006 – Kiểm tra trạng thái Đã nhận tiền và hành động Trả hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-006 |
| **Title** | Kiểm tra trạng thái Đã nhận tiền và hành động Trả hàng |
| **Requirement** | REQ-ADM-040 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái Đã nhận tiền |
| **Test Data** | Một đơn test đã nhận tiền |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra trạng thái.<br>3. Kiểm tra hành động Trả hàng. |
| **Expected Result** | Trạng thái Đã nhận tiền hiển thị đúng; hành động Trả hàng khả dụng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-007 – Chuyển trạng thái từ Đã nhận tiền sang Trả hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-007 |
| **Title** | Chuyển trạng thái từ Đã nhận tiền sang Trả hàng |
| **Requirement** | REQ-ADM-041 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn ở trạng thái Đã nhận tiền |
| **Test Data** | Một đơn test đã nhận tiền |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn Trả hàng.<br>3. Xác nhận nếu có.<br>4. Tải lại trang. |
| **Expected Result** | Trạng thái chuyển thành Trả hàng và được lưu; hệ thống hiển thị hành động tiếp theo đúng thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-008 – Kiểm tra trạng thái Trả hàng và hành động Đã về kho

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-008 |
| **Title** | Kiểm tra trạng thái Trả hàng và hành động Đã về kho |
| **Requirement** | REQ-ADM-042 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái Trả hàng |
| **Test Data** | Một đơn test đang Trả hàng |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra trạng thái.<br>3. Kiểm tra hành động Đã về kho. |
| **Expected Result** | Trạng thái Trả hàng hiển thị đúng; hành động Đã về kho xuất hiện/khả dụng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-009 – Chuyển trạng thái từ Trả hàng sang Đã về kho

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-009 |
| **Title** | Chuyển trạng thái từ Trả hàng sang Đã về kho |
| **Requirement** | REQ-ADM-043 |
| **Priority** | High |
| **Preconditions** | Đã đăng nhập admin; đơn ở trạng thái Trả hàng |
| **Test Data** | Một đơn test trạng thái Trả hàng |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn Đã về kho.<br>3. Xác nhận nếu có.<br>4. Tải lại trang. |
| **Expected Result** | Trạng thái chuyển thành Đã về kho và được lưu; tồn kho được xử lý đúng theo quy tắc nghiệp vụ đã xác nhận. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-010 – Kiểm tra trạng thái Đã về kho và hành động Đã hoàn tiền

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-010 |
| **Title** | Kiểm tra trạng thái Đã về kho và hành động Đã hoàn tiền |
| **Requirement** | REQ-ADM-044 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái Đã về kho |
| **Test Data** | Một đơn test đã về kho |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Kiểm tra trạng thái.<br>3. Kiểm tra hành động Đã hoàn tiền. |
| **Expected Result** | Trạng thái Đã về kho hiển thị đúng; hành động Đã hoàn tiền khả dụng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-011 – Kiểm tra chuyển trạng thái từ Trả hàng sang Đã về kho (cần xác nhận requirement)

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-011 |
| **Title** | Kiểm tra chuyển trạng thái từ Trả hàng sang Đã về kho (cần xác nhận requirement) |
| **Requirement** | REQ-ADM-045 |
| **Priority** | Medium |
| **Preconditions** | Đơn ở trạng thái Trả hàng |
| **Test Data** | Một đơn test trạng thái Trả hàng |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Thực hiện hành động Đã về kho nếu được phép.<br>3. Tải lại trang và kiểm tra trạng thái. |
| **Expected Result** | Nếu REQ-ADM-045 thực sự là luồng Trả hàng → Đã về kho, kết quả phải giống TS-ADM-OS-009. Đây là trường hợp trùng với TS-ADM-OS-009; cần xác nhận hoặc sửa requirement/test case trước khi chạy. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |
| **Notes** | Trùng nội dung TS-ADM-OS-009 nhưng Requirement ID khác; xác minh REQ-ADM-045 trước khi thực thi. |

## TS-ADM-OS-012 – Kiểm tra trạng thái Đã hoàn tiền và hành động xoá đơn

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-012 |
| **Title** | Kiểm tra trạng thái Đã hoàn tiền và hành động xoá đơn |
| **Requirement** | REQ-ADM-046 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái Đã hoàn tiền |
| **Test Data** | Một đơn test đã hoàn tiền |
| **Steps** | 1. Mở chi tiết đơn đã hoàn tiền.<br>2. Kiểm tra nhãn trạng thái.<br>3. Kiểm tra hành động xoá đơn. |
| **Expected Result** | Trạng thái Đã hoàn tiền hiển thị đúng; hành động xoá đơn xuất hiện/khả dụng theo thiết kế. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## TS-ADM-OS-013 – Kiểm tra xoá đơn hàng

| Field | Value |
|---|---|
| **Test Case ID** | TS-ADM-OS-013 |
| **Title** | Kiểm tra xoá đơn hàng |
| **Requirement** | REQ-ADM-047 |
| **Priority** | High |
| **Preconditions** | Đơn ở trạng thái được phép xoá; dùng dữ liệu test riêng |
| **Test Data** | Một đơn test có thể xoá |
| **Steps** | 1. Mở chi tiết đơn.<br>2. Chọn Xoá đơn.<br>3. Xác nhận nếu có hộp thoại.<br>4. Quay lại danh sách và tìm Order ID. |
| **Expected Result** | Đơn bị xoá/ẩn theo thiết kế; thông báo kết quả rõ ràng; không còn xuất hiện trong danh sách tương ứng. Không xoá đơn dữ liệu thật. |
| **Actual Result** | Chưa thực thi |
| **Status** | **NOT RUN** |
| **Evidence** | Add screenshot/video path |

## Notes cần xác nhận

- **TS-ADM-LOGIN-004:** Xác nhận chức năng “Ghi nhớ đăng nhập” có tồn tại và hành vi mong muốn.
- **TS-ADM-DASH-004 và TS-ADM-OM-004:** Xác nhận quy tắc tính doanh thu, đặc biệt đối với đơn huỷ/hoàn tiền.
- **TS-ADM-OS-009 và TS-ADM-OS-011:** Nội dung cùng mô tả luồng `Trả hàng → Đã về kho` nhưng liên kết Requirement ID khác nhau (`REQ-ADM-043` và `REQ-ADM-045`). Cần xác minh requirement gốc.
