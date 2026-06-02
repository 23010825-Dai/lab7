# lab7
# BÁO CÁO THỰC HÀNH POSTMAN

## Thông tin sinh viên

* Họ và tên: Đỗ Hữu Đại
* MSSV: 23010825

## Mục tiêu

Tìm hiểu công cụ Postman và thực hành kiểm thử API bằng các phương thức GET, POST, PUT, DELETE.

## Công cụ sử dụng

* Postman
* GitHub
* JSONPlaceholder API

## Nội dung thực hiện

### 1. GET danh sách bài viết

API:

https://jsonplaceholder.typicode.com/posts

Kết quả:

![GET Posts](images/get_posts.png)

### 2. GET chi tiết bài viết

API:

https://jsonplaceholder.typicode.com/posts/1

Kết quả:

![GET Post By ID](images/get_post_by_id.png)

### 3. POST tạo bài viết mới

API:

https://jsonplaceholder.typicode.com/posts

Kết quả:

![POST Create](images/post_create.png)

### 4. PUT cập nhật bài viết

API:

https://jsonplaceholder.typicode.com/posts/1

Kết quả:

![PUT Update](images/put_update.png)

### 5. DELETE bài viết

API:

https://jsonplaceholder.typicode.com/posts/1

Kết quả:

![DELETE](images/delete_post.png)

### 6. Kiểm thử bằng Test Script

Script:

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response time less than 1000ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(1000);
});
```

Kết quả:

![Test Result](images/test_result.png)

## Nhận xét

* Hiểu được cách gửi request bằng Postman.
* Thực hành các phương thức GET, POST, PUT, DELETE.
* Biết cách viết test script cơ bản.
* Hiểu cấu trúc dữ liệu JSON trong API.

## Kết luận

Qua bài thực hành, em đã nắm được các thao tác cơ bản của Postman và có thể sử dụng công cụ này để kiểm thử API trong quá trình phát triển phần mềm.

