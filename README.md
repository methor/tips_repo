## GDB调试

### 在GDB中获取进程工作目录
直接用pwd得到的是GDB进程的工作目录。可以通过`info proc`得到被调试进程的工作目录。<https://sourceware.org/gdb/onlinedocs/gdb/Working-Directory.html>

### 设置条件端点
首先设置普通端点，会被赋予一个端点号，如`breapoint 1`。再设置条件断点`condition 1 *expr*`。