# SeeComic
Windows下看漫画的工具软件， 部分功能兼容MangaMeeya; 也可作为图片浏览器.

### 支持
- Win7/Win10 64位

### 特性
  - 漫画浏览模式: 空格跳到图片的下一个浏览区域, 上下左右移动图片位置, PageDown/Up翻页, Ctrl+End跳到尾页
  - 窗口适应: 宽高(HOME)，满屏(End)， 原始(Ins), 自定义分辨率(F12); 全屏幕(Enter),还原(Esc)
  - 智能开页: 根据文件名判断开页方向
  - 目录连续浏览: 跳到下一个兄弟目录， 但不会跳到上一层目录
  - 支持7z,rar/rar5, zip, cbz, cbr压缩格式: 文件浏览器右键打开; 内嵌压缩文件暂时不支持.
  - 64位: 支持大图，不会出现Win32里内存不足的提示
  - gif/webp动图播放: 连续翻页时只会显示gif的前面几帧
  - 幻灯播放: 点击右下角工具条的播放按钮(F5), 使用快捷键'[',']'来变更幻灯播放的时间间隔
  - unicode支持: 可以读取带有特殊字符的文件
  - 目录或压缩文件右键打开: 跳到下一个目录是基于文件浏览器排序
  - 功能基本兼容MangaMeeya, 鼠标左键下一页，右键上一页
  - 压缩文件删除子文件: 按快捷键(Ctrl+Del)删除当前显示的压缩文件中的子文件， 在该压缩文件关闭时（或程序关闭时)生效; 需要在config.ini中设置本地的压缩软件路径.
  - 支持压缩文件密码: 输入的密码保存到文本里， 下次可以优先使用密码列表解密. 嵌套压缩不支持, 文件列表加密的不支持.
  - waifu2x滤镜： 在内存中处理， 不破坏原图, 使用默认参数.
  - 本软件无恶意代码，不收集数据， 无任何互联网连接， 不查询升级， 升级自行到该发布页找新版本。
  - 本软件为免费软件, 不开源的原因有两个，一个是第三方依赖太多，编译较麻烦；第二个是用了一些之前公司开发的代码，不方便开源。

### 下载
  - ver2.4.121
  链接：https://pan.baidu.com/s/16vACifSIJZ7ecwLTfQ7ylQ
  提取码：bq0z

  - ver2.4.118
  链接：https://pan.baidu.com/s/1m6FwzVy_eFS1O2i5zfWrXA
  提取码：nd8b

### changelog
  - v2.4.121
    - 修复F5在全屏幕切换后失效的问题
    - 全屏幕下面板延迟几秒后消失
  - v2.4.120
    - 应网友的要求添加自定义分辨率, 指定一个分辨率打开图片.
  - v2.4.118
    - 因为waifu2x较慢, 默认程序开启时为不打开， 需要手动开启
    - 修复几处小bug
  - v2.4.115
    - 菜单打开waifu2x滤镜，需要GPU， 否则打开速度较慢；该滤镜能放大老的分辨率较低的图片； 默认不开启，只处理小于800*800的图片; 参数可在config.ini里调整. 来自 https://github.com/nihui/waifu2x-ncnn-vulkan.git
    - 右键菜单添加了快捷键`, 因此需要先删除再安装
  - v2.3.112
    - 全屏幕时， 鼠标移动到正下方出控制面板
  - v2.3.111
    - 修正加载zip偶尔卡死的问题
    - 右下角添加全屏幕按钮
    - 全屏幕时鼠标移动到右上角弹出关闭面板
  - v2.3.110
    - 把白背景替换成黑背景
  - v2.3.109
    - 可自定义滚屏的速度， 通过修改config.ini里的BrowserWheelStep字段
    - 默认调慢了一点滚屏速度
  - v2.3.108
    - 使用快捷键‘[’,']'来变更幻灯播放的时间间隔, 变更的幅度可以在config.ini中修改
  - v2.2.106
    - config.ini移动到系统AppData目录下，可通过菜单的“打开config.ini”进行编辑,重启后生效. 文档说明参考例子.
  - v2.2.105
    - 添加压缩文件密码支持
    - 修复一些bug
  - v2.1.103
    - 添加删除压缩文件子文件的功能
  - v2.0.101
    - 修正快速浏览时gif播几帧再跳过
  - v2.0.100
    - 修复快速翻页浏览下一目录时有时候直接跳过的bug
  - V2.0.92
    - 变更图像引擎为opencv
  - v1.2.91
	 - 重新添加压缩文件列表排序
  - v1.2.89
    - 优化7z,zip大文件加载
    - 关闭压缩文件列表加载后排序
    - 修复一些崩溃的bug
  - v1.1.87
    - 修复一些灰度图显示花屏的问题
    - 修复用文件打开按钮打开图片后显示空白的问题
  - v1.1.86
    - 解决rar大文件打开慢的问题
    - 解决一些bug

### 反馈
  - 意见或bug请发送 1764462457@qq.com 或者直接提Issues
  - 知乎(https://www.zhihu.com/question/21598701/answer/1337337854) 评论
  - 类似手机app的长竖图浏览方式； 把一个包里的图片合并成一幅长图再浏览.
  - ~~图片的放大缩小功能, 自定义一个分辨率.~~
  - 碰到崩溃可发送C:\Users\Administrator\AppData\Local\CrashDumps目录下的dmp文件给我, 记得带下版本号.
