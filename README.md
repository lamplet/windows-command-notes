# windows-command-notes

## 端口转发
与iptables不同，这里listen地址必须是本机存在的地址。可以配置一个虚拟的IP，掩码255.255.255.255，这样就可以解决IP不存在的问题。  
netsh interface portproxy add v4tov4 listenaddress=1.1.1.1 listenport=7000 connectaddress=2.2.2.2
