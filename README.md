# QLDACNTT
Quản lý khách sạn
Giới thiệu
Dự án Quản lý khách sạn được xây dựng nhằm hỗ trợ quản lý các hoạt
động cơ bản của khách sạn, bao gồm quản lý khách hàng, phòng, loại
phòng, đặt phòng và dịch vụ. Hệ thống giúp lưu trữ thông tin tập trung,
tra cứu dữ liệu thuận tiện và theo dõi tình trạng phòng cũng như đặt
phòng.
Chức năng chính
- Quản lý thông tin khách hàng.
- Quản lý loại phòng và thông tin phòng.
- Theo dõi trạng thái phòng.
- Quản lý đặt phòng, ngày nhận và ngày trả.
- Quản lý chi tiết phòng trong từng đơn đặt phòng.
- Quản lý dịch vụ của khách sạn.
Thiết kế cơ sở dữ liệu
Cơ sở dữ liệu được tổ chức thành các bảng riêng biệt để lưu trữ từng
nhóm thông tin. Các bảng liên kết với nhau thông qua khóa chính (PK) và
khóa ngoại (FK), giúp hạn chế trùng lặp dữ liệu và đảm bảo tính liên
kết.
Các bảng dự kiến
  Bảng                    Các trường tiêu biểu    Mục đích
  KhachHang             MaKH (PK), HoTen,   Lưu thông tin khách
CCCD, SDT, Email  hàng

  LoaiPhong             MaLoai (PK),          Lưu thông tin từng loại
TenLoai, MoTa,      phòng
SucChua, GiaMacDinh 

  Phong                 MaPhong (PK),         Quản lý phòng; loại
SoPhong, MaLoai     phòng được tham chiếu
(FK), TrangThai       qua MaLoai

  DatPhong              MaDatPhong (PK),      Lưu thông tin đặt phòng
MaKH (FK), NgayTao, và khách đặt
NgayNhan, NgayTra,
TrangThai             

  ChiTietDatPhong       MaDatPhong (PK, FK),  Liên kết đơn đặt phòng
MaPhong (PK, FK),     với các phòng được đặt
DonGia                
DichVu                MaDV (PK), TenDV,   Lưu danh mục dịch vụ
DonGia
Công nghệ sử dụng
- Ngôn ngữ: (điền ngôn ngữ sử dụng)
- Cơ sở dữ liệu: (điền hệ quản trị cơ sở dữ liệu)
- Công cụ phát triển: (điền IDE / công cụ)
Cài đặt và chạy chương trình
1. Clone repository về máy:
   git clone <link-repository>
2. Mở thư mục dự án bằng công cụ phát triển phù hợp.
3. Cấu hình kết nối cơ sở dữ liệu.
4. Tạo cơ sở dữ liệu và các bảng theo cấu trúc dự án.
5. Chạy chương trình.
Thành viên thực hiện
- (Tên thành viên 1)
- (Tên thành viên 2)