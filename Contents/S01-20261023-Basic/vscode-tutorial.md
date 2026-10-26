## 快捷键对照表

在开始实操前，请确认你的系统按键对应关系：

| 功能按键 | Windows / Linux | macOS |
| :--- | :--- | :--- |
| **主修饰键 (Ctrl)** | `Ctrl` | `Command (Cmd / ⌘)` |
| **副修饰键 (Alt)** | `Alt` | `Option (⌥)` |
| **功能键 (Shift)** | `Shift` | `Shift (⇧)` |

---

## 编辑技巧与光标黑魔法

> **核心思想**：写代码不要把手频繁移向鼠标，双手停在键盘上效率最高！

**实操演练区**：
请在下方代码块中练习整行操作：

```python
# [练习区 1] 请尝试：
# 1. 光标停在下面第 1 行（不要选中），直接按 Ctrl + C，然后在末尾按 Ctrl + V 粘贴
print("我要被复制一份！")

# 2. 光标停在下面这行，按 Ctrl + Shift + K 彻底删掉它：
print("这行是多余的垃圾代码，快删掉我！")

# 3. 光标停在下面这行，按 Alt + 上方向键 将它移动到注释上方：
print("把我往上移一行！")
```

---

`Alt + Click`：在任意你想插入光标的位置点击，可以同时在多个地方打字！
`Ctrl + Alt + Up / Down`：直接向上/下方延伸光标列（纵向批量对齐时极好用）。

**实操演练区**：
将下面这个列表的每个元素前后加上双引号和逗号，改造成合法数组格式：

```javascript
// [练习区 2] 
// 方式 A：按住 Alt 键，分别在 apple、banana、orange 开头点击，产生 3 个光标
// 方式 B：光标放在 apple 开头，按 Ctrl + Alt + 下方向键 两次，拉出 3 行垂直光标
// 接着输入 " 然后按 End 键（或右方向键移动到词末）输入 ", 

const fruits = [
  apple
  banana
  orange
];
```

---

**快捷键**：`Ctrl + D`
**说明**：选中当前单词后，每按一次 `Ctrl + D`，就会自动将光标扩展到下一个相同单词上，实现同时修改。

**实操演练区**：
下面的代码中 `user_name` 拼写不符合规范，要求全部同时改成 `student_name`：

```python
# [练习区 3] 
# 1. 双击选中第 1 个 user_name
# 2. 连续按下 3 次 Ctrl + D，观察所有 user_name 是否都被同时选中
# 3. 直接键盘打字输入 student_name

user_name = "张三"
print(user_name)
if user_name != "":
    print("Welcome, " + user_name)
```
