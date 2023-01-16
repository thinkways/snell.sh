# Intro
适用于64位Linux系统。运行完毕后屏幕显示psk，默认端口号8080，按照标准填入Surge即可。

建议使用docker
```
https://github.com/primovist/snell-docker
https://hub.docker.com/repository/docker/primovist/snell-docker
```
# Install
## Debian & Ubuntu

```
wget --no-check-certificate -O snell.sh https://raw.githubusercontent.com/primovist/snell.sh/master/snell.sh
chmod +x snell.sh
./snell.sh
```

## Centos & RedHat

```
wget --no-check-certificate -O snell.sh https://raw.githubusercontent.com/primovist/snell.sh/master/snell.centos.sh
chmod +x snell.sh
./snell.sh
```

## Change service port
首次安装默认端口号8080，如需修改请在所有脚本运行结束后运行

```
nano /etc/snell/snell-server.conf
systemctl restart snell
```

## Check status
查看运行状态：

```
systemctl status snell
```

## 卸载方法

```
wget --no-check-certificate -O uninstall-snell.sh https://raw.githubusercontent.com/primovist/snell.sh/master/uninstall-snell.sh
chmod +x uninstall-snell.sh
./uninstall-snell.sh
```
