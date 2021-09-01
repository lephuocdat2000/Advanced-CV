# Social Distancing Violation Detection

Yolov4: 

![image](https://user-images.githubusercontent.com/62682595/131688303-b245c4ac-c573-4262-8781-914c0b1fac78.png)

Hướng giải quyết:
![image](https://user-images.githubusercontent.com/62682595/131688446-e94975a6-2567-4484-a3e9-9edb3bf2d84d.png)

 Xác định vùng ROI:
   Lấy 7 điểm: 
    +4 điểm xác định khu vực Roi
    +3 điểm còn lại đánh dấu theo chiều ngang và chiều dọc khoảng 200 cm so với thực tế.    
    
 ![image](https://user-images.githubusercontent.com/62682595/131688631-aa549ed9-b10a-4a6e-ae88-598a8ca7942c.png)

   Ma trận chuyển đổi
 ![image](https://user-images.githubusercontent.com/62682595/131689248-686f23b3-2abc-4bb4-a867-5322c01cad64.png)
 
   Bird-eye view
   
 ![image](https://user-images.githubusercontent.com/62682595/131689417-efda15fc-0bd1-4dae-a008-4a3d29a3451a.png)
 
   Tính khoảng cách
   
 ![image](https://user-images.githubusercontent.com/62682595/131689763-f6272f5d-0dc0-4cde-8c61-93ef327b7ad6.png)
 ![image](https://user-images.githubusercontent.com/62682595/131689780-27199ab2-7e72-49ef-a9cd-9be85fe7af81.png)

Đánh gia mô hình: 

  - Sử dụng độ đo MAP để đánh giá mô hình Object Detection (0.81)
  - Sử dụng Mean Absolute Error để đánh giá mô hình chuyển đổi Bird-eye view ( ~0.13 m )








