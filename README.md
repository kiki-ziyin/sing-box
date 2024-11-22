# sing-box
tun 模式的配置文件

### vless-xtls-rprx-vision 协议配置

```json
{
  "tag": "{all}",
  "type": "协议类型",
  "server": "IP地址",
  "server_port": 42114,
  "uuid": "xxxxxx",
  "packet_encoding": "xudp",
  "flow": "xtls-rprx-vision",
  "tls": {
    "enabled": true,
    "insecure": false,
    "server_name": "swdist.apple.com",
    "reality": {
      "enabled": true,
      "public_key": "qhTzYYIgBzDLNYR79oxftqdo1kzL-1_hGJKfqrOliCY"
    },
    "utls": {
      "enabled": true,
      "fingerprint": "chrome"
    }
  }
}




    
