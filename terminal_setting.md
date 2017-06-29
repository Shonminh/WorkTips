###在终端设置网络代理:
```
if [ `ps -ef|grep "lantern" -c` -gt 1 ];then
     export http_proxy="http_proxy=http://127.0.0.1:54386"
     export https_proxy="http_proxy=http://127.0.0.1:54386"
else
     export http_proxy=""
     export https_proxy=""
fi
```
###设置Git代理(clone时推荐https形式):
```
git config --global https.proxy http://127.0.0.1:54386
git config --global http.proxy http://127.0.0.1:54386
```

