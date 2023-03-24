# Data Analyst Portfolio Project (Python)
## BÁO CÁO NHÓM - DỰ ĐOÁN LIỆU KHÁCH HÀNG CÓ VỠ NỢ KHOẢN VAY MUA XE HAY KHÔNG?
## TỔNG QUAN ĐỀ TÀI
Tổ chức tài chính phi ngân hàng (NBFI) hoặc công ty tài chính phi ngân hàng (NBFC) là
Tổ chức tài chính không có giấy phép hoạt động ngân hàng đầy đủ hoặc không được giám
sát bởi cơ quan quản lý ngân hàng quốc gia hoặc quốc tế. NBFC tạo điều kiện thuận lợi
cho các dịch vụ tài chính liên quan đến ngân hàng, chẳng hạn như đầu tư, tổng hợp rủi ro,
tiết kiệm theo hợp đồng và môi giới thị trường.

Một NBFI đang gặp khó khăn trong việc đánh dấu lợi nhuận do sự gia tăng các vụ vỡ nợ
trong danh mục cho vay mua xe. Mục tiêu của công ty là xác định khả năng trả nợ của
khách hàng và hiểu được tầm quan trọng tương đối của từng tham số góp phần vào khả
năng trả nợ của người vay.

Mục tiêu của bài toán là dự đoán liệu khách hàng có vỡ nợ khoản thanh toán khoản vay
mua xe hay không. Đối với mỗi ID trong bộ dữ liệu, bạn phải dự đoán mức “Default”.

## QUY TRÌNH LÀM VIỆC: 5 BƯỚC CHÍNH
- Tiền xử lý
  
  - Xử lý dữ liệu Missing
  
  - Xử lý dữ liệu Outliers
 
- Khai phá dữ liệu
  
  - Dùng Heatmap để thể hiện sự tương quan giữa từng feature với target
  
  - Dùng Parallel set plot và Scatter matrix để miêu tả chi tiết một vài mẫu tương quan cao theo Heatmap

- Chuẩn hóa và giảm chiều dữ liệu

- Xây dựng mô hình dự báo

- Đánh giá và kết luận
## PHẦN TÔI PHỤ TRÁCH:
- Tiền xử lý (Phụ trách chính)
  
  - Xử lý dữ liệu Missing

    - Thuộc tính có 2 giá trị
    ![image](https://user-images.githubusercontent.com/128765957/227457886-9069fc81-747b-4e09-9054-563223620707.png)

    - Thuộc tính có dữ liệu kiểu số
    ![image](https://user-images.githubusercontent.com/128765957/227458111-9106922e-750b-45a2-bee6-e2f3cad6739f.png)

    - Thuộc tính có dữ liệu kiểu chữ
    ![image](https://user-images.githubusercontent.com/128765957/227458351-3efac4db-5ecf-4bad-9dda-4031f342bdf2.png)

  
  - Xử lý dữ liệu Outliers

    - Thuộc tính có phân phối chuẩn: Giới hạn 3xSigma
    ![image](https://user-images.githubusercontent.com/128765957/227458587-abaa59f8-3344-4e3c-83d3-2c09562f3816.png)

    - Thuộc tính không có phân phối chuẩn: Giới hạn 1.5xIQR
    ![image](https://user-images.githubusercontent.com/128765957/227458949-bdc58787-87bf-42e6-9f78-f9652a157bc9.png)

 
- Khai phá dữ liệu (Hỗ trợ kiểm tra mối tương quan giữa các feature với target)
  
  - Dùng Heatmap để thể hiện sự tương quan giữa từng feature với target
  ![image](https://user-images.githubusercontent.com/128765957/227459062-d57f216f-f464-493f-a0ec-cd8a07e66b54.png)

  - Dùng Parallel set plot để miêu tả chi tiết một vài mẫu tương quan cao theo Heatmap
  ![image](https://user-images.githubusercontent.com/128765957/227459309-f2ae2a04-fda9-4766-b751-57bb325dc967.png)

  - Dùng Scatter matrix để miêu tả chi tiết một vài mẫu tương quan cao theo Heatmap
  ![image](https://user-images.githubusercontent.com/128765957/227459436-2ad6788a-e862-45ee-bebc-35bc71a92ea2.png)


