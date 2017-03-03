# roadToFreeWorld
vpn settings

for l2tp

```BASH
wget --no-check-certificate https://raw.githubusercontent.com/teddysun/across/master/l2tp.sh

chmod +x l2tp.sh

./l2tp.sh

Please input IP-Range:
(Default Range: 192.168.18):
输入本地IP段范围（本地电脑连接到VPS后给分配的一个本地IP地址），直接回车意味着输入默认值192.168.18

Please input PSK:
(Default PSK: teddysun.com):
PSK意为预共享密钥，即指定一个密钥将来在连接时需要用到，直接回车意味着输入默认值teddysun.com

Please input Username:
(Default Username: teddysun):
Username意为用户名，即第一个默认用户。直接回车意味着输入默认值teddysun

Please input teddysun’s password:
(Default Password: Q4SKhu2EXQ):
输入用户的密码，默认会随机生成一个10位包含大小写字母和数字的密码，当然你也可以指定密码。

ServerIP:your_server_main_IP
显示你的 VPS 的主 IP（如果是多 IP 的 VPS 也只显示一个）

Server Local IP:192.168.18.1
显示你的 VPS 的本地 IP（默认即可）

Client Remote IP Range:192.168.18.2-192.168.18.254
显示 IP 段范围

PSK:teddysun.com
显示 PSK

Press any key to start…or Press Ctrl+c to cancel
按下任意按键继续，如果想取消安装，请按Ctrl+c键



------------------
l2tp -a 新增用户
l2tp -d 删除用户
l2tp -m 修改现有的用户的密码
l2tp -l 列出所有用户名和密码
l2tp -h 列出帮助信息

```

for shadowsocks

```bash
apt-get install python-pip
pip install shadowsocks

ssserver -c ./conf.json > /dev/null 2>&1 &
```
