comic_trans

![image](../pics/rpa_yandex.gif)<br>

翻译一个压缩包，翻译后生成一个新的改名压缩包。
通过selenium自动化提交到yandex进行翻译， 自动保存，无需人工干预, 无须gpu，由网站处理。

### 安装
网盘下载comic_trans.7z文件， 解压到seecomic\comic_trans<br>
测试版本， 只在开发机上跑过，不保证都能运行

### 运行
1. 配置config.ini里的压缩软件路径; 如果comictrans_engine=google改为comictrans_engine=baidu
2. 需要修改seecomic的默认安装路径， 安装到没有空格的目录， 比如c:\soft\seecomic
3. yandex的语言自动侦测会被关闭， 因此要自己选择语言， 快捷键T弹出语言选择
4. 运行后弹出的cef窗体会自行隐藏, 执行完成后关闭
5. 完成后在同一目录会生成一个改名的包
