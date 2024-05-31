# 项目描述
AC_INIT([helloworld], [1.0], [helloworld@nju.edu.cn]) # 项目名称，版本，维护者

# AutoMake 的初始化参数
# * -Wall -Werror 表示编译时，如果有警告，则编译失败
# * foreign 表示使用 automake 的 foreign 功能
AM_INIT_AUTOMAKE([-Wall -Werror foreign])

# 检查 C 编译器
AC_PROG_CC

# 生成一个包含 options 的 config.h 文件
AC_CONFIG_HEADERS([config.h])

# 要生成 Makefile 的列表
AC_CONFIG_FILES([
    Makefile
])

# 生成 Makefile
AC_OUTPUT
