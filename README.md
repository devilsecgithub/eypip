# pyton恶意库排查
客户现场需要对态势感知监测到的恶意python库进行排查

写了一个排查的小玩意

需要自取

# 使用方法
一、将要排查的恶意包名和版本号写进rootkit_pip.txt文件中，以 包名==版本号 的形式分隔开来，例如：

ipaddress==1.0.23

Naked==0.1.31

oauthlib==3.1.0

备注：如果它与要求的版本号匹配，则将包名和版本号写入到文件和控制台中。如果版本号不匹配，则将仅写入包名并指出版本号不匹配。

二、启动py脚本，使用python3启动

```
python3 eypipscan.py
```

三、等待扫描结果

排查到已安装的恶意pip三方包已写入installed_rootkit_pip.txt文件
