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

### changelog
2024/3/25 v2.8.169.0
- [bug] 有些gif实际是webp格式， 修复该问题

2024/3/22
- [bug] 包内的gif加载(gdiplus)失败，造成卡死；目录下的无此问题。加上设置异常标识.


### 下载
  - 请慎重下载，该软件不是MangaMeeya的完全替代， 请仔细看特性再下载，没有的都是不支持的. 免费软件， 不喜勿喷！
  - 只在作者机器上测试通过， 不保证在用户机器上能正常运行， 有bug可提issues
  - <a href="https://pan.baidu.com/s/1Td2vJHmX-yahTPOfYMi2Kg?pwd=9bm1" target="_blank" style="
    -webkit-tap-highlight-color: rgba(18,18,18,0);
    appearance: none;
    font: inherit;
    outline: none;
    display: inline-block;
    font-size: 14px;
    line-height: 32px;
    padding: 0 16px;
    background: none;
    border: 1px solid;
    border-radius: 3px;
    cursor: pointer;
    text-align: center;
    border-color: #056de8;
    min-width: 96px;
    color: #fff;
    background-color: #056de8;
    margin: 0 8px;
">百度网盘</a>变更详见changelog文件
  

