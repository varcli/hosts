# hosts  

## Note  
每日自动更新 github, docker 等常用 的 IP 地址。  

hosts Url:   
Raw Url: ``` https://raw.githubusercontent.com/varcli/hosts/main/hosts ```  
CDN Url: ``` https://cdn.staticaly.com/gh/varcli/hosts/main/hosts ``` 

## Used  
Windows/MacOS:  
```
推荐使用 SwitchHosts
```

Linux:
```
# 删除
sudo sed -i '/# Varcli Hosts Start/,/# Varcli Hosts End/d' /etc/hosts
# 添加
curl -s -L https://raw.githubusercontent.com/varcli/hosts/main/hosts | sudo tee -a /etc/hosts
```