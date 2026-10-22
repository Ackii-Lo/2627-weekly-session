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

Alt + Click         # 在任意位置手动添加光标

Ctrl + Alt + 上/下  # 在当前行的上方或者下方添加光标

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

```js
//Origin version

const user={name:'Alice',age:25,hobbies:['reading','coding','hiking']};
function greet(user){if(user.age>=18){console.log(`Hello, ${user.name}! You are an adult.`)}else{console.log(`Hi, ${user.name}!`)}}

//Prettier version:

const user = {
  name: "Alice",
  age: 25,
  hobbies: ["reading", "coding", "hiking"],
};

function greet(user) {
  if (user.age >= 18) {
    console.log(`Hello, ${user.name}! You are an adult.`);
  } else {
    console.log(`Hi, ${user.name}!`);
  }
}
```

- Error Lens

- Code Spell checker

---

## 可执行文件

对于Windows：

后缀为 `.exe` 的文件

对于macOS：

无后缀文件（编译产物默认无后缀），此外还有 .app（应用包）、.dmg（磁盘映像）等形式

---

## 快捷方式

尝试对心仪的可执行文件使用~~炎拳~~创建快捷方式吧

---

## 编译实践

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

冯·诺依曼体系五大部件：

- CPU（含控制器 + 运算器）

- 存储器（主存，硬盘）

- IO设备（键盘，鼠标，etc）

  - USB Type-B / Type-C 等接口标准

其他重要组件：

- GPU（图形/并行协处理器，不属于经典五大部件）

- 主板

- 网卡

- 总线

---

CPU：

- 计算机的核心，内部包含控制器（CU）和运算器（ALU）

- 控制器负责指令译码与调度

- 运算器负责算术运算和逻辑运算

- 多核（现代 CPU 集成多个核心，可同时处理多个任务）

---

GPU：

- 专用的并行处理器，擅长大规模数值计算和图形渲染

- 极大的数据吞吐量

- 并行运算非常快（核心数远多于 CPU，但单核能力弱于 CPU）

- 显存（GPU 自带的高速内存，独立于主存）

---

存储：

存储结构：

| 层级 | 典型介质 | 访问时间量级 | 容量量级 | 易失性 |
| --- | --- | --- | --- | --- |
| 寄存器 | 触发器（CPU 芯片内） | 亚纳秒 ~ 1 周期 | 几十 ~ 几百字节 | 易失 |
| Cache | SRAM | 0.5 ~ 2.5 ns | KB ~ 几十 MB | 易失 |
| 主存 | DRAM | 50 ~ 70 ns | GB ~ TB | 易失 |
| 辅存 | HDD / SSD | 毫秒级（HDD）/ 微秒级（SSD） | TB ~ PB | **非易失** |

---

主板

- 整体的骨架，所有部件都安装在主板上或通过主板连接

- 承载芯片组、扩展插槽，统筹兼顾通信和供电

---

网卡

- 有线网卡（通过网线连接，速率稳定）

- 无线网卡（通过 Wi-Fi 连接）

- 虚拟网卡（由软件模拟，常用于虚拟机、VPN 等场景）

---

### 网络通信

从mac地址到ARP表

---

### URL结构

```text
scheme://host:port/path?query#fragment
```

- `scheme`: 协议名

- `host`: 目标主机的域名

- `port`: 端口（每个计算机都会有很多端口用于和外部网络交互）

- `path`: 资源在目标服务器上的路径

- `query`: 查询串（发给服务器的）

- `fragment`: 指向资源内部片段

---

### 工作原理

当输入url，请求会被发给DNS解析服务器

然后DNS解析服务器会根据你输入的域名，查找过后返回对应的IP给浏览器。

浏览器得到IP地址之后，就可以直接访问IP地址所对应的服务器

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
