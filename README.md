# Báo cáo kiểm thử hiệu năng bằng JMeter
Thông tin sinh viên
Họ tên: Trương Đan Huy
MSSV: bit220078
Website được kiểm thử: https://www.reddit.com
**Mô tả kịch bản kiểm thử**
Dựa trên MSSV bit220078 (2 chữ số cuối là 78):

*Kịch bản 1: Cơ bản*

Số lượng người dùng: 10 + (78 % 10) = 10 + 8 = 18 người dùng
Hành vi: Gửi yêu cầu GET đến trang chủ https://www.reddit.com
Loop Count: 5
*Kịch bản 2: Tải nặng*

Số lượng người dùng: 50 + (78 % 20) = 50 + 18 = 68 người dùng
Ramp-up Period: 30 giây
Hành vi: Gửi yêu cầu GET đến trang chủ https://www.reddit.com và một trang con 
URL trang chủ: https://www.reddit.com
URL trang con: [https://www.reddit.com/r/popular]
*Kịch bản 3: Tùy chỉnh*

Số lượng người dùng: 20 + (78 % 15) = 20 + 3 = 23 người dùng
Thời gian chạy: 60 giây
Hành vi: Gửi yêu cầu GET (hoặc POST nếu có, ví dụ form tìm kiếm) đến 2 trang con khác nhau (sinh viên tự chọn).
Yêu cầu 1: Gửi yêu cầu GET đến https://www.reddit.com/t/announcements]
Yêu cầu 2: Gửi yêu cầu GET đến [https://www.reddit.com/r/gaming] 
Kết quả kiểm thử


_Kịch bản 1:_

Response Time trung bình: [Điền giá trị] ms
Throughput: 1.2/giây
Error Rate: 0%
![{5464E5D8-1A59-4D35-9EFA-474C86BE0F72}](https://github.com/user-attachments/assets/1afa162e-3802-418e-9290-dfd253aaa37b)
_Kịch bản 2:_

Response Time trung bình: [Điền giá trị] ms
Throughput: 30/giây
Error Rate: 100%

_Kịch bản 3:_

Response Time trung bình: [Điền giá trị] ms
Throughput: 53/giây
Error Rate: 0%
![{8258624A-297D-4E50-8009-54219D34FBF0}](https://github.com/user-attachments/assets/a283057e-e711-465a-8312-cfb841dd93bd)
