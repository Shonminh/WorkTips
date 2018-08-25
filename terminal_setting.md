### 在终端设置网络代理:
```
if [ `ps -ef|grep "lantern" -c` -gt 1 ];then
     export http_proxy="http_proxy=http://127.0.0.1:54386"
     export https_proxy="http_proxy=http://127.0.0.1:54386"
else
     export http_proxy=""
     export https_proxy=""
fi
```
### 设置Git代理(clone时推荐https形式):
```
git config --global https.proxy http://127.0.0.1:54386
git config --global http.proxy http://127.0.0.1:54386
```

### iterm2 使用时的帮助文档
[http://aaronmoment.cn/iterm2/](http://aaronmoment.cn/iterm2/)

item2常用快捷键总结

⌘ + number 切换标签页

⌘ + ←/→ 按方向切换标签页

⌘ + ⏎ 切换全屏

⌘ + f 查找

⌘ + d 垂直分屏，⌘ + shift + d 水平分屏。使用⌘ + ]和⌘ + [在最近使用的分屏直接切换.而⌘ + opt + ←/→切换到指定位置的分屏。

⌘ + t 新的标签页

⌘ + w 关闭当前标签页

⌘ + ; 自动补全历史命令。

⌃ + u 清空当前行。

⌃ + a 到行首

⌃ + e 行末

⌃ + f/b 前进后退，相当于左右方向键，原po说比移开手按方向键更快，我倒是觉得更加难按。

⌃ + d 删除当前字符

⌃ + h 删除之前的字符

⌃ + w 删除光标前的单词

⌃ + k 删除到文本末尾

之所以会去查iterm2的快捷键，是因为我觉得iterm2终端下单词间的移动非常低效。即我只可以通过⌃ + a/e控制到行首和行尾的移动，而不能按照单词移动。按照单词移动大概是用vim用的太顺手了吧。最终找到的解是ESC + b/f（b后退一个单词，f前进一个单词）。然而这未免太难按了吧！最终通过item2的Key bind解决了这个问题。将其映射为⌥ + ←/→。

如下图，打开profile，点选右边的Keys，点选左下的加号。

![image](https://user-images.githubusercontent.com/7269690/44620231-3967e780-a8c3-11e8-81c1-17c02c25be4f.png)


在弹出的对话框中，Action选择Send Escape Sequence。下图以回退为例，选择发送的组合为ESC + b，在最上面的框中输入偏好的快捷键。我设置成的是⌥ + ←。
