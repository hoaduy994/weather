# <h1>So sánh Virtual Machine – VM và Docker Container</h1> <br>
![alt](https://tel4vn.edu.vn/uploads/2020/09/so-sanh-may-ao-va-docker-container-tel4vn.edu_.vn-01.jpg) 
<br>
  - VM là ảo hóa về phần cứng
  - là một mô phỏng của hệ thống máy tính. Có thể tạo ra nhiều “máy tính logic” trên một “máy tính vật lý”.
  - hoạt động trên HyperV, cần 1 phần mềm để chạy đóng gói máy ảo
  - Tiêu tốn tài nguyên của máy
  - Cần một hệ điều hành đi kèm để máy ảo có thể hoạt động GuestOS
  - phân bổ bộ nhớ theo nhu cầu cần thiết, thời gian khởi động lâu
  - Hoàn toàn bị cô lập và an toàn hơn <br>
![alt](https://tel4vn.edu.vn/uploads/2020/09/so-sanh-may-ao-va-docker-container-tel4vn.edu_.vn-02.jpg) 
<br>
  - Docker container là ảo hóa về phần mềm
  - không sử dụng GuestOS -> hiệu suất hoạt động nhanh hơn
  - yêu cầu ít dung lượng bộ nhớ hơn
  - Cô lập ở mức tiến trình, có thể kém an toàn hơn
