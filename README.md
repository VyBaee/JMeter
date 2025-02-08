BÁO CÁO KIỂM THỬ HIỆU SUẤT BẰNG JMETER

1. Giới thiệu

1.1 Mục tiêu kiểm thử

Mục tiêu của kiểm thử hiệu suất là đánh giá khả năng chịu tải của hệ thống, đo lường thời gian phản hồi và xác định giới hạn hiệu suất của trang web thương mại điện tử.

1.2 Môi trường kiểm thử

Công cụ sử dụng: Apache JMeter

Hệ điều hành: Window

CPU: AMD Ryzen 7 4800H

RAM: 16GB

Trình duyệt thử nghiệm: www.example.com

2. Thiết lập kiểm thử

2.1 Kịch bản kiểm thử hiệu suất

Số lượng người dùng (Threads): 50

Ramp-up time: 300 giây (5 phút)

Loop Count: 5 lần

Mô phỏng yêu cầu HTTP đến trang chủ của website

Dữ liệu ghi nhận: Thời gian phản hồi trung bình, throughput, error rate

2.2 Kiểm thử tải (Load Testing)

Số lượng người dùng tăng dần: 10 → 50

Dữ liệu thu thập:

Thời gian phản hồi trung bình: 19 ms

Throughput: 23.5 requests/min

Tỷ lệ lỗi (%): 0

2.3 Kiểm thử khả năng chịu tải (Stress Testing)

Số lượng người dùng tăng lên: 100

Dữ liệu thu thập:

Thời gian phản hồi trung bình: 18 ms

Throughput: 29.5 requests/min

Tỷ lệ lỗi (%): 0

Điểm bắt đầu giảm hiệu suất: 0

3. Phân tích kết quả

3.1 Hiệu suất hệ thống

Thời gian phản hồi trung bình: 20 ms

Throughput tối đa đạt được: 25.5 requests/sec

Tỷ lệ lỗi tối đa: 0 %

3.2 Xác định Bottleneck

Dấu hiệu Bottleneck: Không

Nguyên nhân có thể gây Bottleneck: Không

Quan sát hệ thống khi tăng tải: Không

4. Kết luận và đề xuất

4.1 Kết luận

Dựa trên kết quả thu được, hệ thống đạt yêu cầu hiệu suất. Hiệu suất hệ thống ổn định khi số lượng người dùng tăng lên 100.

4.2 Đề xuất cải thiện hiệu suất

Tối ưu truy vấn database nếu thời gian phản hồi cao.

Tăng cường caching để giảm tải cho server.

Sử dụng load balancer nếu throughput thấp.

Tăng tài nguyên máy chủ (CPU, RAM) nếu hệ thống bị quá tải.

5. Câu hỏi thảo luận

Tại sao kiểm thử phi chức năng lại quan trọng trong phần mềm?

Các thông số quan trọng cần theo dõi trong kiểm thử hiệu suất là gì?

Nếu hệ thống không đáp ứng yêu cầu hiệu suất, bạn sẽ đề xuất giải pháp gì?
