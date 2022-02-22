comic_trans

支持漫画的图片翻译， 无需人工操作， 自动翻译生成一幅新的翻译后图片。当前版本只支持英文翻译中文。

[例子预览](https://github.com/nessessary/SeeComic/blob/master/comic_trans/sample.md)

1. 网盘下载(链接：https://pan.baidu.com/s/1HS7lxT0xNgW-6ELNijRhbA
提取码：n3wu), 可先下载翻译例子看一下效果, 确定接受当前软件达到的效果再继续， 因为是自动生成， 排版不完美(未来主要修正排版)，加上机翻，只是看个大概意思，较真的就别下了；不接受任何形式的退款行为。
2. 解压到seecomic目录下seecomic\comic_trans; 未安装seecomic可解压至任意目录
3. 调用gethardid.exe获取硬件id， 通过邮件(nessessary@qq.com)发送给作者
4. 缴费后，会返回一个reg.key的文件，放置到comic_trans根目录下即注册完成。注册后即无限使用.
5. 命令行下执行play.bat xxx(目录或压缩文件或图片文件, 压缩文件支持需要填写seecomic里的config.ini,设置路径), 第一次执行会自动下载几个大的模型文件，需要一段时间，等待即可。翻译一个30个图片左右的包，cpu需要几十分钟， gpu大约十分钟左右， 视硬件情况。
<br>命令行参数 ：<br> --double=0 1为生成后保留原图，在seecomic里双页打开，可比对原图<br> --para=0 如果文字都在一个块里选择1(比如没有图片全页都是文字的)， 如果是气泡对话多选0
<br>--img 输入的图片，目录，压缩包的路径<br>--multi 处理同一目录下的同名压缩文件，比如abc1.zip,abc2.zip, comic_trans.exe --img='abc1.zip' --multi=1
<br> --langfrom=en --langto=ch 暂时是固定的
6. 会在目标文件同一目录下生成一个改名的翻译后文件

现征集几名内测的小伙伴， 可免费获取注册文件， 需要按上面的步骤发邮件获取， 测试后帮助反馈bug， 比如无法运行, 或运行中碰到的bug; 能正常运行的话也请反馈。
