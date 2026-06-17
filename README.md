# Báo Cáo Bài Tập: Tìm Hiểu Và Thực Hành Kiểm Thử Tải Với JMeter

## 1. Mục tiêu bài tập
* Tìm hiểu khái niệm cơ bản về Kiểm thử hiệu năng (Performance Testing) và Kiểm thử tải (Load Testing).
* Làm quen với giao diện Apache JMeter và biết cách cấu hình kịch bản kiểm thử cơ bản.
* Giả lập tải trọng với nhiều người dùng truy cập đồng thời để đo lường phản hồi của hệ thống.

---

## 2. Các bước thực hiện chi tiết

### Bước 1: Cài đặt công cụ
* Tải tệp cấu hình Apache JMeter từ trang chủ và giải nén.
* Kích hoạt phần mềm thông qua file thực thi `jmeter.bat` trong thư mục `bin`.

### Bước 2: Thiết lập kịch bản kiểm thử tải (Test Plan)
* **Khởi tạo Thread Group:** Cấu hình giả lập số lượng người dùng đồng thời.
  * *Number of Threads (Users):* 10 người dùng.
  * *Ramp-up period (seconds):* 2 giây.
  * *Loop Count:* 1 lần.
* **Cấu hình HTTP Request:** Thiết lập gửi yêu cầu kiểm thử tới địa chỉ Server máy chủ thử nghiệm.
* **Thêm Bộ lắng nghe (Listener):** Sử dụng thành phần `View Results in Tree` để ghi nhận và hiển thị trực quan các kết quả phản hồi trả về từ Server.

### Bước 3: Thực thi và thu thập kết quả
* Tiến hành chạy kịch bản kiểm thử bằng cách nhấn nút **Start**.
* Hệ thống ghi nhận các lượt gửi yêu cầu tải thành công với trạng thái phản hồi hợp lệ (Hiển thị các icon tích xanh trong cây kết quả).
  
---

## 3. Hình ảnh minh họa kết quả thực hiện JMeter
<img width="1920" height="1080" alt="Screenshot 2026-06-17 163844" src="https://github.com/user-attachments/assets/371a2e66-266d-4a83-a8cd-1540cb473b12" />
