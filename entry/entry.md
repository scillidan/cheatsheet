```
^ [caret]
  来自拉丁语 意为它缺失 源自carere 意为缺乏分开,摆脱
  最初并继续在手写中作为校对标记 出现在行级标点的下方 或在行的上方倒置指示楔子的位置 插入的材料可置于符号(夹角)内,上下边距间
  某些编程语言表示异或的符号 本体是数字和逻辑里的二元逻辑运算符

&& [AND IF]
  是连接冗长命令的if-then构造的and操作

s/mime [secure multipurpose internet mail extensions] [安全型多用途网络邮件拓展]

SMTP [简单邮件传输协议]
  用于发送电子邮件

license [许可]
  与著作权相关
  可视为作者,贡献者,用户间最小的社会,法律合同

jpg [joint photographic experts group] [联合图像专家小组]
  一套针对静态数字图像的失真压缩标准
  可被嵌入tiff(tagged image file format 标签图像文件格式) 后者通常被视为一种图像交换格式 用于在正式格式间传输高质量图像 存在兼容缺陷
  可用于长期储存真实相片 不应选择为导出的格式来另存文件 或者图像处理时的中间文件 特别是包含大面积纯色,文字,线条,图标

ttf [truetype font]
  常见的字体格式
  可嵌入数字版权管理(drm, digital rights management)标签
  排印中 字体(typeface)指单组或多组的字模(font)构成的集合 通常含特定的风格,字重,斜体,装饰,字符集,用途,设计师,铸字厂等特征
  其他格式如 otf(opentype font)用以替代ttf但扩展名存在混用 支持多平台和扩展字符集 eot(embedded open type)只有ie支持 woff(web open font format)受主流的浏览器支持 svg(scalable vector graphics font)由svg元素定义

sfz [software synthesizer] [软合成器]
  定义声音样本的行为,存储合成器的数据的纯文本(plain text)格式的文件
  这类文本归为标记语言(markup language) 通常是可读的

ascii [american standard code for information interchange] [美利坚信息交换标准代码]
  基于拉丁字母的一套电脑编码系统
  一套被普遍接受的映射关系表 编码协议
  0-31的字符起一定控制作用 常称为控制字符 不可显示 不可打印

vsync [垂直同步]
  同步到显示器的刷新率

uefi [unified extensible firmware interface] [统一可扩展固件接口]
  操作系统和平台固件间的一套软件界面的规范
  用于替代个人电脑开机阶段内 初始化硬件的软件bios(basic input/output system 基础输入输出系统)
  该标准中的gpt(guid(globally unique identifier) partition table 全局唯一标识符分区表) 一个实体硬盘分区表的结构布局标准 就用来替代旧启动式mbr(master boot record 主引导记录)

shimmer
  祖安特调“微光”

转写 [transl] [transliteration]
  将拼音文字系统的字符按对照表转换成另一套拼音文字系统的字符
  包含基础字符的附加符 用双字符表示的单音素

缩写 [abbr] [abbreviation]
  首字缩写但按词发音
  其中 [字母词] 首字缩写但按逐字母发音 倾向不使用句号间隔字母 [冗余首字缩写综合征] 多词首字组词 但某个或几个词被重复 [简写] 部分属于中略 一般在尾部加一个点 不改变读法 [截音] 截取词的部分

码率 [bit rate]
  每秒的比特数 相关的编码形式有 [可变码率(vbr, variable bit rate),两次固定平均码率(2-pass abr),固定码率(cbr, constants bit rate)
  视频方面 固定码率系数(crf, constant rate factor)的通用值为23 视觉无损使用17 网络流媒体可用29
  音频方面 mp3默认使用cbr ogg使用vbr

采样率 [sample rate]
  声音由模拟信号转换成数字信号时 从连续信号提取以组成离散信号的每秒的采样数
  数位音乐常用44100hz 数位影视常用48000hz 蓝光碟等专业级常用96000hz
```

```
.csv
  最早，我有一个专门的`.txt`文件来记录各类东西，也用于使用Grep检索
  后来使用`.csv`格式
  2022-2023年间，相对集中地多次拆分、合并文本
  2023年下半年开始，部分地迁移到Notion，后来又从Notion移回到Markdown表格
缩写
  我之前在填`.csv`的`tag`列时，为了避免行变得更长，使用了(或不)常见的缩写，如`wdw[window]`、`kbd[keyboard]`，于是有了一个收集遇到的缩写的`abbr.csv`文件
  最早是直接搜索谷歌`<word> abbreviation`
  后来使用[All Acronyms](https://www.allacronyms.com/)
  缩写词也有其他的来源和例外情况。如scene的缩写使用了sn，参考[从新·EVA特报2中可以获取到什么信息？](https://www.bilibili.com/video/BV1zt411E7RV/)
可写易读
  2023年年底，开始从Logseq移除了多个页面
  删减了列数，并在`.md`写由AlignTab对齐的表格。要回收所有`.csv`的事情开头了
  将一些配置文件的备份从MegaSync移到了git
  最近被迫重装了系统，手动去恢复、调整配置时，也在养成更节能、可写、易读的习惯
hypothesis
  之前使用这个插件来标记或者摘抄词条、段落、整篇文章等等。例如，之前我需要使用curl时遇到问题，读到了[deleting system32\curl.exe](https://daniel.haxx.se/blog/2023/04/24/deleting-system32curl-exe/)。我将这类`已读的`全部记在`reference.md`文件提到，很多是跟`故障排除`有关。直到我在自用的install_scoop.bat中列出了curl，就可以清除这篇文章链接，因为我不再会偶然地使用到Windows10的`curl.exe`。实际上我总是在很久之后才清理这类长时间保存的文件。
```

```
lua
  1993年诞生在巴西 葡萄牙语中是月亮的意思
  一种动态脚本语言 常用于配置(config),运行时(runtime) 适合嵌入更大的脚本,库 进行交互
  除基础变量外 大部分都在引用表上数据
  表类似Python的字典(dictionary)或JavaScript中的实体(object) 

python
  [[]]
    有时同一个符号会用于多种用途
    在Python中 通常是列表,值的序列(sequence) 或者用于可选内容,元素(element)
    索引时从0开始 可与字典嵌套
    解释命令时在程序文件自身后以序号0开始
    与值不可变的元组(tuple) 在被访问时都使用\[\]
  [{}]
    通常是字典,键值的无序序列 当索引键时 返回值 当进行赋值时 使用\[\]
  [()]
    用于可填入参数的函数(function)名,传入变量(variable) 作前者时被称为方法(method) 有时具有默认参数 一般能从官方文档检阅 而后者存在在范围(scope)内
    嵌套,组织顺序时 从内到外读
    可作为布尔表达式在条件句子中
  [:] 将处理以下缩进的每行
    部分函数需作为modules更仔细地装载入内存
  [.] 用来间隔模块
  [`__init__.py`] 将文件夹视为一个包(package)
  [f"{}"] 格式化字符串

class
  函数的容器
  制作相关联的数据,代码的一张图纸 包含字段,功能
  根据模型图纸 可制造属性方法各异的多个实体
```