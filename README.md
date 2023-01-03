# weather <br>
![alt](https://cdn.coursehunter.net/course/python-django-s-nulya-do-kommercheskih-prilozheniy.jpg) <br>
Cài đặt Django
  - pipenv install django 

chạy lệnh startproject mà Django cung cấp để tạo dự án.
  - django-admin startproject the_weather 

tạo database SQLite cho bạn, database mặc định trong cài đặt và nó đã thêm một số bảng vào database đó.
  - python manage.py migrate 

Để tạo ứng dụng, chạy lệnh:
  - python manage.py startapp weather

Ta sẽ tạo một folder templates

  - cd weather 
  - mkdir templates && cd templates 
  - mkdir weather 

  - bên trong folder weather, hãy tạo một file mới có tên là index.html. 

Sử dụng API thời tiết OpenWeather <br>
![alt](https://openweathermap.org/themes/openweathermap/assets/img/logo_white_cropped.png) <br>
Truy cập trang web, tạo account và sau đó đi tới các khóa API trên trang tổng quan của họ. 
Nhập tên và tạo khóa API mới. Khóa này sẽ cho phép ta sử dụng API để xem thời tiết.
 
Cài đặt các yêu cầu để có thể gọi API từ bên trong ứng dụng.
  - pipenv install request
  
Tạo một bảng trong database, cột này sẽ có một cột được gọi là tên, là tên của city. 
Thành phố này sẽ là một charfield, chỉ là một chuỗi.
Để có được những thay đổi này trong database, ta phải chạy makemigrations để tạo mã cập nhật database và di chuyển để áp dụng những thay đổi đó. 
  - python manage.py makemigrations 
  - python manage.py migrate 
  
khởi động server và truy cập lại.
  - python manage.py runserver 
