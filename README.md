# BTL1 - Biểu diễn ảnh màu, Lọc tín hiệu và Biến đổi hình học

Bài tập lớn môn **Xử lý ảnh số và thị giác máy tính (CO3057)** - Trường Đại học Bách Khoa, ĐHQG TP. HCM.

**Nhóm thực hiện (Nhóm BTL_10):**
* 2311359 - Trần Nguyễn Đức Hưng
* 2311041 - Huỳnh Huy Hoàng
* 2311064 - Nguyễn Trần Đức Hoàng
* 2312410 - Phan Đức Nhã

## Nội dung chính

Dự án bao gồm 3 phần chính, tập trung vào các kỹ thuật xử lý ảnh cơ bản trong thị giác máy tính, từ việc thao tác với không gian màu đến lọc tín hiệu và biến đổi hình thái ảnh.

### Phần 1: Biểu diễn ảnh màu
* Thao tác và chuyển đổi giữa các không gian màu (RGB, Grayscale,...).
* Tách, xử lý và ghép các kênh màu riêng biệt của ảnh.
* Đánh giá sự khác biệt khi xử lý trên từng không gian màu.

### Phần 2: Lọc tín hiệu (Miền không gian và Miền tần số)
Khảo sát các kỹ thuật lọc ảnh tuyến tính nhằm làm trơn ảnh, phát hiện biên và tăng cường chi tiết. Thực nghiệm trên cả ảnh màu và ảnh xám.
* **Low-pass (miền không gian):** Mean filter, Gaussian filter (khảo sát với các kích thước kernel và $\sigma$ khác nhau).
* **High-pass & Tăng cường chi tiết (miền không gian):** Laplacian (áp dụng trực tiếp và kết hợp Gaussian Blur), Sobel (phương X, Y và magnitude), Prewitt (phương X, Y và magnitude), Sharpening filter.

### Phần 3: Biến đổi hình học
* Áp dụng các phép biến đổi không gian cơ bản trên ảnh (có thể bao gồm phép tịnh tiến, xoay, co giãn, biến đổi Affine hoặc Perspective).
* Phân tích hệ quả của việc biến đổi tọa độ pixel đối với chất lượng ảnh đầu ra.

## Cấu trúc thư mục

* `Part1_img_representation.ipynb`: Notebook thực hiện phần tiền xử lý ảnh (chuyển xám, tách/ghép xử lý kênh màu) - phục vụ Phần 1.
* `Part2_img_filtering.ipynb`: Notebook chính chứa code hiện thực các bộ lọc low-pass/high-pass trong miền không gian và lọc miền tần số - phục vụ Phần 2.
* `Part3_img_transformation.ipynb`: Notebook của phần biến đổi các phép biến đổi không gian cơ bản trên ảnh- phục vụ Phần 2.


## Yêu cầu môi trường

* Python 3.x
* OpenCV (`cv2`)
* NumPy
* Jupyter Notebook (hoặc Google Colab)

**Cài đặt nhanh các thư viện cần thiết:**
```bash
pip install opencv-python numpy
```

## Cách chạy

1. Mở các file `.ipynb` bằng Jupyter Notebook hoặc Google Colab.
2. Chạy lần lượt các cell từ trên xuống dưới để load ảnh và xem các bước xử lý.
3. Kết quả (ảnh gốc so sánh với ảnh đã qua xử lý) sẽ được hiển thị trực tiếp ngay bên dưới mỗi cell.

## Link notebook trên Colab

## Google Colab Notebooks

- [Part 1 - Image Processing](https://colab.research.google.com/drive/1Broldky8wxZp-WWvKBn3WdC66PIw4uDz?usp=sharing)
- [Part 2 - Image Filtering](https://colab.research.google.com/drive/1bkk-TzNW7BoYiID0bTxl4d-aUgXxwRPV#scrollTo=rJtODoJ9Nmpk)
- [Part 3 - Image Transformation](https://colab.research.google.com/drive/1zHEzkXY3L8GOVyetaxUSzBdzM-7BFLxc?usp=sharing)