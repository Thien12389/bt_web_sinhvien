\# Bài tập Lập trình Web - K59KMT



\## Yêu cầu

\- Cài đặt môi trường Linux (WSL Ubuntu) và Docker Compose

\- Triển khai 5 dịch vụ: Nginx, Node-RED, MariaDB, phpMyAdmin, Cloudflared

\- Cấu hình Nginx phục vụ 2 domain riêng biệt: lab1 và lab2

\- Xây dựng API trên Node-RED, cấu hình proxy qua Nginx

\- Viết JavaScript gọi API và hiển thị dữ liệu trên trang HTML

\- Public ra internet bằng Cloudflare Tunnel với domain thật



\## Deadline

(Deadline: 30/09/2026 23:59)



\## Sinh Viên:

Lê Đỗ Hoàng Thiện



\## Kết quả dự kiến

\- `https://lab1.chiyeuminhem.id.vn` và `https://lab2.chiyeuminhem.id.vn` chạy được

\- API `/api/tacke` trên Node-RED trả về đúng dữ liệu JSON

\- Nginx proxy `/api/` hoạt động qua domain thật

\- Trang lab1 gọi API bằng JavaScript và hiển thị bảng dữ liệu



\---



\## Nhật ký thực hiện (7 commit)



\### 1. `docs: khoi tao repo, xac nhan da cai WSL Ubuntu`

Khởi tạo repo, xác nhận đã cài WSL Ubuntu.



\### 2. `chore: da cai dat Docker + Docker Compose`

Cài đặt Docker và Docker Compose trên WSL Ubuntu.



\### 3. `feat: tao cau truc thu muc va docker-compose.yml cho 5 dich vu`

Tạo cấu trúc thư mục và file `docker-compose.yml` khai báo 5 dịch vụ: nginx, nodered, mariadb, phpmyadmin, cloudflared.



\### 4. `feat: cau hinh nginx 2 domain lab1 va lab2, them anh minh chung`

Cấu hình Nginx phục vụ 2 domain riêng biệt qua Cloudflare Tunnel.

<img width="1920" height="1080" alt="Ảnh chụp màn hình 2026-09-27 153646" src="https://github.com/user-attachments/assets/fbd89e07-5b31-4716-95bd-590c9092143d" />

<img width="1920" height="1080" alt="Ảnh chụp màn hình 2026-09-27 154756" src="https://github.com/user-attachments/assets/39206130-def3-4311-aa7f-3e5f2e17d6ed" />



\### 5. `feat: tao API /api/tacke tren Node-RED, them anh minh chung`

Tạo API `/api/tacke` trên Node-RED (http in → function → http response).

<img width="1920" height="1080" alt="Ảnh chụp màn hình 2026-09-27 153701" src="https://github.com/user-attachments/assets/65fc836b-7c33-4fff-b7d5-a6bd23c9b187" />

<img width="1920" height="1080" alt="Ảnh chụp màn hình 2026-09-27 160005" src="https://github.com/user-attachments/assets/34ae98ac-d525-4e7b-9dc0-cf30e209abd8" />





\### 6. `feat: them proxy /api/ tren nginx lab1 toi nodered`

<img width="1917" height="541" alt="image" src="https://github.com/user-attachments/assets/20052a89-b7ea-412d-bd30-2833e7e2ae06" />





!\[Curl qua domain thật](images/lab1-api-proxy.png)



\### 7. `feat: hoan thanh JS goi API va hien thi du lieu, them anh minh chung`

Viết JavaScript trong trang HTML gọi API và hiển thị bảng dữ liệu.

<img width="1920" height="1080" alt="Ảnh chụp màn hình 2026-09-27 153646" src="https://github.com/user-attachments/assets/fbe4fec1-747a-4868-8725-1fcd8aff0725" />







