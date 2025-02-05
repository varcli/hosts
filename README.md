# hosts  

## 备注  

自动更新 github, docker 等常用 的 IP 地址。  

hosts Raw Url: ``` https://raw.githubusercontent.com/varcli/hosts/main/hosts ```  
hosts CDN Url: ``` https://cdn.staticaly.com/gh/varcli/hosts/main/hosts ``` 

> Linux / MacOS hosts路径：/etc/hosts
> 
> Windows hosts路径：C:\Windows\System32\drivers\etc\hosts

## 使用  

Windows:  
```
推荐使用 SwitchHosts

# 刷新生效
ipconfig /flushdns
```

MacOS:  
```
推荐使用 SwitchHosts

# 刷新生效
sudo killall -HUP mDNSResponder
```

Linux:
```
# 删除
sudo sed -i '/# Varcli Hosts Start/,/# Varcli Hosts End/d' /etc/hosts
# 添加
curl -s -L https://raw.githubusercontent.com/varcli/hosts/main/hosts | sudo tee -a /etc/hosts
# 刷新生效
/etc/init.d/network restart
```

## 其他

- [SwitchHosts](https://github.com/oldj/SwitchHosts)
- [shidahuilang/hosts](https://github.com/shidahuilang/hosts)
- [521xueweihan/GitHub520](https://github.com/521xueweihan/GitHub520)
- [Licoy/fetch-github-hosts](https://github.com/Licoy/fetch-github-hosts)
