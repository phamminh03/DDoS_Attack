<<<<<<< HEAD
# ddosAttack
=======
## Đọc Dữ Liệu Từ Tệp và Khởi Tạo Biến
Chương trình bắt đầu bằng việc đọc dữ liệu từ tệp thông qua tham số dòng lệnh argv[1].
Khởi tạo các biến như line, key, t, value, mean, sum, variance, stdDeviation, H, và B.
Sử dụng một map có tên premapper để theo dõi số lượng kết nối đến từng cổng mục tiêu.
## Xử Lý Dữ Liệu
Chương trình tiếp tục bằng việc đọc dữ liệu từ tệp và phân tích nó trong vòng lặp while:
Mỗi dòng dữ liệu được chia thành các phần tử bằng dấu ',' và lưu trữ trong một vector có tên result.
Sau đó, các phần tử trong result được kết hợp để tạo ra một key, mà dường như là thông tin về cổng mục tiêu và địa chỉ IP.
Sử dụng premapper để theo dõi số lần xuất hiện của từng key.
Biến t được sử dụng để đếm số lượng bản ghi đã xử lý và dừng sau khi xử lý 500 bản ghi.
## Xử Lý Lặp và Phân Tích Dữ Liệu Lần Nữa
Chương trình tiếp tục xử lý dữ liệu trong vòng lặp while bên ngoài:
Lặp qua dữ liệu trong tệp và tạo một mapper mới để theo dõi số lần xuất hiện của từng key trong 500 bản ghi tiếp theo.
Tính toán giá trị trung bình (mean) và phương sai (variance) của số lần xuất hiện của các key trong mapper.
Tính độ lệch chuẩn (stdDeviation) dựa trên phương sai.
Duyệt qua mapper và tính giá trị entropy (H) dựa trên số lần xuất hiện và các giá trị từ premapper.
Dựa trên giá trị entropy và các ngưỡng (mean, B, stdDeviation), chương trình xác định xem liệu có cuộc tấn công DDoS hay không.
## Lặp Vào Lần Kế Tiếp (nếu cần)
Nếu bạn muốn thực hiện nhiều lần phân tích, chương trình cho phép nhập số lần (check) và lặp lại quá trình phân tích.
## Kết Thúc Và Đóng Tệp
- Khi đã hoàn thành phân tích hoặc gặp lỗi khi mở tệp, chương trình kết thúc và đóng tệp.
---
## Note
Giải thuật này sử dụng entropy để xác định sự không bình thường trong dữ liệu mạng, và nếu phát hiện, nó có thể tăng hoặc giảm ngưỡng B để điều chỉnh độ nhạy của phát hiện tấn công DDoS. 
Tuy nhiên, giải thuật này có thể cần được điều chỉnh và mở rộng để phù hợp với nhiều loại tấn công DDoS khác nhau.
>>>>>>> c9b329f85da974363ee5b2dbbb885448cb5144d7
# ddosAttack
# ddosAttack
