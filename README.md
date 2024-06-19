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

Tạo bảng PhongBan

- MaPhongBan🔑:Khóa chính được sử dụng để xác định mỗi phòng ban một cách duy nhất, tự tăng.
- TenPhongBan :Tên phòng ban được đặt là NOT NULL để đảm bảo mỗi phòng ban được lưu trữ đều có thông tin tên. Điều này cực kỳ quan trọng để có thể phân biệt và quản lý các phòng ban.
 
![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/b54b2c48-e260-4c0e-b385-332f6917043e)

Tạo bảng NhanVien

- MaNhanVien🔑 :Khóa chính được sử dụng để xác định mỗi nhân viên một cách duy nhất, tự tăng.
- TenNhanVien :Tên nhân viên được đặt là NOT NULL để đảm bảo mỗi phòng ban được lưu trữ đều có thông tin tên. Điều này cực kỳ quan trọng để có thể phân biệt và quản lý các nhân viên.
- NgaySinh : Ngày sinh nhân viên
- DiaChi : Địa chỉ nhân viên
- SoDienThoai : Số điện thoại nhân viên
- MaPhongBan : Xác định mã phòng nhân viên

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/d5bfa76b-74b0-45ac-8784-24ca72f88014)


Tạo bảng DuAn

- MaDuAn🔑 :Khóa chính được sử dụng để xác định mỗi dự án một cách duy nhất, tự tăng.
- TenDuAn : Tên dự án được đặt là NOT NULL để đảm bảo mỗi phòng ban được lưu trữ đều có thông tin tên. Điều này cực kỳ quan trọng để có thể phân biệt và quản lý các dự án.
- NgayBatDau : Ngày bắt đầu dự án
- NgayKetThuc : Ngày kết thúc dự án
- MaPhongBan : Xác định mã phòng dự án

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/51be8cff-7791-4ae3-bad0-7b522161c847)


Tạo bảng PhanCong

- MaNhanVien : xác định mã phân công nhân viên
- MaDuAn : xác định mã phân công dự án


  ![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/b556bf80-e9db-4b30-821e-cbade217e0e8)


Sơ đồ liên kết

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/0a961726-f65b-42d4-b21a-0ce31191a114)


# 2 Thêm dữ liệu vào các bảng

-- Thêm dữ liệu vào bảng MaPhong

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/7875457f-8dcd-40e4-8322-68cf94430e17)


-- Thêm dữ liệu vào bảng NhanVien

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/03a4747e-d68c-4544-8a31-c7825cb17347)


-- Thêm dữ liệu vào bảng DuAn

![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/89d067f9-1df2-4e2e-8b0e-471d06e4c3ad)

-- Thêm dữ liệu vào bảng PhanCong


![image](https://github.com/DaoHoang1242003/QUANLYCONGTY/assets/173042044/2e83d99e-37a4-4c60-8035-29ca3820ce33)











