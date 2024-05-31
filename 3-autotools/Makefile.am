# Primaries: PROGRAMS, LIBRARIES, LTLIBRARIES, DATA, HEADERS , SCRIPTS, MANS...

# Building a program:
# * Primary: PROGRAMS
# * Destinations: bin, sbin, libexec, pkglibexec

# bin_PROGRAMS 是一个标准的 Automake 变量，用于列出项目中要生成的二进制文件（可执行程序）
bin_PROGRAMS = helloworld  # 需要生成一个规则来构建一个叫 helloworld 的程序

# _SOURCES 后缀用于定义与主目标（该例子中为 helloworld）相关的源文件列表
helloworld_SOURCES = helloworld.c

# 定义预处理器标志
helloworld_CPPFLAGS = -DPWET

# 指定了 C 编译器标志
# -Wall 让编译器显示所有的警告信息
helloworld_CFLAGS = -Wall
