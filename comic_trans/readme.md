comic_trans

![image](../pics/rpa_yandex.gif)<br>

漫画的图片翻译，通过selenium自动化提交到yandex进行翻译， 自动保存，无需人工干预, 无须gpu，网站处理。

### 安装
网盘下载comic_trans.7z文件， 解压到seecomic\comic_trans<br>
测试版本， 只在开发机上跑过，不保证都能运行

### 运行
1. 配置config.ini里的压缩软件路径
2. 需要修改seecomic的默认安装路径， 安装到没有空格的目录， 比如c:\soft\seecomic
3. yandex的语言自动侦测会被关闭， 因此要自己选择语言， 快捷键T弹出语言选择
4. 运行后弹出的cef窗体不要关闭，也不用干预，退出时会自行关闭
5. 完成后会生成一个改名的包
