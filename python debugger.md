## 检视当前状态

- 输出变量值：p x
- 显示调用帧：w
- 当前位置前后源代码（11行）：l or lst, 再次输入显示后11行，输入l.返回当前位置
- 当前函数全部代码：ll
- 调整当前帧：u or d

## 控制程序运行

- 运行一行：n or next
- 进入函数：s or step
- 拿到返回值：retval
- 运行，直到行数比现在大：until
- 运行，直到行数比10大：until 10
- 运行直到函数返回：r or return
- 跑完：c
- 当前文件第五行设置断点：b 5
- 列出所有breakpoint：break
- 删除断点（1个 or 全部）：clear 1 or clear
- 退出调试：q or quit