##lệnh này chạy viriffer

```bash
curl -L https://github.com/cysic-labs/cysic-phase3/releases/download/v1.0.0/setup_linux.sh > ~/setup_linux.sh && bash ~/setup_linux.sh "thay dòng này bằng ví của bạn"
cd ~/cysic-verifier/ && bash start.sh
```
##lệnh chạy prover cysic

```bash
curl -L https://github.com/cysic-labs/cysic-phase3/releases/download/v1.0.0/setup_prover.sh >
~/setup_prover.sh && bash
~/setup_prover.sh 0xe77b6cebd20B3693f958464627946A4C08caAF8d https://eth-mainnet.g.alchemy.com/v2/TuVRCujrYbgkUiBxHqajw
```
## ***thay ví của bạn vào chỗ 0xx và dán url eth mainet vào***
-- https://dashboard.alchemy.com/apps
## sau khi chạy xong chạy tiếp lệnh sau
```bash
cd ~/cysic-prover/ && bash start.sh
```
##tài liệu tham khảo
--https://x.com/PeterTran_CT/status/1942389331626451011
