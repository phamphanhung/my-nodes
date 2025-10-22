lệnh mới trên mac tắt nexus đi rồi chạy 
```
RAYON_NUM_THREADS=3 ~/.nexus/bin/nexus-network start --max-threads 3
```
```
RAYON_NUM_THREADS=10 ~/.nexus/bin/nexus-network start --max-threads 10
```
trên win
```
export RAYON_NUM_THREADS=24
export THREADS=24
alias nexus-start='~/.nexus/bin/nexus-network start --max-threads 24'
```

# Cài đặt Nexus Node (Ubuntu 24.04)

## 1. Cập nhật hệ thống & cài Docker

```bash
sudo apt update && sudo apt upgrade -y
sudo apt update
sudo apt install -y build-essential cmake protobuf-compiler libprotobuf-dev curl
curl https://cli.nexus.xyz/ | sh
source ~/.bashrc
nexus-network register-user --wallet-address <your-wallet-address>
nexus-network register-node
nexus-network start
```
### **Tài liệu liên quan**
- https://cli.nexus.xyz
- 

# 
```bash
curl https://cli.nexus.xyz/ | sh
source /Users/admin/.zshrc
nexus-network register-user --wallet-address 0xc16dC1E4c107a1B1D4AD7F87ED8fc5b1BA84F832
nexus-network register-node
nexus-network start
```

```bash
curl https://cli.nexus.xyz/ | sh
source /Users/admin/.zshrc
nexus-network register-user --wallet-address 0xD67C8522794C2ce32a043771f08CB9bd5b29151e
nexus-network register-node
nexus-network start
```
