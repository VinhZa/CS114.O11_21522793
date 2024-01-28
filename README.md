
# PHÂN LOẠI HÌNH ẢNH TRONG THƯ VIỆN ĐIỆN THOẠI

Đề tài nghiên cứu, phát triển hệ thống với chức năng phân loại các hình ảnh có thể xuất hiện trong thư viện điện thoại và sắp xếp chúng vào cùng 1 thư mục.


## Sinh viên thực hiện
Nhóm sinh viên trường Đại học Công nghệ Thông tin Đại học Quốc gia-TP.HCM :
- Đỗ Trí Gia Bảo - 21520603
- Nguyễn Thành Vinh - 21522793
- Trương Lê Diễn - 21520189

## Giảng viên hướng dẫn
- PhGS.TS. Lê Đình Duy
- ThS. Phạm Nguyễn Trường An
  
## Mục lục
1. [ Mở đầu. ](#mở-đầu)
2. [ Công cụ và ngôn ngữ lập trình. ](#công-cụ-và-ngôn-ngữ-lập-trình)
3. [ Tổng quan. ](#tổng-quan)
- [ Mô tả bài toán ](#mô-tả-bài-toán)
- [ Dataset ](#dataset)
4. [ Hướng thực hiện. ](#Hướng-thực-hiện)
5. [ Đánh giá và tổng kết. ](#đánh-giá-và-tổng-kết)
6. [ Tài liệu tham khảo. ](#tài-liệu-tham-khảo)


## Mở đầu
Bắt đầu từ nhu cầu ngày càng tăng về quản lý ảnh trên điện thoại di động, dự án Machine Learning của nhóm ra đời với mục tiêu giải quyết thách thức này một cách tự động và hiệu quả hơn bằng cách áp dụng các phương pháp học máy đặc biệt là mô hình supervised learning vào bài toán phân loại hình ảnh. Mục tiêu cốt lõi của dự án là xây dựng một hệ thống tự động có khả năng nhận diện và phân loại các hình ảnh, sau đó tự động sắp xếp chúng vào các thư mục hoặc danh mục có nhãn tương ứng


## Công cụ và ngôn ngữ lập trình

Đề tài được lập trình bằng ngôn ngữ Python và chạy trên Google Colab.
- Ngôn ngữ lập trình: Python
- Môi trường lập trình: Google Colab


## Tổng quan
### Mô tả bài toán
Đề tài của nhóm có yêu cầu là hiện thực một hệ thống mà khi người dùng đưa ảnh vào với các nội dung trong ảnh là ngẫu nhiên, mô hình máy học sẽ tự động nhận dạng và hình ảnh sẽ được đưa vào thư mục có label tương ứng với ảnh.

#### Input
- Input: một ảnh có nội dung ngẫu nhiên

#### Output
- Output: label của ảnh, sau đó dựa trên label đó sẽ đưa ảnh vào folder có label tương ứng.

#### Ngữ cảnh ứng dụng
Với bối cảnh ứng dụng là trên một thư viện chứa ảnh của điện thoại, khi người sử dụng ngẫu nhiên mở điện thoại lên và chụp hoặc lưu một ảnh thì ảnh sẽ được đẩy vào thư viện chính. Nhưng sau một thời gian khi số lượng ảnh nạp vào quá lớn và bạn cần lấy ra ảnh cần thiết là rất khó khăn và mất thời gian vì có quá nhiều nội dung, việc hiện thực một mô hình như trên giúp cho việc quản lí các ảnh trong thư viện điện thoại trở nên dễ dàng hơn

### Tập dữ liệu
- Tập dữ liệu bao gồm 2000 chia ra thành 4 chủ đề: Car,Cat,Human,Flower.
- Nguồn thu thập dữ liệu: các trang web và mạng xã hội.

## Hướng thực hiện
Bài toán Machine Learning này được thực hiện dựa trên mô hình CNN tuần tự và sử dụng các hàm sẵn có trong thư viện Keras
![image](https://github.com/VinhZa/CS114.O11_21522793/assets/106794944/af3a74b1-c4a7-48aa-9424-a72b3ab7fed3)

## Đánh giá và tổng kết
Thực hiện đánh giá với tập test gồm 400 ảnh chứa các chủ đề đã nói nhưng không được gắn nhãn, kết quả thu được như sau:
![image](https://github.com/VinhZa/CS114.O11_21522793/assets/106794944/b91ebe46-c61e-4e7d-b3bb-90687130c7a4)
Có thể thấy hệ thống đã hoạt động và có độ chính xác ở 15 lần lặp là 0,88.

## Tài liệu tham khảo
- [Convolutional Neural Network (CNN)](https://www.tensorflow.org/tutorials/images/cnn)

