# Gender_classifycation_by_faces

Link raw data và clean data: [Google Drive](https://drive.google.com/drive/folders/1foRSOjX99adr49aVeS1a1RmeykPUsIfI?usp=sharing) 
## 1. Craw Data
- Thu thập dữ liệu ảnh từ Freepik.
  - Import thư viện.
  - Tìm nguồn dữ liệu ảnh.
  - Tìm các thẻ chứa đường dẫn liên kết ảnh.
  - Phân tích cấu trúc của trang dữ liệu.
  - Lấy các ảnh với các nhãn khác nhau:
    - Sử dụng thư viện request, lấy nội dung của trang.
    - Sử dụng thư viện crawl dữ liệu theo cấu trúc đã phân tích, lấy các đường dẫn của ảnh.
    - Với mỗi nhãn, tạo một thư mục và lấy đường dẫn liên kết các ảnh thuộc nhãn đó.
    - Sử dụng thư viện os để lưu lại ảnh vào hệ thống.
  - Xuất ra một số ảnh kết quả đã được crawl.
## 2. EDA
- Với Small Dataset:
  - Xuất ra số lượng ảnh, sơ đồ thể hiện sự phân bố ảnh theo mỗi lớp.
  - Xuất ra các thông số như kích thước, chiều cao, chiều dài...
- Với Big Dataset:
  - Xuất ra số lượng ảnh, sơ đồ thể hiện sự phân bố ảnh theo mỗi lớp.
  - Xuất ra các thông số như kích thước, chiều cao, chiều dài...
## 3. Tiền xử lý
- Cắt lọc ảnh:
  - Nạp tập dữ liệu.
  - Sử dụng thư viện FaceBoxes để cắt lấy gương mặt.
  - Lưu lại ảnh.
- Xuất ra số lượng ảnh, sơ đồ thể hiện sự phân bố ảnh theo mỗi lớp.
- Xuất ra các thông số như kích thước, chiều cao, chiều dài...
## 4. HOG & SVM
- Phân loại trên Small Dataset
  - Import thư viện
  - Import Small Dataset
  - Trích xuất đặc trưng
  - Khởi tạo Model
  - Thực hiện huấn luyện
  - Đánh giá trên Test Dataset
  - Hiển thị một vài kết quả trực quan
- Phân loại trên Big Dataset
  - Import thư viện
  - Import Big Dataset
  - Trích xuất đặc trưng
  - Khởi tạo Model
  - Thực hiện huấn luyện
  - Đánh giá trên Test Dataset
  - Hiển thị một vài kết quả trực quan
## 5. Resnet18 & MLP
- Phân loại trên Small Dataset
  - Import thư viện
  - Import Small Dataset
  - Khởi tạo Model
  - Thực hiện huấn luyện
  - Đánh giá trên Test Dataset
  - Hiển thị một vài kết quả trực quan
- Phân loại trên Big Dataset
  - Import thư viện
