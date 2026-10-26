# Bài 2: Chuẩn bị hồ sơ dự án trước khi triển khai hệ thống

## 1. Giới thiệu

**Dự án:** PTIT-Learning  
**Chủ đề:** Chuẩn bị hồ sơ cho hệ thống học trực tuyến  
**Phiên bản:** 1.0  
**Ngày thực hiện:** 25/10/2026

Bài tập xây dựng bộ hồ sơ cho nền tảng PTIT-Learning, tập trung vào đặc tả yêu cầu phần mềm, quản lý dữ liệu bằng Excel và trình bày tính năng bằng PowerPoint.

## 2. Danh sách file hoàn thành

| STT | Tên file | Nội dung |
|---|---|---|
| 1 | `SRS_PTIT_Learning.docx` | Đặc tả yêu cầu phần mềm cho chức năng Lớp học ảo |
| 2 | `DanhSachKhoaHoc.xlsx` | Quản lý dữ liệu khóa học, sinh viên và lọc dữ liệu |
| 3 | `LoTrinhHocTap.pptx` | Giới thiệu tính năng Lớp học ảo và trình bày lộ trình học tập |

## 3. Phần 1: Phân tích cấu trúc Heading

File Word `SRS_PTIT_Learning.docx` được tổ chức bằng Heading Styles để tạo cấu trúc rõ ràng, hỗ trợ Navigation Pane và mục lục tự động.

### Sơ đồ cây Heading

- **Heading 1: 1. Giới thiệu**
  - Heading 2: 1.1. Mục đích
  - Heading 2: 1.2. Phạm vi
  - Heading 2: 1.3. Định nghĩa, viết tắt

- **Heading 1: 2. Mô tả tổng quan**
  - Heading 2: 2.1. Tổng quan hệ thống
  - Heading 2: 2.2. Vai trò người dùng

- **Heading 1: 3. Mô tả chức năng lớp học ảo**
  - Heading 2: 3.1. Tạo và quản lý lớp học ảo
  - Heading 2: 3.2. Tham gia lớp học
  - Heading 2: 3.3. Tính năng trong lớp học
  - Heading 2: 3.4. Ghi hình và lưu trữ
  - Heading 2: 3.5. Chat và hỏi đáp
  - Heading 2: 3.6. Chia sẻ tài liệu và bảng trắng
  - Heading 2: 3.7. Điểm danh và báo cáo tham gia

- **Heading 1: 4. Yêu cầu phi chức năng**
  - Heading 2: 4.1. Hiệu năng
  - Heading 2: 4.2. Bảo mật
  - Heading 2: 4.3. Khả dụng
  - Heading 2: 4.4. Khả năng mở rộng

- **Heading 1: 5. Ràng buộc và giả định**

- **Heading 1: 6. Phụ lục**

### Kết quả

- Sử dụng Heading 1 cho các mục chính và Heading 2 cho các mục nhỏ.
- Sử dụng Navigation Pane để kiểm tra cấu trúc tài liệu.
- Tạo mục lục tự động và cập nhật bằng chức năng Update entire table trước khi lưu.

## 4. Phần 2: Triển khai hồ sơ

### 4.1. File Word — SRS_PTIT_Learning.docx

Tài liệu đặc tả yêu cầu phần mềm cho module Học trực tuyến, tập trung vào chức năng Lớp học ảo.

Nội dung gồm:

- Giới thiệu mục đích và phạm vi hệ thống.
- Mô tả tổng quan và vai trò người dùng.
- Đặc tả chức năng tạo lớp học, tham gia lớp học, chat, chia sẻ tài liệu, ghi hình và điểm danh.
- Xác định các yêu cầu phi chức năng về hiệu năng, bảo mật, khả dụng và khả năng mở rộng.
- Trình bày các ràng buộc, giả định và tiêu chí kiểm thử.

### 4.2. File Excel — sd_filter.xlsx

File Excel dùng để quản lý dữ liệu khóa học và sinh viên theo cấu trúc bảng.

Nội dung thực hiện:

- Tổ chức dữ liệu với hàng tiêu đề duy nhất.
- Quản lý danh sách khóa học và thông tin sinh viên.
- Sử dụng AutoFilter bằng tổ hợp phím `Ctrl + Shift + L`.
- Lọc sinh viên thuộc khoa CNTT có điểm chuyên cần dưới 7.
- Chuẩn hóa dữ liệu văn bản để hỗ trợ tìm kiếm và lọc chính xác.

### 4.3. File PowerPoint — ptit_learning_tinh_nang.pptx

Slide giới thiệu chức năng Lớp học ảo của nền tảng PTIT-Learning.

Nội dung trình bày:

- Giới thiệu các tính năng chính của lớp học ảo.
- Mô tả lộ trình học tập gồm đăng nhập, chọn khóa học, tham gia lớp học và hoàn thành khóa học.
- Trình bày giá trị của hệ thống đối với sinh viên và giảng viên.

Thiết kế sử dụng nền Navy, chữ trắng và màu cam làm điểm nhấn, ưu tiên nội dung ngắn gọn, dễ đọc và có độ tương phản cao.

## 5. Phần 3: Kiểm thử và xử lý lỗi Excel

### Tình huống

Khi lọc sinh viên theo tên, Excel không hiển thị kết quả dù tên đó vẫn nhìn thấy trong bảng dữ liệu.

### Nguyên nhân

Dữ liệu có thể chứa khoảng trắng thừa ở đầu, cuối hoặc giữa các từ, khiến nội dung không khớp với từ khóa tìm kiếm.

### Cách xử lý bằng hàm TRIM

Giả sử họ tên sinh viên nằm trong ô B2.

Nhập công thức vào một cột phụ:

```excel
=TRIM(B2)
```

Các bước thực hiện:

1. Thêm cột mới có tên `Tên đã chuẩn hóa`.
2. Nhập công thức `=TRIM(B2)` tại dòng dữ liệu đầu tiên của cột mới.
3. Kéo công thức xuống các dòng còn lại.
4. Lọc hoặc tìm kiếm theo cột đã chuẩn hóa.
5. Kiểm tra lại kết quả trước khi sử dụng dữ liệu.

Hàm TRIM loại bỏ khoảng trắng đầu và cuối, đồng thời thu gọn các khoảng trắng thông thường liên tiếp giữa các từ thành một dấu cách.

### Kết quả mong đợi

Tên sinh viên được chuẩn hóa, giúp việc tìm kiếm và lọc dữ liệu chính xác hơn. Nếu vẫn không tìm thấy, cần kiểm tra thêm các ký tự khoảng trắng đặc biệt hoặc lỗi dữ liệu khác.

## 6. Kết luận

Bài tập hoàn thiện bộ hồ sơ dự án PTIT-Learning gồm tài liệu SRS trên Word, bảng quản lý dữ liệu trên Excel và slide trình bày trên PowerPoint.

Thông qua bài tập, người thực hiện vận dụng được Heading Styles, mục lục tự động, AutoFilter, hàm TRIM và nguyên tắc thiết kế slide có độ tương phản cao.


