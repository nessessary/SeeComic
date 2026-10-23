# SeeComic
Windows下看漫画的工具软件， 主要操作兼容MangaMeeya, （ MM足够优秀， 不过有些特殊字符的文件打不开，gif不能连看，大图片内存不足的三大问题是作者重新开发的原因，如果您也碰到了上述问题， 欢迎试用）; 也可作为图片浏览器.

### 支持
- Win7/Win10+ 64位

### 特性
  - 漫画浏览模式: 空格/单击左键跳到图片的下一个浏览区域(衔接上一区域，mm会一次到底), 鼠标滚轮上下移动图片，
  方向键上下左右移动图片, PageDown/Up翻页, Ctrl+End跳到尾页, Ctrl+PageUp/Down跳目录,
  +/-放大缩小图片，按住左键拖拽图片
  - 窗口适应: 宽高(HOME)，满屏(End)， 原始(Ins), 自定义分辨率(F12); 全屏幕(Enter),还原(Esc)
  - 单双页显示: 双页时不显示gif
  - 智能开页: 根据文件名判断开页方向
  - 目录连续浏览: 跳到下一个兄弟目录， 但不会跳到上一层目录
  - 支持7z,rar/rar5, zip, cbz, cbr压缩格式: 文件浏览器右键打开; 内嵌压缩文件暂时不支持. 现在对于7z的策略是一次性加载到内存， 因此对于大的7z会比较慢.
  - 压缩文件打开后会根据文件列表排序, 主要是基于数字排序, 按L键在原始排序与数字排序之间切换
  - 64位: 支持大图，不会出现Win32里内存不足的提示
  - gif/webp动图播放: 连续翻页时只会显示gif的前面几帧
  - 幻灯播放: 点击右下角工具条的播放按钮(F5), 使用快捷键'[',']'来变更幻灯播放的时间间隔
  - unicode支持: 可以读取带有特殊字符的文件
  - 目录或压缩文件右键菜单打开: 跳到下一个目录是基于文件浏览器排序; 如果有everything(普通用户模式，工具 → 选项里关闭管理员，勾选服务)先按everything的顺序，其次是文件浏览器，最后是字母排序。
  - 操作基本兼容MangaMeeya, 鼠标左键下一页，右键上一页
  - 压缩文件删除子文件: 按快捷键(Ctrl+Del)删除当前显示的压缩文件中的子文件， 在该压缩文件关闭时（或程序关闭时)生效; 需要在config.ini中设置本地的压缩软件路径.
  - [漫画图片翻译](comic_trans/readme.md)：(T/Ctrl+T) config.ini里设置引擎
    - Baidu 打开百度翻译客户端， 发送热键Ctrl+Alt+X
  - GPU渲染， 对于大图用gpu快， 小图用cpu快， 3.0以上支持gpu，ini可以配置gpu=0来显式使用cpu，win7默认使用cpu
  - 本软件无恶意代码，不收集数据， 无任何互联网连接， 不查询升级， 升级自行到该发布页找新版本。

### changelog
2026/10/22 v3.1.217
- 优化显存占用， 优化内存占用

2026/10/17 v3.1.212
- 修正多个bug，优化内存
- 对解码进行提速

2026/10/1 v3.0.204
- 支持gpu渲染， 需要cuda显卡，有的话自动选择gpu，没有的选cpu

2026/8/28 v2.9.203
- 修复打开输入法后快捷键不响应的问题

2026/2/6  v2.9.199.0
- 优化webp加载
- 添加config设置对话框
- 废弃waifu2x插件

2026/2/5  v2.8.196.0
- 裁剪opencv，只保留jpg png webp解码

2025/8/23 v2.8.191.0
- 菜单里添加一个原始排序(L)

### 下载
  - github为唯一发布页，无任何推广， 纯粹是基于爱好开发， 永久免费软件。
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
