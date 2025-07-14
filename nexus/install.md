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

