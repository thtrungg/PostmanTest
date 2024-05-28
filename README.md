# PostmanTest

GET /status

Trả về trạng thái của API

# List of books
GET /books
Trả về 1 list danh sách **
![3](https://github.com/thtrungg/PostmanTest/assets/99778704/829a28ab-e6f1-4ecf-8ed0-0fd762339316)


# Get a single book
GET /books/:bookId
Truy xuất thông tin chi tiết về một cuốn sách
![2](https://github.com/thtrungg/PostmanTest/assets/99778704/39377266-2402-4ff4-aa56-49628726b17b)

# Submit an order
POST /orders
Cho phép bạn gửi một đơn đặt hàng mới. Yêu cầu xác thực.
![1](https://github.com/thtrungg/PostmanTest/assets/99778704/42e4104e-3686-4ca7-a17b-ba879b6e0103)

Phần thân yêu cầu cần phải ở định dạng JSON và bao gồm các thuộc tính sau:

bookId - Integer - Required
customerName - String - Required

POST /orders/
{
  "bookId": 1,
  "customerName": "Trung"
}

# Get all orders
GET /orders
Cho phép bạn xem tất cả các đơn đặt hàng. Yêu cầu xác thực.
![Screenshot 2024-05-28 121630](https://github.com/thtrungg/PostmanTest/assets/99778704/f445f814-0ea3-4a02-98bd-ab1279280666)

# Get an order
GET /orders/:orderId
Cho phép bạn xem một đơn đặt hàng hiện có. Yêu cầu xác thực
![getanorder](https://github.com/thtrungg/PostmanTest/assets/99778704/a9ae5f27-09b5-4495-98d3-05a081b70d8d)

# Update an order
PATCH /orders/:orderId
Cập nhật đơn hàng hiện có. Yêu cầu xác thực
![Upload](https://github.com/thtrungg/PostmanTest/assets/99778704/7368e3e0-a8e2-482e-8a08-26db0f8d7dfa)



