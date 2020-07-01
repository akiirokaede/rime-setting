# 秋色枫自用的 Rime 输入法配置
基本配置 fork 自[lorest/rime-setting仓库](https://github.com/Iorest/rime-setting)。

在此基础上，我：
1. 删除了自然码双拼
2. 修改了 easy_en 输入法配置使其默认输入英文字符
3. 增加了 rime-japanese 输入法，因为输入习惯的问题我觉得这个比 ibus-anthy 更好用，然后稍作改动让他的行为和其他输入法一致
4. 修改了英文切换的按键绑定，像 macOS 内置输入法那样，按大写锁定切换中（日）英文输入，shift 只保留长按输入大写字符和上档键的功能（需要中英文混写的时候，这样设置的好处就凸显出来了）
5. 增加了自制的实验性质的莫尔斯电码输入法，敲击大写字母和阿拉伯数字可以直接输入对应的莫尔斯电码，之后试着给小写字母加一些常用缩写的词库
6. 更改了各输入方案的显示名称，有效减轻自己的强迫症发病情况

## 用法

1. 安装[Rime输入法](https://rime.im/)，并注销或重启
2. 下载仓库所有配置到本地
3. 将下载的除字体外的所有文件覆盖到用户设定文件夹中
4. 安装明朝花园体（可选，字符很全，可以避免输入法中出现方块字符）

    `sudo pacman -S ttf-hanazono`

5. 重新部署 Rime，部署完毕即可用

用户设定文件夹的位置：
- Windows
  - Weasel: %APPDATA%\Rime
- macOS
  - Squirrel: ~/Library/Rime
- Linus
  - iBus: ~/.config/ibus/rime
