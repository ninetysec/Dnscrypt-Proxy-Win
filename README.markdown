Dnscrypt-Proxy-Win

[官方下载地址(国内访问被墙)](http://download.dnscrypt.org/dnscrypt-proxy/)

[win版文档](https://github.com/jedisct1/dnscrypt-proxy/blob/master/README-WINDOWS.markdown)

[linux版文档](https://github.com/jedisct1/dnscrypt-proxy/blob/master/README.markdown)

==================

配置方法：

0x01  1.vbs为启动文件，将文件放入启动项可开机启动，需要可编辑替换resolvers-name

0x02  cmd下启动命令为：dnscrypt-proxy -R <resolvers-name>   // 例如：dnscrypt-proxy -R opendns

0x03  除了opendns跟opennic-jp-ns2，其他dns在国内延迟都很大，一般不采用，而日本的dns虽然低，但解析有限，例如网易云音乐等网站，会造成解析不了，需等几分钟后，它向上级DNS查询才可访问成功。遂此处推荐opendns。其他dns-name与其详细信息，可查看bin/dnscrypt-resolvers.csv文件。

0x04  安装Dnscrpyt服务命令，虽然可以成功安装，但不知为何无法启动，如有人知道，求指出。

  $dnscrypt-proxy -R opennic-jp-ns2 --install    //這是安裝命令

  $dnscrypt-proxy  --uninstall      //這是卸載命令
