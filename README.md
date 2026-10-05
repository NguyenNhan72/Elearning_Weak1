# Bài tập: Xây dựng giao diện UI Profile (Lập trình thiết bị di động)

##  1. Mô tả bài tập
Ứng dụng di động đơn giản được phát triển bằng ngôn ngữ **Kotlin** kết hợp với bộ công cụ giao diện hiện đại **Jetpack Compose**. Dự án tái hiện lại giao diện trang cá nhân (Profile Screen) theo mẫu thiết kế yêu cầu với các thành phần trực quan.

---

##  2. Mục tiêu bài tập
* Làm quen với môi trường phát triển ứng dụng di động trên Android Studio và cấu trúc dự án Kotlin.
* Vận dụng thành thạo **Jetpack Compose** để xây dựng giao diện bố cục (Layout) hiện đại.
* Xây dựng các thành phần cơ bản: Thanh tiêu đề (Header), căn chỉnh bố cục đối xứng, xử lý hình ảnh bo tròn (Circle Avatar) và tùy chỉnh typography (kiểu chữ, màu sắc).

---

##  3. Kết quả đạt được
* **Giao diện hoàn thiện:** 
  * Góc trên bên trái: Nút mũi tên quay lại (`Back`) có viền bo góc.
  * Góc trên bên phải: Nút ghi chú/chỉnh sửa (`Edit`) với tông màu xanh đặc trưng.
  * Vùng trung tâm: Ảnh đại diện cá nhân được cắt tròn sắc nét, hiển thị họ tên đầy đủ và mã số sinh viên được căn giữa cân đối.


---

##  4. Giải thích các hàm & Thành phần chính
* **`MainActivity`**: Lớp khởi chạy (`ComponentActivity`) điểm đầu vào của ứng dụng, chịu trách nhiệm gọi hàm giao diện thông qua khối `setContent`.
* **`ProfileScreen()`**: Hàm `@Composable` chính chứa toàn bộ mã nguồn bố cục màn hình hồ sơ cá nhân.
* **`Column`**: Bố cục sắp xếp các thành phần con theo chiều dọc (từ trên xuống dưới), hỗ trợ thiết lập màu nền và khoảng cách lề (`padding`).
* **`Row`**: Bố cục sắp xếp các thành phần theo chiều ngang, kết hợp thuộc tính `Arrangement.SpaceBetween` để đẩy nút Back sang trái và nút Edit sang phải.
* **`Image` kết hợp `.clip(CircleShape)`**: Tải ảnh tài nguyên từ thư mục `drawable` và cắt khung ảnh thành hình tròn hoàn hảo.
* **`Spacer`**: Tạo các khoảng trống đệm có kích thước cố định (`dp`) giúp bố cục các dòng chữ và hình ảnh không bị dính sát vào nhau.

---

##  5. Hình ảnh đầu ra (Output Preview)
<img width="371" height="727" alt="image" src="https://github.com/user-attachments/assets/e3597ce2-769c-400e-bdab-a678cb70aa36" />

