# 快到碗里来-----炒鸡简单配置
#订阅链接在最下面填
dns:
  default-nameserver:
    - 114.114.115.115
    - 119.28.28.28
    - 223.6.6.6
    - system
  nameserver:
    - https://dns.alidns.com/dns-query
    - https://doh.pub/dns-query
proxy-groups:
  - name: 手动选择
    include-all: true
    type: select
    icon: https://fastly.jsdelivr.net/gh/Koolson/Qure/IconSet/mini/Proxy.png
    proxies:
      - url-test
      - DIRECT
  - name: url-test
    include-all: true
    type: url-test
    url: 'http://www.gstatic.com/generate_204'
    interval: 3600
ruls:
  GEOIP,CN,DIRECT
  MATCH,手动选择
proxy-providers:
 链接:
    interval: 3600
    #URL后面填你的节点链接，记得加空格
    url: https://paste.gg/p/anpengxin9@gmail.com/a9290e191148446e924107ca36a717a2/files/9dc9f14bd71045299d97e128aec66466/raw
# 如果有特殊需求的话可以私信我我再添加相关规则
