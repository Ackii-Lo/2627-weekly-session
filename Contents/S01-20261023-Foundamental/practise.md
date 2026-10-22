## VSCode 相关操作

```bash
# 基础操作

Ctrl + Shift + P    # 打开命令面板

Ctrl + P            # 快速打开文件

Ctrl + W            # 关闭当前标签

Ctrl + Shift + T    # 重新打开刚才关闭的标签

Ctrl + Shift + N    # 新建独立窗口

Ctrl + S            # 保存（重要性不必多言）

Ctrl + ,            # 打开设置

# 编辑技巧

Alt + Click         # 再任意位置手动添加光标

Ctrl + Alt + 上/下  # 再当前行的上方或者下方添加光标

Ctrl + D            # 逐个选中相同的词

Ctrl + C            # 直接复制整行（不是选中复制，不要小看了）

Ctrl + X            # 直接剪切整行

Ctrl + Shift + K    # 删除整行

# 导航搜索

F12                 # 跳转到定义（你猜什么意思？试试就知道了，选中一个python中的函数然后按下F12）

Ctrl + Shift + F    # 全局搜索

Ctrl + F            # 当前文本内搜索

F2                  # 批量重命名
```

---

## VSCode 实用插件

- Prettier

- GitLens

- Error Lens

- Code Spell checker

- Remote 家族

---

## 可执行文件

对于Windows：

后缀为 `.exe` 的文件

对于macos：

无后缀文件

---

## 快捷方式

尝试对心仪的可执行文件使用~~炎拳~~创建快捷方式吧

---

编译实践

```bash

gcc -E test.c -o test.i

gcc -S test.i -o test.s

gcc -c test.s -o test.o

gcc test.o -o test

# python和C对比

gcc test.c -o test

python test.py

```

## 计算机基础元器件

- 控制器 (CPU)

- 运算器 (GPU)

- 存储器 (主存，硬盘)

- IO设备（键盘，鼠标，etc）

- Type B/C

- 主板

- 网卡

- 总线

---

CPU：

- 用于进行逻辑运算和部分算术运算

- 多核

---

GPU：

- 极大的数据吞吐量

- 并行运算非常快

- 显存

---

存储：

存储结构：

| 层级 | 典型介质 | 访问时间量级 | 容量量级 | 易失性 |
| --- | --- | --- | --- | --- |
| 寄存器 | 触发器（CPU 芯片内） | 亚纳秒 ~ 1 周期 | 几十 ~ 几百字节 | 易失 |
| Cache | SRAM | 0.5 ~ 2.5 ns | KB ~ 几十 MB | 易失 |
| 主存 | DRAM | 50 ~ 70 ns | GB ~ TB | 易失 |
| 辅存 | 磁盘 / SSD | 毫秒级（磁盘） | TB ~ PB | **非易失** |

---

主板

- 整体的骨架

- 统筹兼顾通信和供电等等

---

网卡

- 有线网卡

- 无线网卡

- 虚拟网卡

---

### 网络通信

从mac地址到ARP表

---

### URL结构

```text
scheme://userinfo@host:port/path?query#fragment
```

- `scheme`: 协议名

- `userinfo`: 用户信息（不怎么用，会泄露信息）

- `host`: 目标主机的域名

- `port`: 端口（每个计算机都会有很多端口用于和外部网络交互）

- `path`: 资源在目标服务器上的路径

- `query`： 查询串（发给服务器的）

- `fragment`: 指向资源内部片段

---

### 工作原理

当输入url，请求会被发给DNS解析服务器

然后DNS解析服务器会根据你输入的域名，查找过后返回对应的IP给浏览器。

浏览器得到IP地址之后，就可以直接访问ip地址所对应的服务器

---

### 终端

打开终端

```bash
#windows

windows + R

输入powershell，然后回车

#macos

command + space

输入terminal.app，然后回车

```

什么是终端

- 物理终端（上古时期）

- 终端模拟器（伪终端）

伪终端分为两端：

- 主端：由终端模拟程序或者远程服务程序控制

- 从端：和与终端交互的程序链接，作为该程序的输入输出

---
