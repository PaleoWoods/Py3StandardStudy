## Python3 标准库模块
### 说明
本内容依据 Python3.7 版本标准库  
总共内置模块数为 `229` （包括二级模块，如：`collections.abc`, `os.path`）

### 文本

1. string: 通用字符串操作
2. re: 正则表达式操作
3. difflib: 差异计息工具
4. textwrap: 文本填充
5. unicodedata: Unicode 字符数据库
6. stringprep: 互联网字符串准备工具
7. readline: GNU 按行读取接口
8. rlcompleter: GNU 按行读取的实现函数

### 二进制数据

1. struct: 将字节解析为打包的二进制数据
2. codecs: 注册表与基数的编解码器（提供编解码数据的函数）

### 数据类型

1. datetime: 基于日期与时间工具
2. calendar: 能用月份函数（提供一组与日期相关的函数）
3. collections: 容器数据类型（提供一组有用的数据结构）
4. collectoons.abc: 窗口虚拟类（也可以理解为抽象类： abstractClass）
5. heqpq: 堆队列算法
6. bisect: 数组二分算法（为可排序的列表提供二分查的算法）
7. array: 高效数值数组
8. weakref: 弱引用
9. types: 内置类型的动态创建与命名
10. copy: 浅拷贝与深拷贝（提供复投数据的函数）
11. pprint: 格式化打印
12. reprlib: 交替 repr() 的实现

### 数学 

1. numbers: 数值的虚基类
2. math: 数学函数
3. cmath: 复数的数学函数
4. decimal: 定点数与浮点数计算
5. fractions: 有理数
6. random: 伪随机数函数

### 函数式编程
 
1. itertools: 为高效循环生成迭代器
2. functools: 可调用对象上的高阶函数与操作
3. operator: 针对函数的标准操作（提供实现基本的 Python 运算符功能的函数，可以使用这些函数而不是自己写 Lambda 表达式）

### 文件与目录

1. os.path: 通用路径名控制
2. fileinput: 从多输入流中遍历行
3. stat: 解释 stat() 的结果
4. filecmp: 文件与目录的比较函数
5. tempfile: 生成临时文件与目录（提供用于创建临时文件和目录的函数）
6. glob: Unix 风格路径名格式的扩展（提供用于匹配`unix`风格路径模式的函数）
7. fnmatch: Unix 风格路径名格式的比对（提供用于匹配`unix`风格文件名模式的函数）
8. linecache: 文本行的除湿机存储
9. shutil: 高级文件操作（提供对高级文件处理函数的访问）
10. macpath: MacOS 9 路径控制函数 （deprecated in 3.7 and will be removed in 3.8,可以不用专门学习使用）

### 持久化

1. pickle: Python 对象的序列化
2. copyreg: 注册机对  pickle 的支持函数
3. shelve: Python 对象的持久化
4. marshal: Python内部对象序列化
5. dbm: Unix “数据库”接口
6. sqlite3: 针对 SQLite 数据库的 API2.0

### 压缩

1. zlib: 兼容 gzip 的压缩
2. gzip: 对 gzip 文件的支持
3. bz2: 对bzip2 压缩的支持
4. lzma: 使用 LZMA 算法的压缩 
5. zipfile: 操作 ZIP 存档
6. tarfile: 读写 tar 存档文件

### 文件格式化

1. csv: 读写 CSV 文件
2. configparser: 配置文件解析器
3. netrc: netrc 文件处理器
4. xdrlib: XDR 数据编码与解码
5. plistlib: 生成和解析 MacOS X `.plist` 文件

### 加密
1. hashlib: 安全散列与消息摘要
2. hmac: 针对消息认证的键散列

### 操作系统工具

1. os: 多方面的操作系统接口（提供对基本的操作系统函数的访问）
2. io: 流核心工具（提供用于处理 I/O 流的函数，在 python3 还包含 StringIO, 可以像处理文件一样处理字符串）
3. time: 时间的查询与转化
4. argparser: 命令行选项、参数和子命令的解析器（提供解析命令行参数的函数）
5. optparser: 命令行选项解析器
6. getopt: C 风格的命令行选项解析器
7. logging: Python 日志工具
8. logging.config: 日志配置
9. logging.handlers: 日志处理器
10. getpass: 简易密码输入
11. curses: 字符显示的终端处理
12. curses.textpad: curses 程序的文本输入域
13. curses.ascii: ASCII 字符集工具
14. curses.panel: curses 的控件栈扩展
15. platform: 访问底层平台认证数据
16. errno: 标准错误记号
17. ctypes: Python 外部函数库

### 并发

1. threading: 基于线程的并行（提供对处理高级线程功能的访问）
2. multiprocessing: 基于进程并行（可以在应用程序中运行多个子进程，而且提供 API 让那个子进程看上去像线程一样）
3. concurrent: 并发包（提供一部计算）
4. concurrent.futures: 启动并行任务
5. subprocess: 子进程管理
6. sched: 事件调度（提供一个无需多线程的事件调度器）
7. queue: 同步队列
8. select : 等待 I/O 完成（提供对函数 `select()` 和 `poll()` 的访问，用于创建事件循环）
9. dummy_threading: threading 的模块替代（当 `_thread` 不可用时）
10. `_thread`: 底层的线程 API(threading 基于其上)
11. `_dummy_thread`: `_thread` 模块的替代（当 `_thread` 模块不可用时）

### 进程间通信

1. socket: 底层网络接
2. ssl:  socket 对象的 TLS/SSL 填充器
3. asyncore: 异步套接字处理器
4. signal: 异步事务信号处理器（提供用于处理 POSIX 信号的函数）
5. mmap: 内存映射文件支持

### 互联网

1. email: 邮件与 MIME 处理包
2. json: JSON 编码与解码
3. mailcap: mailcap 文件处理
4. mailbox: 多种格式控制邮箱
5. mimetypes: 文件名与 MIME 类型映射
6. base64: RFC3548 - Base16/Base32/Base64编码
7. binhex: binhex4文件编码与解码
8. binascii: 二进制码与 ASCII 码间的转化
9. quopri: MIME quoted-printable 数据的编码与解码
10. uu: uuencode 文件的编码与解码

### HTML 与  XML

1. html: HTML 支持
2. html.parser: 简单 HTML 与 XHTML 解析器
3. html.entities: HTML 通用实体定义
4. xml: XML 处理模块
5. xml.etree.ElementTree: 树形 XML 元素 API
6. xml.dom: XML DOM API
7. xml.dom.minidom: XML DOM 最小生成树
8. xml.dom.pulldom: 构建部分 DOM 树的支持
9. xml.sax: SAX2解析的支持
10. xml.sax.handler: SAX 处理器基类
11. xml.sax.saxutils: SAX 工具
12. xml.sax.xmlreader: SAX 解析器接口
13. xml.parsers.expat: 运用 Expat 快速解析 XML

### 互联网协议与支持

1. webbrowser: 简易 Web 浏览器控制器
2. cgi: CGI 支持
3. cgitb: CGI 脚本反射追踪管理器
4. wsgiref: WSGI 工具与引用实现
5. urllib: URL 处理模块，提供处理和解析 URL 的函数
6. urllib.request: 打开 URL 链接的扩展库
7. urllib.response: urllib 模块的响应类
8. urllib.parse: 将 URL 解析成组件
9. urllib.error: urllib.request 引发的异常类
10. urllib.robotparser: robots.txt 的解析器
11. http: HTTP 模块
12. http.client: HTTP协议客户端
13. ftplib: FTP 协议客户端
14. poplib: POP 协议客户端
15. imaplib: IMAP4 协议客户端
16. nnptlib: NNPT 协议客户端
17. smtplib: SMTP 协议客户端
18. smptd: SMTP 服务器
19. telnetlib: Telent 客户端
20. uuid: RFC4122的 UUID对象（可以生成全局唯一标志的 Universally unique identifies）
21. socketserver: 网络服务器框架
22. http.server: HTTP服务器
23. http.cookies: HTTPCookie 状态管理器
24. http.cookiejar: HTTP 客户端的 Cookie 处理
25. xmlrpc: XML-RPC 服务器和客户端模块
26. xmlrpc.client: XML-RPC 客户端访问
27. xmlrpc.server: XML-RPC 服务器基础
28. ipaddress: IPv4/IPv6控制库

### 多媒体
1. audioop: 处理原始音频数据
2. aifc: 读写 AIFF/AIFC 文件
3. sunau: 读写 Sun AU 文件
4. wave: 读写 WAV 文件
5. chunk: 读取 IFF 大文件
6. colorsys: 颜色系统间转化
7. imghdr: 指定图像类型
8. sndhdr: 指定声音文件类型
9. ossaudiodev: 访问兼容 OSS 的音频设备

### 国际化

1. gettext: 多语言的国际化服务
2. locale: 国际化服务

### 编程框架

1. turtle: Turtle图形库
2. cmd: 基于行的命令解释器支持
3. shlex: 简单词典分析

### TK 图形用户接口（TK GUI）

1. tkinter: Tcl/Tk 接口
2. tkinter.ttk: Tk 主题控件
3. tkinter.tix: Tk 扩展控件
4. tkinter.scrolledtext: 滚轴文本控件

### 开发工具

1. pydoc: 文档生成器和在线帮助系统
2. doctest: 交互式 Python 示例
3. unittest: 单元测试框架
4. unittest.mock: 模拟对象库
5. test: Python 回归测试包
6. test.support: Python 测试工具套件
7. venv: 虚拟环境搭建

### 调试

1. bdb: 调试框架
2. faulthandler: Python 反向追踪库
3. pdb: Python调试器
4. timeit: 小段代码执行时间测算
5. trace: Python 执行状态追踪

### 运行时

1. sys: 系统相关的参数与函数
2. sysconfig: 访问 Python 配置信息
3. builtins: 内置对象
4. main: 顶层脚本环境
5. warnings: 警告控制
6. contextlib: with 状态的上下文工具
7. abc: 虚基类
8. atexit: 出口处理器（允许注册在程序退出时调用的函数）
9. traceback: 打印或读取一条栈的反向追踪
10. future: 未来状态定义
11. gc: 垃圾回收接口
12. inspect: 检查存活的对象
13. site: 网址相关的配置钩子（Hook）
14. fpectl: 浮点数异常控制
15. distutils: 生成和安装 Python 模块

### 解释器

1. code: 基类解释器
2. codeop: 编译 Python 代码

### 导入模块

1. imp: 访问 import 模块的内部
2. zipimport: 从 ZIP 归档中导入模块
3. pkgutil: 包扩展工具
4. modulefinder: 通过脚本查找模块
5. runpy: 定位并执行 Python 模块
6. importlib: import 的一种实施

### Python 语言

1. parser: 访问 Python 解析树
2. ast: 抽象句法树
3. symtable: 访问编译器符号表
4. symbol: Python 解析树中的常量
5. token: Python 解析树中的常量
6. keyword: Python 关键字测试
7. tokenize: Python 源文件分词
8. tabnany: 模糊缩进检测
9. pyclbr: Python 类浏览支持
10. py_compile: 编译 Python 源文件
11. compileall: 按字节编译 Python 库
12. dis: Python 字节码的反汇编器
13. pickletools: 序列化开发工具

### 其他
1. formatter: 通用格式化输出

### Windows 相关
1. msilib: 读写 Windows Installer 文件
2. msvcrt: MS VC++ Runtime 的有用程序
3. winreg: Windows 注册表访问
4. winsound: Windows 声音播放接口

### Unix 相关
1. posix: 最常用的 POSIX 调用
2. pwd: 密码数据库
3. spwd: 影子密码数据库
4. grp: 组数据库
5. crypt: Unix 密码验证
6. termios: POSIX 风格的 tty 控制
7. tty: 终端控制函数
8. pty: 伪终端工具
9. fcntl: 系统调用和`fcntl()` 和 `ioctl()`
10. pipes: shell 管理接口
11. resource: 资源可用信息
12. nis: Sun 的 NIS 接口
13. syslog: Unix syslog 程序库
