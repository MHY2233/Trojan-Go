# Trojan-Go

- **安装 Trojan-GO**
    
        wget https://github.com/p4gefau1t/trojan-go/releases/download/v0.10.6/trojan-go-linux-amd64.zip && unzip trojan-go-linux-amd64.zip -d ./trojan-go && mv trojan-go/trojan-go /usr/local/bin && chmod +x /usr/local/bin/trojan-go && rm -rf trojan-go  trojan-go-linux-amd64.zip
    
- **下载配置文件**
    
        mkdir /usr/local/etc/trojan-go/ && curl -Lo /usr/local/bin/trojan-go/config.json https://raw.githubusercontent.com/MHY2233/Trojan-Go/main/config.json
    
- **下载 service 文件**
    
        curl -Lo /etc/systemd/system/trojan-go.service https://raw.githubusercontent.com/MHY2233/Trojan-Go/main/trojan-go.service && systemctl daemon-reload
    
- **开启 Trojan-Go**
    
        systemctl enabel --now trojan-go
    
- **查看运行状态**
    
    systemctl status trojan-go
