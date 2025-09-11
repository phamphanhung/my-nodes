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
```bash
w32tm /resync
net start w32time
w32tm /resync
```
Open cmd prompt with open as an administrator 
Paste this 
```bash
wsl --shutdown
```
### cập nhật lần 3
cách 3 khi máy bị đứng 

pip install reasoning-gym

cd ~/rl-swarm

docker-compose run --rm --build -Pit swarm-gpu

python3 -m venv .venv
source .venv/bin/activate
./run_rl_swarm.sh
chạy 3 lệnh đầu mà bị lỗi down nữa
thì chạy tiếp lệnh cuối
### web check : https://dashboard.gensyn.ai/
### https://discord.gg/gensyn
###cập nhật lần 4 
nâng cấp Cuda 12.8

sudo apt-get --purge remove

sudo apt-get autoremove


wget https://developer.download.nvidia.com/compute/cuda/repos/wsl-ubuntu/x86_64/cuda-wsl-ubuntu.pin
sudo mv cuda-wsl-ubuntu.pin /etc/apt/preferences.d/cuda-repository-pin-600

sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/wsl-ubuntu/x86_64/3bf863cc.pub

sudo add-apt-repository "deb https://developer.download.nvidia.com/compute/cuda/repos/wsl-ubuntu/x86_64/ /"

sudo apt update
sudo apt install -y cuda-toolkit-12-8


export PATH=/usr/local/cuda-12.8/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-12.8/lib64:$LD_LIBRARY_PATH

source ~/.bashrc


nvcc --version

Kết quả: Cuda compilation tools, release 12.8, V12.8.89
xong chạy lại cái lệnh như bình thường
khi nó hỏi đến Hub Face (FC) thì N enter



genssyn4


1. cd ~/rl-swarm

2. từng lệnh

git fetch --tags


git checkout tags/v0.5.8 -b v0.5.8


git clone --branch v0.5.8 https://github.com/gensyn-ai/rl-swarm.git
cd rl-swarm
pip install -r requirements.txt


3, check xem lên v0.58 chưa 

cd ~/rl-swarm
 git describe --tags


4. 1 lệnh

cd ~/rl-swarm
docker-compose run --rm --build -Pit swarm-gpu


nếu lỗi ctrl + C và gõ 1 lệnh

python3 -m venv .venv
source .venv/bin/activate
./run_rl_swarm.sh

lỗi tiếp gõ 1 lệnh tiếp theo


cd ~/rl-swarm
source .venv/bin/activate
./run_rl_swarm.sh
xong dán model này vào
Gensyn/Qwen2.5-1.5B-Instruct
enter cho chạy xem bị văng k
chạy 6.0 mở thư
davidhung@DESKTOP-A39CHVD:~$ cd /mnt/c/Users/phamh/Downloads/rl-swarm-0.6.0
davidhung@DESKTOP-A39CHVD:/mnt/c/Users/phamh/Downloads/rl-swarm-0.6.0$ chmod +x run_rl_swarm.sh
davidhung@DESKTOP-A39CHVD:/mnt/c/Users/phamh/Downloads/rl-swarm-0.6.0$ ./run_rl_swarm.sh
