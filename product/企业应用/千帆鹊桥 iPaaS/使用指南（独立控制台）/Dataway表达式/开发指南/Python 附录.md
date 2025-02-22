[](id:builtin-refs)
## 内置函数

目前代码模式 Python 支持的内置函数如下：

| 序号 | 内置函数     | 功能说明                                                     |
| ---- | ------------ | ------------------------------------------------------------ |
| 1    | abs()        | 求数值绝对值                                                 |
| 2    | all()        | 判断序列（集合、列表、元组、dict) 中所有元素是否满足给定条件 |
| 3    | any()        | 判断集合中是否存在元素满足给定条件                           |
| 4    | bool()       | 构造布尔值                                                   |
| 5    | bytearray()  | 构造字节数组                                                 |
| 6    | bytes()      | 构造空字节                                                   |
| 7    | chr()        | 0~256的整数对应的ASCII码                                     |
| 8    | dict()       | 创建字典                                                     |
| 9    | enumerate()  | 将一个可遍历的数据对象组合列出数据和数据下标，一般用于 for   循环中 |
| 10   | filter()     | 集合过滤，如 list(filter(lambda   x:x>=100, [1,3,4,100,102])) -> [100,102] |
| 11   | float()      | 构造浮点数                                                   |
| 12   | getattr()    | 求一个对象的属性值                                           |
| 13   | hasattr()    | 判断一个对象是否有某个属性                                   |
| 14   | hash()       | 求哈希值                                                     |
| 15   | id()         | 求对象的唯一标识                                             |
| 16   | int()        | 构造整数                                                     |
| 17   | isinstance() | 判断对象是否属于某种类型                                     |
| 18   | iter()       | 生成一个迭代器                                               |
| 19   | len()        | 获取集合元素个数                                             |
| 20   | list()       | 构造列表                                                     |
| 21   | map()        | 根据函数对指定序列做映射，如 list(map(lambda x: x * 2, [1, 2, 3, 4, 5])) -> [2, 4, 6, 8, 10] |
| 22   | max()        | 获取数值最大值                                               |
| 23   | min()        | 数值最小值                                                  |
| 24   | next()       | 返回迭代器的下一个项目，和 iter() 一起使用                   |
| 25   | objects()    | 返回空对象                                                   |
| 26   | ord()        | 单个ASCII码字符的整数值                                      |
| 27   | pow()        | 求指数                                                       |
| 28   | print()      | 代码模式 Python 调试时可以打印相关信息（仅在 Dataway   表达式编辑时使用 Debug 功能生效） |
| 29   | range()      | 创建可迭代对象，如 list(range(5)) -> [0,   1, 2, 3, 4]       |
| 30   | reversed()   | 创建反转的迭代器，如   list(reversed('abcdefg')) -> ['g', 'f', 'e', 'd', 'c', 'b', 'a'] |
| 31   | round()      | 截取数值的整数部分                                           |
| 32   | set()        | 创建一个集合                                                 |
| 33   | slice()      | 设置截取元素的切片                                           |
| 34   | sorted()     | 排序                                                         |
| 35   | str()        | 构造字符串                                                   |
| 36   | sum()        | 数值求和                                                     |
| 37   | tuple()      | 构造元组                                                     |
| 38   | type()       | 返回对象类型                                                 |
| 39   | zip()        | 打包可迭代对象中元素成多个 tuple。如   list(zip([1,2,3], [4,5,6])) -> [(1, 4), (2, 5), (3, 6)] |


[](id:modules)
## 第三方模块
### time
time 用于时间处理的库，可参考 [Python 官方文档](https://docs.python.org/zh-cn/3.5/library/time.html)。已内置代码模式 Python，可以直接引用。

目前代码模式 Python 支持的库函数/类型如下：

| 序号 | 库函数/类型 | 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
| 1    | altzone           | 当前时区相对于 UTC 时区的延迟偏移，单位为秒                  |
| 2    | asctime           | 将一个 struct_time 转换为时间字符串                          |
| 3    | ctime             | 将一个时间戳转换为时间字符串                                 |
| 4    | mktime()          | 将一个 struct_time 转换为时间戳                              |
| 5    | strftime()        | 将一个 struct_time 进行格式化                                |
| 6    | strptime()        | 按照给定的格式解析事件字符串，并返回一个结构化的struct_time对象 |
| 7    | timezone          | 当前时区                                                     |
| 8    | tzname            | 当前时区名称                                                 |
| 9    | time()            | 当前时间                                                     |
| 10   | localtime         | 将一个时间戳转换为当前时区的本地时间，返回 struct_time 类型对象 |
   
	 
### json 
json 用于处理 json 数据的库，可参考 [Python 官方文档](https://docs.python.org/zh-cn/3.5/library/json.html)。已内置代码模式 Python，可以直接引用。

目前代码模式 Python 支持的 json 模块函数：

| 序号 | json 模块函数 | 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   |  dumps()   | 将 json 对象编码为 json 字符串  |
|  2   |  loads()     | 将一个 json 串解析为 Python 对象  | 


### math
math 用于数学运算的库，可参考 [Python 官方文档](https://docs.python.org/zh-cn/3.5/library/math.html)。已内置代码模式 Python，可以直接引用。

目前代码模式 Python 支持的 math 模块函数：  

| 序号 | json 模块函数 | 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|   1  | math.ceil(x)  | 返回 x 的上限，即大于或者等于 x 的最小整数。如果 x 不是一个浮点数，则委托 x.ceil()，返回整数值。  | 
|   2  | math.floor(x)   | 返回 x 的向下取整，小于或等于 x 的最大整数。如果 x 不是浮点数，则委托 x.floor() ，返回整数值。  | 
|   3  |  math.fabs(x)  | 返回 x 的绝对值。  | 
|   4  | math.pow(x,y)  | 返回 x 的 y 次幂。  | 
|   5  | math.sqrt(x)     |  返回 x 的平方根。  | 

支持的常量：

| 序号 | 常量 | 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|	1 |  math.pi | 数学常数 π = 3.141592...，精确到可用精度。 | 
|	2 |  math.e | 数学常数 e = 2.718281...，精确到可用精度。 | 
|	3 |  math.inf | 浮点正无穷大。（对于负无穷大，使用 -math.inf）相当于 float('inf') 的输出。 | 
|	4 |  math.nan | 浮点“非数字”（NaN）值。 相当于 float('nan') 的输出。 | 


### base64
base64 用于 base64 编解码的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/base64.html)。已内置代码模式 Python，可以直接引用。 支持的函数有：

| 序号 |支持的函数| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   |  base64.b64encode(s)  | 对 bytes 类型参数 base64 编码，返回编码后的 bytes。  | 
|  2   | base64.b64decode(s)   |  对 bytes/str 类型参数 base64 解码，返回解码后的 bytes。  | 


### hmac
hmac 用于 hmac 加解密的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/hmac.html)。已内置代码模式 Python，可以直接引用。 支持的函数有：
   
| 序号 |支持的函数| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   |  hmac.new(key)  | 返回一个新的 hmac 对象, key 是一个指定密钥的 bytes 或 bytearray 对象。  | 


### random
random 用于随机数生成的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/random.html)。已内置代码模式 Python，可以直接引用。 支持的函数有：
  
| 序号 |支持的函数| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   |  random.randint(a,b) | 返回随机整数 N 满足 a <= N <= b。  | 


###  hashlib  
hashlib 用于生成哈希值的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/hashlib.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   | hashlib.sha256()  |  创建一个 SHA-256 hash 对象。  | 
|  2   | hashlib.md5()  |  创建一个 MD5 的 hash 对象。  | 
|  3   | hashlib.sha1()  | 创建一个 SHA1 的 hash 对象。  | 
    

### datetime
datetime 用于时间日期处理的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/datetime.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
| 1   | datetime.date   |一个理想化的简单型日期，它假设当今的公历在过去和未来永远有效。属性有: year, month 和 day。   |
| 2   | datetime.time    | 一个理想化的时间，它独立于任何特定的日期，假设每天一共有 24*60*60 秒。 属性有： hour, minute, second, microsecond 和 tzinfo。   |
| 3   | datetime.datetime   | 日期和时间的结合。属性有：year, month, day, hour, minute, second, microsecond 和 tzinfo。   |
| 4   | datetime.timedelta   | 表示两个 date 对象或者 time 对象，或者 datetime 对象之间的时间间隔，精确到微秒。   |
| 5   | datetime.timezone   | 表示相对于世界标准时间（UTC）的偏移量。   |
| 6   | datetime.tzinfo   | 描述时区信息对象, 用来给 datetime 和 time 类提供自定义的时间调整概念，如处理时区和/或夏令时。   |
	
	
### decimal
decimal 用于定点数处理的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/decimal.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1  | decimal.Decimal |  表示十进制浮点数对象。 |


### socket
socket 是 Python 中 tcp 套接字的底层实现，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/socket.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|   1  |  socket.htonl()  | 将 32 位正整数从网络序转换成主机字节序。  |
|   2  |  socket.ntohl()  | 将 32 位正整数从网络字节序转换为主机字节序。  |


### pycryptodome
pycryptodome 是专用的加密工具三方库，可参考 [pycryptodome官方文档](https://pycryptodome.readthedocs.io/en/latest/)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|   1  | Crypto.Util.Padding | 该模块为添加和删除数据中的标准填充提供了最小的支持, 提供 pad()、unpad() 方法。 |
|   2  | Crypto.Cipher.AES  | AES 加密模块。它具有16字节的固定数据块大小，密钥可以是128、192或256位长。提供 new() 方法。 |


### struct
struct 用于打包二进制文件的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/struct.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|   1  |  struct.pack(format, v1, v2, ...) | 返回一个 bytes 对象，其中包含根据格式字符串 format 打包的值 v1, v2, ... 参数个数必须与格式字符串所要求的值完全匹配。|
|   2  |   struct.unpack(format, buffer) | 根据格式字符串 format 从缓冲区 buffer 解包，返回一个 tuple。|
  
	
### urllib	
urllib 用于 URL 处理的库，可参考 [Python官方文档](https://docs.python.org/zh-cn/3.5/library/urllib.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|   1  |  urllib.parse.urlparse()  | 获取 url 参数，将 url 解析成一个包含6个字符串的 tuple，分别为：协议，位置，路径，参数，查询，片段识别。|
|   2  |  urllib.parse.unquote() |  将编码的 url 进行解码。 |


### csv
csv 用于 CSV 文件读写的库，可参考 [Python官方文档](#https://docs.python.org/zh-cn/3.5/library/csv.html)。已内置代码模式 Python，可以直接引用。 支持的函数/属性有：

| 序号 |支持的函数/属性| 功能说明                                                     |
| ---- | ----------------- | ------------------------------------------------------------ |
|  1   | csv.reader()  |   创建一个 reader对象，将逐行遍历 csv 文件对象。|
