# PostmanTest

GET /status

Trả về trạng thái của API

List of books
GET /books

Trả về 1 list danh sách 

Get a single book
GET /books/:bookId

Truy xuất thông tin chi tiết về một cuốn sách

Submit an order
POST /orders

Cho phép bạn gửi một đơn đặt hàng mới. Yêu cầu xác thực.

Phần thân yêu cầu cần phải ở định dạng JSON và bao gồm các thuộc tính sau:

bookId - Integer - Required
customerName - String - Required
Example

POST /orders/
{
  "bookId": 1,
  "customerName": "Trung"
}

Get all orders
GET /orders

Cho phép bạn xem tất cả các đơn đặt hàng. Yêu cầu xác thực.

Get an order
GET /orders/:orderId

Cho phép bạn xem một đơn đặt hàng hiện có. Yêu cầu xác thực

Update an order
PATCH /orders/:orderId

Cập nhật đơn hàng hiện có. Yêu cầu xác thực



