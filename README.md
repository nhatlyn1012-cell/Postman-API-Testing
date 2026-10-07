
# Postman API Testing

## Thông tin sinh viên

* **Họ và tên:** Nguyễn Thị Nhật Linh
* **MSSV:** 23010511
* **Ngành:** Công nghệ thông tin

## 1. Mục tiêu

Thực hành kiểm thử API bằng Postman với các phương thức GET, POST, PUT, DELETE, sử dụng Parameters, Variables và Test Script.

## 2. Công cụ

* Postman
* GitHub

## 3. Nội dung thực hiện
### Overview

### GET

```text
GET https://postman-echo.com/get
```

### GET Params

```text
GET https://postman-echo.com/get
```

Parameters:

```text
name=Linh
studentId=23010511
```


### POST

```text
POST https://postman-echo.com/post
```

```json
{
    "name": "Nguyen Thi Nhat Linh",
    "studentId": "23010511",
    "major": "Information Technology"
}
```


### PUT

```text
PUT https://postman-echo.com/put
```



### DELETE

```text
DELETE https://postman-echo.com/delete
```


### Test

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response is JSON", function () {
    pm.response.to.be.json;
});
```


### Weather API

```text
GET https://api.open-meteo.com/v1/forecast
```

Parameters:

```text
latitude=21.0285
longitude=105.8542
current=temperature_2m,relative_humidity_2m,weather_code
```


## 4. Kết quả

| Nội dung    | Kết quả |
| ----------- | ------- |
| GET         | Passed  |
| GET Params  | Passed  |
| POST        | Passed  |
| PUT         | Passed  |
| DELETE      | Passed  |
| Test        | Passed  |
| Weather API | Passed  |

