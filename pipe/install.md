🔥Hướng Dẫn Chạy Node PoP PipeNetwork trên Windowns

✅Raised $10M
✅Backer: Multicoin, robot ventures, Solana Ventures
✅Cost: 0$ (Nếu thuê VPS 10$/tháng)

📱 Video HD: https://youtu.be/bwe1M6F2nDE

Bước 1️⃣: tải WSL về máy (Nếu thuê VPS hệ điều hành Ubuntu thì không cần làm bước này)
tìm kiếm Power Shell trên thanh tìm kiếm và run as admin
wsl --install
- tiếp theo: Mở Microsoft Store, tải Ubuntu 22.04 LTS và cài đặt.
mở Ubuntu lên cài đăng tài khoản mật khẩu

Bước 2️⃣: Cài đặt PoP Node Pipe network

curl -L -o pop "https://dl.pipecdn.app/v0.2.8/pop"
chmod +x pop
mkdir download_cache

Bước 3️⃣: Chạy Node

Đăng ký node:
sudo ./pop --signup-by-referral-route f2998c66d9a5feeb

Chạy node:

Chạy nhanh: 
sudo ./pop "Solana addrest"

chạy với setup:
sudo ./pop --ram 6 --max-disk 200 --cache-dir /data --pubKey "Solana addrest"
Ram tối thiểu là 4gb, disk là 100, nhưng mình để 6 và 200 chạy cho thoải mái, pubkey để địa chỉ ví 

4️⃣Chạy thì anh em treo 24/24 để nó lên uptime check points dùng câu lệnh:
./pop --points
Hoặc vào https://dashboard.pipenetwork.com/node-lookup dán Node ID để kiểm tra node chạy không

5️⃣  Mở thêm 1 tab ubuntu mới chạy lệnh
./pop --status
Chụp ảnh màn hình, vào discord: https://discord.gg/6Z22SKPR gửi kèm NodeID để lấy role
