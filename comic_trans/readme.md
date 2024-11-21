comic_trans

![image](../pics/rpa_yandex.gif)<br>

翻译一个压缩包，翻译后生成一个新的改名压缩包。
通过selenium自动化提交到yandex进行翻译， 自动保存，无需人工干预, 无须gpu，由网站处理。

### 安装
网盘下载comic_trans.7z文件， 解压到seecomic\comic_trans<br>
测试版本， 只在开发机上跑过，不保证都能运行

### 运行
 - v2.8.172以上版本
 - yandex的语言自动侦测会被关闭， 因此要自己选择语言， 快捷键T弹出语言选择
 - 运行后弹出的cef窗体会自行隐藏, 执行完成后关闭
 - 完成后在同一目录会生成一个改名的包

### hosts
<pre>
77.88.55.77    yandex.com
178.154.131.217 yastatic.net
87.250.250.119 mc.yandex.com
</pre>