✅ BƯỚC 1: Cài đặt Node.js 20+
bash
Sao chép
Chỉnh sửa
```bash
sudo apt remove -y nodejs
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs
```
node -v  # ✅ Kiểm tra: cần ra v20.xx.x trở lên
✅ BƯỚC 2: Cài Python virtualenv (chỉ chạy 1 lần duy nhất)
bash
Sao chép
Chỉnh sửa
```bash
sudo apt update
sudo apt install -y python3-venv python3-pip
```
✅ BƯỚC 3: Clone source code từ GitHub
bash
Sao chép
Chỉnh sửa
```bash
cd ~
git clone https://github.com/gensyn-ai/rl-swarm.git
cd rl-swarm
```
✅ BƯỚC 4: Tạo và kích hoạt môi trường ảo Python
bash
Sao chép
Chỉnh sửa
```bash
python3 -m venv .venv
```
# ✅ Tạo virtual environment
```bash
source .venv/bin/activate
```
# ✅ Kích hoạt môi trường ảo
⚠️ Mỗi lần chạy lại sau này, luôn phải chạy lại source .venv/bin/activate trước khi chạy script.

✅ BƯỚC 5: Cấp quyền thực thi và đăng nhập Modal
bash
Sao chép
Chỉnh sửa
```bash
chmod +x modal-login
```
```bash
./modal-login
```
🔑 Bước này sẽ mở trình duyệt tại http://localhost:3000 để bạn login và lấy API KEY, sau đó sẽ tự sinh ra file userData.json.
### **BƯỚC NÀY NÓ LÊN Y?n THÌ BẤM N VÀ ENTER** 
✅ BƯỚC 6: Chạy RL-Swarm
bash
Sao chép
Chỉnh sửa
```bash
./run_rl_swarm.sh
```
✅ Nếu mọi thứ đúng, bạn sẽ thấy log giống như:
API key is activated! Proceeding... và tiến trình bắt đầu huấn luyện (training).
📌 GHI NHỚ:
Mỗi lần mở lại máy, bạn cần chạy:
bash
Sao chép
Chỉnh sửa
```bash
cd ~/rl-swarm
source .venv/bin/activate
./run_rl_swarm.sh
```
### **cập nhật khi bị lỗi dòng chữ đỏ**
Ok so 
Run your cmd as an administrator 
Then 
paste this
w32tm /resync
net start w32time
w32tm /resync
Open cmd prompt with open as an administrator 
Paste this 
wsl --shutdown
### web check : https://dashboard.gensyn.ai/
### https://discord.gg/gensyn
