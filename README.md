#SeeComic
Simple and fast manga browser.
[中文文档](https://github.com/nessessary/SeeComic/blob/master/readme_cn.md)

### support
- Win7/Win10 64bit

### Features
  - Comic browsing mode: space/left click to jump to the next browsing area of ​​the picture, mouse wheel to move the picture up and down, arrow keys to move the picture up, down, left and right, PageDown/Up to turn pages, Ctrl+End to jump to the last page, +/- To zoom in and out of the picture, hold down the left button and drag the picture
  - Window adaptation: width and height (HOME), full screen (End), original (Ins), custom resolution (F12); full screen (Enter), restore (Esc)
  - Single and double page display: no gif is displayed when double page
  - Smart page opening: determine the page opening direction according to the file name
  - Directory continuous browsing: skip to the next sibling directory, but not to the previous directory
  - Support 7z, rar/rar5, zip, cbz, cbr compression formats: right-click to open the file browser; embedded compressed files are temporarily not supported. Now the strategy for 7z is to load into memory at one time, so it will be slower for large 7z .
  - File list sorting: After opening the compressed package or directory, the pictures in it will be sorted by numbers
  - 64-bit: support large image, no prompt of insufficient memory in Win32
  - gif/webp animation playback: only the first few frames of the gif will be displayed when the pages are turned continuously
  - Slide show: Click the play button (F5) on the toolbar at the lower right corner, use the shortcut keys '[',']' to change the time interval of the slide show
  - unicode support: can read files with special characters
  - Right-click to open a directory or compressed file: Jumping to the next directory is based on the file browser sorting; if there is anything, it is first sorted by everything, followed by the file browser, and finally alphabetically.
  - The function is basically compatible with MangaMeeya, the left mouse button goes to the next page, and the right mouse button goes to the previous page
  - Deleting sub-files from compressed files: Press the shortcut key (Ctrl+Del) to delete sub-files in the currently displayed compressed file, which will take effect when the compressed file is closed (or when the program is closed); local compression needs to be set in config.ini software path.
  - Support compressed file password: The entered password is saved in the text, and the password list can be used first to decrypt it next time. Nested compression is not supported, and file list encryption is not supported.
  - waifu2x filter: (W) Process in memory, do not destroy the original image, use default parameters.
  - Comic image translation: (T) Generate a new post-translation compressed package, generate it in a command line, and automatically open it after generation
  - This software is permanently free, no malicious code, no data collection, no Internet connection, no query upgrade, please download the release version by yourself to upgrade.

### Feedback
  - If you have bugs or suggestions, please send issuse or email to: nesserrary@gmail.com
