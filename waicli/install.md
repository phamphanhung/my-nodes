chạy Wai qua CLI 

 curl -fsSL https://app.w.ai/install.sh | bash

 echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc

source ~/.bashrc

 which wai

thấy ra kết quả: /home/ubuntu24/.local/bin/wai

 wai --help

 wai login

nó tự nhảy lên chrome

kq
Signed in as 'johnyzhao.eth@gmail.com'

wai list-networks


Nếu ko dc chơi cách 2

Vào Dashbroard trên chrome
Vào API Key tạo key, copy và lưu kỹ lại

Vào ubuntu chạy:

echo 'export WAI_API_KEY="wsk-bQNl3oLaCJdalcXhP9pbswGDL1u1-1OOpEKJuu1bGv1tWDiVGobZJsKB3wZRl"' >> ~/.bashrc
source ~/.bashrc
 (thay APIKey vào giữa "")

dán và enter

tiếp

wai run 



Done/
