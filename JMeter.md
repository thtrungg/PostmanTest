# So sánh Performance(Load) Testing & API Testing 2 trang web (weatherapi.com & openweathermap.com)

**Với**: 
- Số lượng chủ đề – Đây là số lượng người dùng ảo mà chúng tôi dự kiến ​​​​sẽ kết nối với máy chủ: 1000
- Giai đoạn tăng tốc – Đây có thể được định nghĩa là thời gian mà JMeter có thể đưa số lượng luồng được đề cập ở trên vào trạng thái chạy: 100
- Số vòng lặp: 2

## Kết quả của trang openweathermap.com
![Screenshot_13](https://github.com/thtrungg/PostmanTest/assets/99778704/5eb1e0a2-2923-4e88-835c-23b0ab505e1d)
![Screenshot_16](https://github.com/thtrungg/PostmanTest/assets/99778704/fca03440-a93e-44c5-a47f-5927dd9bee7c)

## Kết quả của trang weatherapi.com
![Screenshot_8](https://github.com/thtrungg/PostmanTest/assets/99778704/3a6c41fb-18bc-43f5-9c94-dab52120cf59)
![Screenshot_15](https://github.com/thtrungg/PostmanTest/assets/99778704/c9ff55be-9e99-42aa-b20d-4fcd51c28f52)

## Kết quả phân tính thông số 2 trang web
![Screenshot_17](https://github.com/thtrungg/PostmanTest/assets/99778704/5d2b7dd1-3736-4b90-bf0d-1a0819d07f15)

## Phân tích:
- **Tổng số kết nối**: Giảm từ 120 xuống 82 kết nối, điều này có thể do cải thiện hiệu quả trong việc tái sử dụng các kết nối hiện có.
- **Số lượng yêu cầu bị lỗi**: Giảm từ 62 xuống 40, cho thấy hiệu suất và độ tin cậy của hệ thống đã được cải thiện.
- **Tổng số bytes truyền tải**: Tăng từ 1157 lên 1653 bytes, cho thấy lượng dữ liệu được truyền tải đã tăng lên.
- **Thời gian trung bình hoàn thành yêu cầu**: Tăng từ 69.35 ms lên 101.69 ms, cho thấy hệ thống mất nhiều thời gian hơn để xử lý mỗi yêu cầu.
- **Thời gian trung bình để thiết lập kết nối**: Tăng nhẹ từ 19.93 ms lên 19.99 ms, cho thấy sự thay đổi không đáng kể trong việc thiết lập kết nối.
- **Thời gian trung bình để nhận phản hồi đầu tiên**: Tăng từ 28.16 ms lên 92.32 ms, cho thấy thời gian để nhận phản hồi từ máy chủ đã tăng lên đáng kể.
- **Thời gian trung bình để nhận phản hồi đầy đủ**: Tăng từ 3.54 ms lên 3.83 ms, cho thấy thời gian để nhận toàn bộ phản hồi từ máy chủ đã tăng lên.
- **Tổng thời gian tiêu tốn**: Tăng từ 1447.05 ms lên 4729.0 ms, cho thấy tổng thời gian xử lý tất cả các yêu cầu đã tăng lên đáng kể.

## Kết luận:
Mặc dù có sự cải thiện về số lượng lỗi và số lượng kết nối, nhưng thời gian xử lý trung bình cho mỗi yêu cầu và tổng thời gian xử lý đã tăng lên đáng kể. Điều này có thể cho thấy hệ thống đang xử lý các yêu cầu phức tạp hơn hoặc có sự thay đổi trong cách các yêu cầu được xử lý, dẫn đến tăng thời gian xử lý. Việc tăng lượng dữ liệu truyền tải cũng có thể là một yếu tố góp phần
