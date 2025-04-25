# baitap6
btvn 6 của sv: K225480106043_Nguyễn Giang Long_HQTCSDL

-Bài tập 6: Hệ quản trị CSDL

-Chủ đề: Câu lệnh Select

-Yêu cầu bài tập: 

-Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

Bài Làm:
1. import dữ liệu:

![image](https://github.com/user-attachments/assets/aecb1eef-ab5c-469b-b1ed-cc9b5bdaf319)

Sau đó create database ( ở đây e đặt là sv_tnut cho tiện với lệnh use sẵn có, ngoài ra có thể tùy biến):

Sau khi tạo database thì mở query mới, paste dữ liệu của file sv_tnut.sql vừa mở rồi execute:

![image](https://github.com/user-attachments/assets/aa314bd2-734b-4acd-af67-b7597f14a448)

![image](https://github.com/user-attachments/assets/d7069f4f-1133-4089-8a1e-38237f4f70e9)

2. Truy vấn dữ liệu đầu vào:
   Để truy vấn e tạo 1 query mới, ở đây e sẽ dùng lệnh select như trên để ảnh để thực hiện:

![image](https://github.com/user-attachments/assets/bd20daf3-b968-4b24-a61a-3912aac9cb13)

3.Nhập sql để tìm có sv nào trùng ngày tháng năm sinh với em 
 Vẫn tiếp tục là lệnh select với cú pháp như ảnh trên:

 ![image](https://github.com/user-attachments/assets/8489ccf1-9d91-4078-a9dc-79acd33f16b9)

4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
   Vẫn tiếp tục là lệnh select với cú pháp như ảnh trên:

   ![image](https://github.com/user-attachments/assets/053d365b-aa71-46d0-b90e-efa2274b81b4)

5.nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?

![image](https://github.com/user-attachments/assets/1d8d2bdd-7974-46ed-83f6-07d959b31864)

6.nhập sql để tìm xem có những sv nào trùng tên với em?

![image](https://github.com/user-attachments/assets/b53c0fc0-62de-481b-a45d-08e27cf1c257)

7.nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.

![image](https://github.com/user-attachments/assets/096da67a-16b6-4934-b8b5-c4c3b46c0537)

8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.

![image](https://github.com/user-attachments/assets/a79012e9-f031-4a11-be27-9a7ec768d5db)

9.BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.

![image](https://github.com/user-attachments/assets/87d62370-36e9-4b11-afa4-aa5d3e2d37b6)

where ...: lấy những dòng có chữ KMT 
order by: sắp xếp kết quả
[ten] COLLATE Vietnamese_CI_AS: Sắp xếp theo tên sinh viên, dùng bộ mã chuẩn tiếng Việt để phân biệt
[hodem] COLLATE Vietnamese_CI_AS: Nếu trùng tên thì sắp xếp tiếp theo họ đệm theo tiếng Việt.

10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VƯỚNG MẮC)?

Vì do kh có cột nào về giới tính nên em sẽ liệt kê những tên mà em có thể biết là của các bạn nữ( hoặc sử dụng dữ liệu trên mạng hoặc hỏi chat ai r cop), sau đó dùng lệnh Where và or những dữ liệu về tên cần thiết để lọc và liệt kê. Em nghĩ sẽ khó có thể liệt kê đầy đủ với cách trên nhưng mà phần trăm sai giới tính sẽ thấp. 

 ![image](https://github.com/user-attachments/assets/fe106223-8df9-4c08-8329-00b939433d82)
 

