# Cuộc thi Data Gotalent

## I. Thông tin nhóm:

- **Trường:** Trường Đại học Khoa học Tự nhiên- Đại học Quốc gia Thành phố Hồ Chí Minh
  
    Mã số sinh viên|Họ và tên|Số điện thoại
    -|-|-
    21127684|Kuo Young Sheng|0904098763 
    21127471|Nguyễn Hoàng Anh Tuấn|0913776073
    21127687|Phan Huy Đức Tài|0913003511
    21127605|Dương Gia Hân|0397774304
    21127351|Hồ Đinh Duy Lực|0877731725


## II. Thông tin dự án:
### 1. Bộ dữ liệu:
- Nội dung: Bộ dữ liệu ghi nhận thông tin về các khách hàng và lịch sử xem phim của các cụm rạp chiếu phim khắp thành phố Đà Nẵng.
- Nguồn: Bộ Data được cung cấp bởi Ban tổ chức cuộc thi Data Got Talent.

### 2. EDA
#### 22.1 Dữ liệu khách hàng:
| ID | Column | Non-Null Count | Dtype | Meaning |
|----|--------|----------------|-------|---------|
| 0  | customerid | 4479 non-null  | object | Mã khách hàng |
| 1  | DOB        | 4479 non-null  | int64  | Ngày sinh |
| 2  | gender     | 4479 non-null  | object | Giới tính |
| 3  | address    | 4478 non-null  | object | Địa chỉ |
| 4  | Website    | 3943 non-null  | object | Dữ liệu web |
| 5  | job        | 4479 non-null  | object | Công việc |
| 6  | industry   | 3357 non-null  | object | Lĩnh vực |

#### 2.2 Dữ liệu bán vé:

| ID | Column | Non-Null Count | Dtype | Meaning |
|----|--------|----------------|-------|---------|
| 0  | cashier | 35378 non-null | object | Nhân viên thu ngân |
| 1  | saledate | 35378 non-null | datetime64[ns] | Ngày bán |
| 2  | total | 35378 non-null | float64 | Tổng tiền |
| 3  | customerid | 35378 non-null | object | Mã khách hàng |
| 4  | slot | 35378 non-null | object | Suất chiếu |
| 5  | room | 35378 non-null | int64 | Phòng chiếu |
| 6  | film | 35378 non-null | object | Tên phim |
| 7  | slot type | 35378 non-null | object | Loại suất chiếu |
| 8  | ticket price | 35378 non-null | int64 | Giá vé |
| 9  | popcorn | 35378 non-null | object | Bỏng ngô |


#### 2.3 Dữ liệu Phim được chiếu
| ID | Column       | Non-Null Count | Dtype  | Meaning                                              |
|----|--------------|----------------|--------|------------------------------------------------------|
| 0  | show_id      | 60 non-null    | object | Mã định danh phim                   |
| 1  | title        | 60 non-null    | object | Tên bộ phim                                 |
| 2  | director     | 50 non-null    | object | Tên đạo diễn bộ phim                 |
| 3  | cast         | 54 non-null    | object | Các diễn viên tham gia chương trình         |
| 4  | country      | 53 non-null    | object | Các quốc gia tham gia sản xuất phim |
| 5  | release_year | 60 non-null    | int64  | Năm phát hành chương trình                  |
| 6  | rating       | 59 non-null    | object | The age rating of the show                           |
| 7  | duration     | 60 non-null    | object | Độ dài chương trình(phút) hoặc mùa        |
| 8  | listed_in    | 60 non-null    | object | Thể loại chương trình                  |
| 9  | description  | 60 non-null    | object | Giới thiệu chương trình                       |

#### 2.4 Dữ liệu phim được thu thập thêm:

| #   | Column       | Non-Null Count | Dtype  | Ý nghĩa                                             |
|----|--------------|----------------|--------|------------------------------------------------------|
| 0  | film         | 19 non-null    | object | Tên của bộ phim                                      |
| 1  | count        | 19 non-null    | int64  | Số lượng vé bán ra của bộ phim                        |
| 2  | cast         | 19 non-null    | object | Danh sách các diễn viên  trong bộ phim |
| 3  | country      | 19 non-null    | object | Quốc gia hoặc các quốc gia sản xuất bộ phim           |
| 4  | release_year | 19 non-null    | int64  | Năm phát hành của bộ phim                            |
| 5  | rating       | 19 non-null    | object | Đánh giá độ tuổi của bộ phim                         |
| 6  | duration     | 19 non-null    | object | Thời lượng của bộ phim theo phút            |
| 7  | listed_in    | 19 non-null    | object | Thể loại hoặc các thể loại của bộ phim                |
| 8  | description  | 19 non-null    | object | Tóm tắt cốt truyện của bộ phim                       |
| 9  | Link         | 19 non-null    | object | Đường dẫn đến trang web thu thập thông tin           |


- **Distribution**
    - Numeric Values
      
    <img src="Image/Numeric-values.png">

    - Categorical Values
      
    <img src="Image/Categorical-values.png">



### 3. Phân tích vấn đề và đề xuất giải pháp:
**a. Question 1:** 

**Benefits:** 

**How to answer this question:**

  
    <img src="Image/Age-Sex.png">


**&rarr; Answer the question:** 

  
<hr/>

**b. Question 2:** 
**Benefits:** 
**How to answer this question:**


