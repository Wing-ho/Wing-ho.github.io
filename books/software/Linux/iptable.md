iptables -t nat -A PREROUTING -s 192.168.1.3 -p tcp -m multiport --dport 80,8080 -j DNAT --to 192.168.1.10:80

iptables -t nat -A PREROUTING -s 192.168.1.5 -p tcp -m multiport --dport 80,8080 -j DNAT --to 192.168.1.10:80

iptables -t nat -D PREROUTING 7

[iptables的限速测试总结 ](http://blog.51cto.com/ptallrights/1841911)
[iptables中限速的limit,limit-burst功能研究](http://blog.sina.com.cn/s/blog_6e5e78bf0101tuq9.html)
