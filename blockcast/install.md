DePIN #Blockcast
Vào link ref chọn “Sin Up/đăng nhập/đăng ký” bằng tài khoản Google:
https://app.blockcast.network?referral-code=VodNum
- Mã CODE:
VodNum
- Đăng nhập được vào trang tổng quan thì chọn “MyProfile” để liên kết ví mạng Solana: Ví phantom hoặc ví Solflare..
VIDEO hướng dẫn chạy node Blockcast từ a đến z, nên khá dài:
### https://youtu.be/T-6RRBvJEwY
Tiếp theo là cách chạy node Blockcast bằng Docker:
### https://www.docker.com/
### https://github.com/Blockcast/beacon-docker-compose
Tải về, chạy file trên và kết hợp với 2 dòng lệnh bên dưới:
### cách mở cmd. sau khi tải về thư mục Block. bấm vào thư múc , bấm vào thanh đường dẫn tại đó bâm 'cmd'
Mở “cmd” để chạy lệnh:
```bash
docker compose up
```
Đợi lệnh trên chạy xong, mở thêm 1 cửa sổ “cmd” khác và chạy lệnh:
```bash
docker compose exec blockcastd blockcastd init
```
### sau lệnh này ra 1 đường link, bấm coppy qau trình duyệt để đăng ký node
----------------------------------
