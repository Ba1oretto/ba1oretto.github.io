---
title: Ubuntu防火墙
tags:
  - 日常
---

# ubuntu防火墙指令

```bash
Commands:
 enable                          enables the firewall
 disable                         disables the firewall
 default ARG                     set default policy
 logging LEVEL                   set logging to LEVEL
 allow ARGS                      add allow rule
 deny ARGS                       add deny rule
 reject ARGS                     add reject rule
 limit ARGS                      add limit rule
 delete RULE|NUM                 delete RULE
 insert NUM RULE                 insert RULE at NUM
 route RULE                      add route RULE
 route delete RULE|NUM           delete route RULE
 route insert NUM RULE           insert route RULE at NUM
 reload                          reload firewall
 reset                           reset firewall
 status                          show firewall status
 status numbered                 show firewall status as numbered list of RULES
 status verbose                  show verbose firewall status
 show ARG                        show firewall report
 version                         display version information
```

# 用法

```bash
ufw command
```

***

### 一般的服务器是默认关闭防火墙的，所以先要开启

```bash
ufw enable
```

可能会提示**Command may disrupt existing ssh connections. Proceed with operation (y/n)?**，不用管直接***y***+***回车***

显示**Firewall is active and enabled on system startup**代表开启成功

### 然后查看防火墙状态

```bash
ufw status
```

会列出当前被记录的端口的***状态***以及***被准许访问的IP***(anywhere表示任何ip都可访问)

***

### 开放你想要的端口(ARGS替换成你要开放的端口号)

```bash
ufw allow ARGS
```

比如

```bash
ufw allow 11451
```

- 端口范围为**0-65535** (以后会开新栏专门写)
    - 一般用到的是**1-65535**
    - 其中**0**不使用
    - **1-1023**为公认端口，用不了
    - **1024-49151**为注册端口，尽量别用
    - **49152–65535为动态，专用或临时端口，可放心分配**

资料来自[维基百科](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)

### 放行后重新加载防火墙

```bash
ufw reload
```

### 然后再次查看防火墙状态，检查端口是否被放行
