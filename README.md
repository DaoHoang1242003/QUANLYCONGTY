# QUẢN LÝ CÔNG TY
- Họ Tên : Đào Việt Hoàng
- Mã sinh vinh viên : K215480106068
- Lớp : K57KMT
- Ngày làm : 19/6/2024
## Chức Năng Cơ Bản
# 1. Quản lý 
1.1. Quản lý phòng ban
- Thêm phong ban: Cho phép thêm mới một phong ban vào cơ sở dữ liệu
- Sửa thông tin phong ban: Cho phép chỉnh sửa thông tin của một phong ban đã tồn tại
- Xóa phong ban: Cho phép xóa một phong ban khỏi cơ sở dữ liệu
- Xem danh sách phong ban: Hiển thị danh sách tất cả các phong ban

1.2. Quản lý nhân viên
- Thêm nhân viên: Cho phép thêm mới một nhân viên vào cơ sở dữ liệu
- Sửa thông tin nhân viên: Cho phép chỉnh sửa thông tin của một nhân viên đã tồn tại
- Xóa nhân viên: Cho phép xóa một nhân viên khỏi cơ sở dữ liệu
- Xem danh sách nhân viên: Hiển thị danh sách tất cả các nhân viên

1.3. Quản lý dự án
- Thêm dự án: Cho phép thêm mới một dự án vào cơ sở dữ liệu
- Sửa thông tin dự án: Cho phép chỉnh sửa thông tin của một dự án đã tồn tại
- Xóa dự án: Cho phép xóa một dự án khỏi cơ sở dữ liệu
- Xem danh sách dự án: Hiển thị danh sách tất cả các dự án
  
1.4. Quản lý phân công
- Thêm phân công: Cho phép thêm mới một nhân viên vào cơ sở dữ liệu
- Sửa thông tin phân công: Cho phép chỉnh sửa thông tin của một nhân viên đã tồn tại
- Xóa phân công: Cho phép xóa một nhân viên khỏi cơ sở dữ liệu
- Xem danh sách phân công: Hiển thị danh sách tất cả các nhân viên
  
2. Chức Năng Truy Vấn
  
- Tìm kiếm công ty doanh nghiệp theo tên 
- Tìm kiếm nhân viên hoặc nhà hàng theo công ty 
- Xem chi tiết đánh giá của một công ty cụ thể
- Xem chi tiết thông tin nhân viên

# Thiết kế chương trình trong SQL

##1. Tạo các bảng

Tạo bảng phòng ban

- MaPhongBan🔑:Khóa chính được sử dụng để xác định mỗi phòng ban một cách duy nhất, tự tăng.
- TenPhongBan :Tên phòng ban được đặt là NOT NULL để đảm bảo mỗi phòng ban được lưu trữ đều có thông tin tên. Điều này cực kỳ quan trọng để có thể phân biệt và quản lý các phòng ban.
 






