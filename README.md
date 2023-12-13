# My-V2Ray-Config

【v2fly】https://github.com/v2fly/fhs-install-v2ray
//1. 安裝執行檔和 .dat 資料檔
bash <(curl -L https://raw.githubusercontent.com/v2fly/fhs-install-v2ray/master/install-release.sh)
//2. 启动服务
sudo systemctl enable v2ray
sudo systemctl start v2ray
//3. 编辑配置文件
vim /usr/local/etc/v2ray/config.json

【vless】https://github.com/kirin10000/Xray-script
//1. 安装wget && ca-certificates
apt --no-install-recommends -y install wget ca-certificates || (apt update && apt --no-install-recommends -y install wget ca-certificates)
//2. 获取/更新脚本
wget -O Xray-TLS+Web-setup.sh https://github.com/kirin10000/Xray-script/raw/main/Xray-TLS+Web-setup.sh
//3. 执行脚本
bash Xray-TLS+Web-setup.sh

【BBR】
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" chmod +x tcp.sh ./tcp.sh
sudo bash tcp.sh
