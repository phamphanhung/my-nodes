### swap sol sang wsol : https://tools.smithii.io/solana-wrapper/solana
### bài hướng dẫn chính : https://github.com/Joko588/Solana-Raydium-Sniper-Bot-2025/blob/main/README.md
hướng dẫn chạy trên mac book
### cài brew : BƯỚC 1: Cài Homebrew (bắt buộc)
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Trong Terminal, copy nguyên dòng này dán vào rồi Enter:
⏳ Chờ 3–10 phút (tuỳ mạng)

Trong quá trình cài:

Nó sẽ hỏi Enter → bấm Enter

Có thể hỏi password máy → nhập mật khẩu Mac (không hiện chữ là đúng)
### BƯỚC 2: Thêm Homebrew vào PATH (RẤT QUAN TRỌNG)

Sau khi cài xong, Homebrew sẽ in ra dòng hướng dẫn, thường là:
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```
### BƯỚC 3: Kiểm tra brew đã hoạt động chưa
```
brew --version
```

Nếu thấy kiểu:

Homebrew 4.x.x


👉 OK, đã xong phần khó nhất 🎉

### ✅ BƯỚC 4: Cài nvm
```
brew install nvm
````

Tạo thư mục nvm:

```
mkdir ~/.nvm
```

Thêm nvm vào shell:
```
echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.zshrc
echo '[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"' >> ~/.zshrc
source ~/.zshrc
```
### BƯỚC 5: Cài Node.js (chuẩn cho bot)
```
nvm install 18
nvm use 18
node -v
````


👉 Phải thấy:

v18.x.x

### ✅ BƯỚC 6: Quay lại chạy bot

```
cd ~/Solana-Raydium-Sniper-Bot-2025
npm install
```

### BƯỚC TIẾP THEO (CHẠY BOT)
1️⃣ Tạo file .env
```
cp .env.example .env
nano .env
````

👉 Dán cấu hình test an toàn:
file nano .env điền như sau, các thống số có thể thay đỏi tuỳ vào muốn lọc như nào 
 UW PICO 5.09                                              File: .env                                                
```env
PRIVATE_KEY=3u4LAaxxxxxxxxxx
RPC_ENDPOINT=https://mainnet.helius-rpc.com/?api-key=eba544b7-29a5xxx-xxxxx
RPC_WEBSOCKET_ENDPOINT=wss://mainnet.helius-rpc.com/?api-key=eba544b7xxxxxxxxxxx
QUOTE_MINT=WSOL
QUOTE_AMOUNT=0.01
COMMITMENT_LEVEL=processed
USE_SNIPE_LIST=false
SNIPE_LIST_REFRESH_INTERVAL=20000
CHECK_IF_MINT_IS_RENOUNCED=false
AUTO_SELL=true
MAX_SELL_RETRIES=5
AUTO_SELL_DELAY=10000
LOG_LEVEL=info
TAKE_PROFIT=30
STOP_LOSS=20
BIRDEYE_API_KEY=86fab0e57e7546cexxxxxxxxxx
MIN_POOL_SIZE=0.3
```
# hướng dẫn lẫy API key birdeye tại đây Tạo miễn phí tại đây: https://docs.birdeye.so/docs/authentication-api-keys
💡 Lúc test đừng để số lớn

2️⃣ Chạy bot

```
npm run start
```
### 📌 Giải thích nhanh
- QUOTE_AMOUNT: Số SOL mua mỗi lệnh
- TAKE_PROFIT: % chốt lời
- STOP_LOSS: % cắt lỗ
- MIN_POOL_SIZE: Thanh khoản tối thiểu (SOL)

Ví dụ:

### 🧪 Test lần đầu
Khuyến nghị:
- QUOTE_AMOUNT = 0.005 – 0.01 SOL
- Không test số lớn













