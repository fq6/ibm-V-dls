# ibm-V

| Secrets变量 | 形式 |
  | --------------------- | ----------- |
  | `IBM_CF_USERNAME`       | IBM Cloud 邮箱地址 |
  | `IBM_CF_PASSWORD` | IBM Cloud 邮箱密码 |
  | `IBM_CF_APP_NAME` | IBM Cloud 应用程序名 |
  | `V2_UUID` | 自定义UUID码 |
  | `V2_WS_PATH_VMESS` </br> `V2_WS_PATH_VLESS` | 协议选择一个，填入自定义PATH路径 |



# cf加速


打开和复制脚本

```
addEventListener(
"fetch",event => {
let url=new URL(event.request.url);
url.hostname="域名";
let request=new Request(url,event.request);
event. respondWith(
fetch(request)
)
}
)
```

