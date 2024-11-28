# Thành viên nhóm #
| STT | Họ và tên          | Mã số sinh viên |
|-----|--------------------|-----------------|
| 1   | Hứa Hồ Gia Huy      | 21522143        |
| 2   | Quách Minh Huy      | 21522164        |
| 3   | Nguyễn Hoàng Diệp Phi|21522453  |

# Trước khi chạy source cần cấu hình aws credentials : #

- Trên github vào repo -> settings -> secret variables -> Cung cấp aws access key, secret key và session key của tài khoản aws student, mỗi phiên làm việc trên aws academy chỉ có 5 giờ và sẽ phải cung cấp lại key mới sau mỗi phiên làm việc.
- terraform -> variables.tf : sửa aws access key, secret key và session key được cung cấp trên awsacademy
# Câu 1: #
- Sau khi cấu hình file aws.yml, Để test github action có hoạt động không, thực hiện git push rồi theo dõi quá trình deploy ở mục Actions
- Ví dụ :  ![image](https://github.com/user-attachments/assets/8c45963e-44c8-4e63-8bf5-d3bce1c2709f)


# Triển khai dùng cloudformation #
 - upload file yaml lên aws cloudformation -> add a tag Name -> Next triển khai
 - Có thể chỉnh sửa cloudformation file dùng cloudformation infrastructure composer
 - Sơ đồ cloudformation stack : 
   ![image](https://github.com/user-attachments/assets/2b3bdf82-e588-457e-8f71-34313599b07a)

# Testing

## Install
- GO Framework: [Download](https://go.dev/doc/install)
- Thêm gói Terraform trên GO: `go get github.com/gruntwork-io/terratest/modules/aws@v0.47.2`

## Usage
- Mở termninal trong thư mục test, run `go test -v`

## Kết quả
![Test](https://drive.google.com/thumbnail?id=1rhkWTQnex8tCd6K1uwuTCnQCeOxiMQWf)


