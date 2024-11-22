# sing-box
tun 模式的配置文件



```json
####vless-xtls-rprx-vision 协议配置
{
  "tag": "{all}",
  "type": "vless",
  "server": "IP地址",
  "server_port": 42114,
  "uuid": "xxxxxx",
  "packet_encoding": "xudp",
  "flow": "xtls-rprx-vision",
  "tls": {
    "enabled": true,
    "insecure": false,
    "server_name": "ip或域名",
    "reality": {
      "enabled": true,
      "public_key": "qhTzYYIgBzDLKfqrOliCY"
    },
    "utls": {
      "enabled": true,
      "fingerprint": "chrome"
    }
  }
}

---
#### Hysteria2 配置
```json
{
  "tag": "e73cad83-singbox_hysteria2",
  "type": "hysteria2",
  "server": "IP地址或者域名",
  "server_port": 端口,
  "up_mbps": 50,
  "down_mbps": 200,
  "password": "e73cad83-e754-",
  "tls": {
    "enabled": true,
    "server_name": "可以是www.bing.com",
    "alpn": [
      "h3"
    ]
  }
}

VLESS Reality gRPC 配置

{
  "tag": "e73cad83-VLESS_Reality_gPRC",
  "type": "vless",
  "server": "域名或ip",
  "server_port": 888,
  "uuid": "e73c9-fa5c628319e7",
  "tls": {
    "enabled": true,
    "server_name": "域名或ip",
    "utls": {
      "enabled": true,
      "fingerprint": "chrome"
    },
    "reality": {
      "enabled": true,
      "public_key": "vBQBcoL1v7xfI_TnA",
      "short_id": "6ba8fc2"
    }
  },
  "packet_encoding": "xudp",
  "transport": {
    "type": "grpc",
    "service_name": "grpc"
  }
}



TUIC 配置
{
  "tag": "e73cad83-singbox_tuic",
  "type": "tuic",
  "server": "ip或域名",
  "server_port": 1111,
  "uuid": "e73ca628319e7",
  "password": "e73cad83c628319e7",
  "congestion_control": "cubic",
  "tls": {
    "enabled": true,
    "server_name": "ip或域名",
    "alpn": [
      "h3"
    ]
  }
}







    
