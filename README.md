# SeeComic
Windows下看漫画的工具软件， 主要操作兼容MangaMeeya, （ MM足够优秀， 不过有些特殊字符的文件打不开，gif不能连看，大图片内存不足的三大问题是作者重新开发的原因，如果您也碰到了上述问题， 欢迎试用）; 也可作为图片浏览器.

### 支持
- Win7/Win10 64位

### 特性
  - 漫画浏览模式: 空格/单击左键跳到图片的下一个浏览区域, 鼠标滚轮上下移动图片，方向键上下左右移动图片, PageDown/Up翻页, Ctrl+End跳到尾页, +/-放大缩小图片，按住左键拖拽图片
  - 窗口适应: 宽高(HOME)，满屏(End)， 原始(Ins), 自定义分辨率(F12); 全屏幕(Enter),还原(Esc)
  - 单双页显示: 双页时不显示gif
  - 智能开页: 根据文件名判断开页方向
  - 目录连续浏览: 跳到下一个兄弟目录， 但不会跳到上一层目录
  - 支持7z,rar/rar5, zip, cbz, cbr压缩格式: 文件浏览器右键打开; 内嵌压缩文件暂时不支持. 现在对于7z的策略是一次性加载到内存， 因此对于大的7z会比较慢.
  - 压缩文件打开后会根据文件列表排序, 主要是基于数字排序
  - 64位: 支持大图，不会出现Win32里内存不足的提示
  - gif/webp动图播放: 连续翻页时只会显示gif的前面几帧
  - 幻灯播放: 点击右下角工具条的播放按钮(F5), 使用快捷键'[',']'来变更幻灯播放的时间间隔
  - unicode支持: 可以读取带有特殊字符的文件
  - 目录或压缩文件右键菜单打开: 跳到下一个目录是基于文件浏览器排序; 如果有everything先按everything的顺序，其次是文件浏览器，最后是字母排序。
  - 操作基本兼容MangaMeeya, 鼠标左键下一页，右键上一页
  - 压缩文件删除子文件: 按快捷键(Ctrl+Del)删除当前显示的压缩文件中的子文件， 在该压缩文件关闭时（或程序关闭时)生效; 需要在config.ini中设置本地的压缩软件路径.
  - 支持压缩文件密码: 输入的密码保存到文本里， 下次可以优先使用密码列表解密. 嵌套压缩不支持, 文件列表加密的不支持.
  - waifu2x滤镜： (W)在内存中处理， 不破坏原图, 使用默认参数; 需要gpu支持(只在rtx显卡上测试过)，加载较慢.
  - [漫画图片翻译](comic_trans/readme.md)： (T)生成一本新的翻译后压缩包, 在一个命令行(需要单独下载)中生成， 生成后自动打开;
  - 本软件无恶意代码，不收集数据， 无任何互联网连接， 不查询升级， 升级自行到该发布页找新版本。
  - 如果觉得有帮助可捐赠支持， 不捐赠也是永久免费的.
  - 一些小功能请自行查阅changelog

### 下载
  - 该软件不是MangaMeeya的完全替代， 请仔细看特性再下载，没有的都是不支持的.
  - [下载](down.md)
  
### changelog
  - v2.7.155 2023/8/4
    - 修正双页不能跳到上一目录的bug
  - v2.7.154 2023/7/24
    - 添加翻译对话框， 可选语言及翻译引擎; 详见[漫画图片翻译](comic_trans/readme.md)
    - 命令行翻译支持多语言
  - v2.6.152 2023/7/10
    -  解决幻灯播放时下面板不隐藏的问题
    -  支持压缩包内子文件打印
    -  菜单添加“打开文件夹"
  - v2.6.149 2023/3/1
    - 右键菜单打开的压缩包恢复到上一次关闭的页面
  - v2.6.147 2022/12/2
    - 翻译改为免费试用版本, 需要自行网盘下载后解压至固定目录
  - v2.6.146 2022/9/14
    - 解决偶尔gif加载卡死的问题
  - v2.6.145 2022/8/12
    - 全屏幕右上角面板添加最小化
    - 幻灯播放只在最小化时暂停
  - v2.6.144 2022/6/20
    - 空格长按松开不继续跳到下一页
    - 幻灯播放时， 界面失去焦点后， 播放暂停， 待重新拥有焦点后再继续
  - v2.6.143 2022/2/26
    - 滑动条改为鼠标松开时触发
  - v2.6.141 2022/2/22
    - 图片翻译支持rtx_gpu本地运行， 配合菜单直接调用， 暂时只处理压缩包
  - v2.6.140
    - 预加载当前打开文件的后一个压缩包
    - 修复waifu2x当前图不刷新的问题， 因为waifu执行较慢， 默认完成后在图像左上角加上一个‘W’标识， 可以在config中关闭.
  - v2.6.139
    - 多国语言
  - v2.6.138 2022/2/2
    - 目录文件列表排序，修复下一目录浏览器排序支持
    - 修复单帧webp占用cpu问题
  - v2.6.136 2021/12/14
    - 放大缩小在所有模式下都生效， 不修改全局设置
  - v2.6.134 2021/11/30
    - 添加everything窗体的目录排序支持; 在everything搜索某关键字的压缩包， 下一目录会按该排序跳转
  - v2.6.132 2021/11/20
    - 优化7z加载,7z不支持文件列表排序， 按顺序加载
    - Ctrl+pagedown/up 直接跳到下一目录
    - 按住鼠标左键可直接拖拽移动图片
  - v2.5.131 2021/11/13
    - 完善自定义分辨率对话框，锁定宽高，快捷键+，-放大缩小图片
    - 菜单添加翻译， 功能由“漫画图片翻译”命令行提供
  - v2.5.128 2021/9/21
    - 解决某些机器写不上config.ini的问题, 修正文件列表数字排序
  - v2.5.126
    - bug 修正文件列表数字排序
  - v2.5.124
    - 一些小调整
  - v2.5.123
    - 添加双页显示, 双页时会跳过gif，webp
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
