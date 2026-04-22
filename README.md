# 🌿 ĐẶC TẢ BÀI TOÁN

---

## 1. Tên bài toán

Xây dựng hệ thống quản lý cửa hàng bán trà thảo mộc  

---

## 2. Bối cảnh bài toán

Trong bối cảnh nhu cầu sử dụng các sản phẩm tự nhiên và tốt cho sức khỏe ngày càng tăng, các cửa hàng trà thảo mộc phát triển với số lượng sản phẩm đa dạng như:

- Trà hoa (hoa cúc, hoa hồng…)  
- Trà lá (bạc hà, lá sen…)  
- Trà phối trộn (detox, ngủ ngon…)  

Tuy nhiên, trong quá trình vận hành, cửa hàng gặp nhiều khó khăn:

- Dữ liệu sản phẩm phân tán, khó kiểm soát  
- Không theo dõi chính xác tồn kho và hạn sử dụng  
- Nhân viên bán hàng xử lý thủ công → dễ sai sót  
- Người dùng khó tìm được sản phẩm phù hợp  
- Chưa có hệ thống gợi ý sản phẩm  

Do đó, cần xây dựng một hệ thống có khả năng:

- Quản lý dữ liệu tập trung  
- Hỗ trợ bán hàng  
- Hiển thị và tìm kiếm sản phẩm  
- Gợi ý sản phẩm phù hợp  
- Tích hợp thanh toán bằng quét mã QR để tăng tốc độ bán hàng  

---

## 3. Mục tiêu bài toán

### 3.1. Mục tiêu tổng quát

Xây dựng một hệ thống web hỗ trợ quản lý cửa hàng trà thảo mộc và nâng cao trải nghiệm người dùng thông qua tìm kiếm, gợi ý và thanh toán nhanh bằng mã QR.  

---

### 3.2. Mục tiêu cụ thể

- Quản lý dữ liệu sản phẩm và kho  
- Hỗ trợ nhân viên bán hàng  
- Hiển thị sản phẩm cho người dùng  
- Tìm kiếm và lọc sản phẩm  
- Gợi ý sản phẩm phù hợp  
- Hỗ trợ quét mã QR khi thanh toán  
- Tạo nền tảng mở rộng trong tương lai  

---

## 4. Phát biểu bài toán

Cho trước một tập dữ liệu sản phẩm trà thảo mộc với các thuộc tính:

- Tên sản phẩm  
- Loại sản phẩm  
- Giá bán  
- Thành phần  
- Hạn sử dụng  
- Số lượng tồn kho  

Yêu cầu xây dựng một hệ thống có khả năng:

- Lưu trữ và quản lý dữ liệu sản phẩm  
- Hỗ trợ nhân viên bán hàng  
- Hiển thị dữ liệu trên website  
- Cho phép người dùng tìm kiếm và lọc sản phẩm  
- Hỗ trợ gợi ý sản phẩm dựa trên dữ liệu  
- Cho phép thanh toán bằng cách quét mã QR sản phẩm  

---

## 5. Đối tượng của bài toán

### 5.1. Đối tượng dữ liệu

Dữ liệu sản phẩm bao gồm:

- Tên sản phẩm  
- Loại sản phẩm  
- Giá  
- Thành phần  
- Hạn sử dụng  
- Số lượng tồn kho  
- Mô tả  
- Mã định danh sản phẩm (dùng để tạo QR)  

---

### 5.2. Đối tượng sử dụng hệ thống

####  1. Quản trị viên (Admin)

**Vai trò:**  
Là người quản lý cao nhất của hệ thống.  

**Chức năng:**
- Quản lý toàn bộ sản phẩm  
- Quản lý kho hàng  
- Theo dõi doanh thu và báo cáo  
- Quản lý nhân viên  
- Tạo và quản lý mã QR cho sản phẩm  

**Mục tiêu:**
- Kiểm soát hoạt động kinh doanh  
- Đảm bảo dữ liệu chính xác  

---

####  2. Nhân viên (Staff)

**Vai trò:**  
Người trực tiếp vận hành bán hàng tại cửa hàng.  

**Chức năng:**
- Tạo đơn hàng  
- Tư vấn sản phẩm cho khách  
- Kiểm tra tồn kho  
- Quét mã QR sản phẩm khi thanh toán  
- Cập nhật thông tin khách hàng  

**Mục tiêu:**
- Bán hàng nhanh, chính xác  
- Giảm thao tác nhập liệu thủ công  

---

####  3. Người dùng (Customer)

**Vai trò:**  
Khách hàng sử dụng hệ thống để tìm và xem sản phẩm.  

**Chức năng:**
- Xem danh sách sản phẩm  
- Tìm kiếm sản phẩm  
- Lọc sản phẩm theo nhu cầu  
- Xem chi tiết sản phẩm  
- Nhận gợi ý sản phẩm  

**Mục tiêu:**
- Tìm sản phẩm nhanh  
- Dễ dàng lựa chọn sản phẩm phù hợp  

---

## 6. Đầu vào của bài toán

Hệ thống nhận đầu vào từ:

- Dữ liệu sản phẩm  
- Thông tin tìm kiếm từ người dùng  
- Dữ liệu hành vi (xem sản phẩm, lọc…)  
- Dữ liệu quét từ mã QR sản phẩm khi thanh toán  

---

## 7. Đầu ra của bài toán

Hệ thống cung cấp các đầu ra sau:

- Danh sách sản phẩm  
- Kết quả tìm kiếm  
- Kết quả lọc  
- Thông tin chi tiết sản phẩm  
- Danh sách sản phẩm gợi ý  
- Thông tin sản phẩm sau khi quét QR và cập nhật vào hóa đơn  

---

## 8. Yêu cầu chức năng

### 8.1. Quản lý dữ liệu (Admin)

- Nhập dữ liệu sản phẩm  
- Thêm / sửa / xóa sản phẩm  
- Quản lý tồn kho  
- Kiểm tra hạn sử dụng  
- Tạo mã QR cho từng sản phẩm  

---

### 8.2. Bán hàng (Nhân viên)

- Tạo đơn hàng  
- Chọn sản phẩm hoặc quét mã QR  
- Nhập số lượng  
- Kiểm tra tồn kho  
- Thanh toán  

**Quy trình quét QR:**
- Nhân viên quét mã QR trên sản phẩm  
- Hệ thống nhận mã định danh  
- Tự động truy xuất thông tin sản phẩm  
- Thêm sản phẩm vào hóa đơn  

---

### 8.3. Hiển thị sản phẩm (Người dùng)

- Hiển thị danh sách sản phẩm  
- Hiển thị thông tin cơ bản  
- Xem chi tiết sản phẩm  

---

### 8.4. Tìm kiếm và lọc

- Tìm theo tên sản phẩm  
- Lọc theo loại sản phẩm  
- Lọc theo mức giá  
- Kết hợp nhiều điều kiện  

---

### 8.5. Gợi ý sản phẩm

- Gợi ý sản phẩm cùng loại  
- Gợi ý sản phẩm có mức giá tương tự  
- Gợi ý sản phẩm phổ biến  

---

## 9. Yêu cầu phi chức năng

### 9.1. Tính chính xác
- Dữ liệu hiển thị phải chính xác  
- Kết quả tìm kiếm phải đúng  

### 9.2. Hiệu năng
- Thời gian phản hồi nhanh  
- Quét QR phải xử lý gần như tức thời  

### 9.3. Giao diện
- Dễ sử dụng  
- Thân thiện với nhân viên bán hàng  

### 9.4. Khả năng mở rộng
- Có thể mở rộng QR cho quản lý kho  
- Có thể nâng cấp thành barcode hoặc RFID  

---

## 10. Phạm vi bài toán

### 10.1. Phạm vi thực hiện

- Quản lý sản phẩm  
- Quản lý kho  
- Hỗ trợ bán hàng  
- Tìm kiếm và lọc sản phẩm  
- Gợi ý sản phẩm cơ bản  
- Thanh toán bằng quét mã QR  

