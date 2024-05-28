# JMeter
## Kiểm tra hiệu năng trang web
### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://www.geeksforgeeks.org/.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 10
  - Thời gian chạy: 3 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://www.geeksforgeeks.org/
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report

### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 998/1000 = 99,8%
- Số lượng yêu cầu thất bại: 2/1000 = 0,2%
- Thời gian phản hồi trung bình: 40 ms
- Thời gian phản hồi trung vị: 38 ms
- Thời gian phản hồi percentil 90: 70 ms
- Chuyển tải: 16 yêu cầu/giây
### Kết luận:

Trang web https://www.geeksforgeeks.org/ có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (99,8%), số lượng yêu cầu thất bại rất thấp (0,2%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web cũng khá cao (16 yêu cầu/giây).
### Hình ảnh tổng quát

![z5481246042585_43e222f8b942e6019359dafff783dd84](https://github.com/Geenutt/JMeter/assets/96821358/786a39b7-5f65-4202-b907-0d7c3cf14d6d)

## Kiểm tra hiệu năng API

### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
  - Thời gian chạy: 60 giây
  - Ramp-up period: 10 giây
- HTTP Request:
  - URL: https://openweathermap.org/current
  - Method: GET
  - Content encoding: UTF-8
- Listeners:
  - View Results Tree
  - Aggregate Report
### Kết quả kiểm tra:

![334016679-7ef95a94-377c-42ae-9f47-4b323fd73fd4](https://github.com/Geenutt/JMeter/assets/96821358/8d106380-fa3d-46dc-bb2a-d33324d271ff)


### Phân tích kết quả kiểm tra:

- Số lượng yêu cầu thành công: 996/1000 = 99,6%
- Số lượng yêu cầu thất bại: 4/1000 = 0,4%
- Thời gian phản hồi trung bình: 10
