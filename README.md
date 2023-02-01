# <h1>So sánh Virtual Machine – VM và Docker Container</h1> 
Virtual Machine – VM<br>
![alt](https://tel4vn.edu.vn/uploads/2020/09/so-sanh-may-ao-va-docker-container-tel4vn.edu_.vn-01.jpg) 
<br>
  - VM là ảo hóa về phần cứng
  - là một mô phỏng của hệ thống máy tính. Có thể tạo ra nhiều “máy tính logic” trên một “máy tính vật lý”.
  - hoạt động trên HyperV, cần 1 phần mềm để chạy đóng gói máy ảo
  - Tiêu tốn tài nguyên của máy
  - Cần một hệ điều hành đi kèm để máy ảo có thể hoạt động GuestOS
  - phân bổ bộ nhớ theo nhu cầu cần thiết, thời gian khởi động lâu
  - Hoàn toàn bị cô lập và an toàn hơn 

Docker Container<br>
![alt](https://tel4vn.edu.vn/uploads/2020/09/so-sanh-may-ao-va-docker-container-tel4vn.edu_.vn-02.jpg) 
<br>
  - Docker container là ảo hóa về phần mềm
  - không sử dụng GuestOS -> hiệu suất hoạt động nhanh hơn
  - yêu cầu ít dung lượng bộ nhớ hơn
  - Cô lập ở mức tiến trình, có thể kém an toàn hơn


# <h1>Tìm hiểu về CI/CD và cách cài đặt Jenkins</h1> 
# <h2>CI là gì?</h2>
  - Continuous Integration hay CI là một phương pháp phát triển phần mềm. Phương pháp này đòi hỏi các thành viên trong team cần phải tích hợp công việc với nhau một cách thường xuyên. Mỗi lần tích hợp sẽ được xây dựng một cách tự động nhằm mục đích phát hiện ra những lỗi phát sinh một cách nhanh nhất có thể. Khi sử dụng CI sẽ giúp làm giảm những vấn đề về tích hợp và cho phép các developer phát triển phần mềm được nhanh hơn và đúng tiến độ hơn.
  - Quy trình công việc điển hình cho Tích hợp liên tục (CI) bao gồm các bước sau:

    + Commit: Dev commit code lên repo (ví dụ: Git).

    + Build: CI server được thông báo về thay đổi mã và tự động kích hoạt quá trình xây dựng.

    + build & test: CI server kiểm tra code mới nhất từ kho lưu trữ và build. auto test được chạy để xác thực các thay đổi và đảm bảo rằng ứng dụng hoạt động như mong đợi.

    + feedback: CI server cung cấp phản hồi về kết quả build & test, bao gồm mọi lỗi. Phản hồi này có thể ở dạng thông báo, nhật ký và báo cáo.

    + fix & repeat: Nếu quá tình build hoặc test không thành công, nhóm phát triển sẽ được thông báo và có thể khắc phục sự cố. Sau khi các sự cố được giải quyết, chu trình sẽ lặp lại từ bước 1.

    + Deploy: Nếu tất cả các bước trên thành công, các thay đổi sẽ tự động được triển khai sang môi trường staging hoặc production.

Chu kỳ này được lặp lại nhiều lần trong ngày, đảm bảo rằng các thay đổi mã được tích hợp và kiểm tra thường xuyên, giảm nguy cơ xung đột và đảm bảo rằng ứng dụng luôn ở trạng thái có thể phát hành được.
  
  ![alt](https://d3hi6wehcrq5by.cloudfront.net/itnavi-blog/2021/07/CI-CD-la-gi-1.png)
  
  
 # <h2>CD là gì?</h2>
  - Continuous Delivery (CD) là một phương pháp phát triển phần mềm tập trung vào việc tự động hóa toàn bộ quá trình phân phối phần mềm từ phát triển đến sản xuất. Nó là phần mở rộng của CI, trong đó các nhà phát triển thường xuyên tích hợp mã vào kho lưu trữ dùng chung và các thử nghiệm tự động được chạy để xác thực các thay đổi.

  - Trong CD, các thay đổi mã được tự động triển khai vào môi trường thử nghiệm sau khi vượt qua các bài kiểm tra CI và chỉ khi vượt qua các bài kiểm tra bổ sung và kiểm tra chất lượng, chúng mới được triển khai vào sản xuất. Cách tiếp cận này cho phép cung cấp các tính năng mới và sửa lỗi một cách nhanh chóng và đáng tin cậy mà không cần can thiệp thủ công hoặc quy trình phát hành phức tạp.

  - Mục tiêu của Phân phối liên tục là cho phép các tổ chức phát hành phần mềm nhanh hơn và với độ tin cậy cao hơn, bằng cách tự động hóa càng nhiều quy trình phân phối càng tốt và loại bỏ các lỗi thủ công. Điều này giúp các tổ chức phản ứng nhanh hơn với nhu cầu thay đổi của khách hàng và điều kiện thị trường, đồng thời cung cấp phần mềm chất lượng cao với tốc độ nhanh hơn.
  
  
<h2>Cách cài đặt Jenkins trên CentOS 7</h2>
