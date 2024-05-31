# 定义变量，SRCS 是 sources 的简写
# 通常包含 c、cpp、s、asm 后缀名的源文件列表
# 也可以包含 h 头文件，虽然头文件通常不会被编译，但有时也会在源文件列表中包含它们以便于自动化工具检测需要重新编译的源文件
SRCS = main.c print.c

main: $(SRCS)       # 定义了一个 Makefile rule，其中 target 为 main、prerequisite 为 $(SRCS) 中定义的那些文件
                    # * target 是 Makefile 的一个核心概念，通常是一个可执行文件或者库文件，通过 make target 来执行该 target，例如 make main
                    #   * 绝大多数时间，我们都将 target 命名为要生成的可执行文件或库文件的名称
                    # * main、prerequisite 是当前 target 需要先构建的文件或目标，通常是源文件
                    #   * 当前 target 依赖的文件或 target 构建完成后，当前 target 才会被构建
                    #   * 当 target 依赖的文件或 target 被修改后，当前 target 才会被重新构建（相当于缓存，对大型项目开发阶段很有帮助）
# Makefile 中需要用 <tab> 键缩进，而不是 4 个空格
	$(CC) $(SRCS) -o $@
    # CC 是 Makefile 中的一个变量，通常是 gcc 或 clang，表示编译器
    # $(SRCS) 是 Makefile 中的一个变量，表示源文件列表
    # -o $@ 表示输出文件名，通常是可执行文件或库文件
    # * $@ 是 Makefile 中的一个变量，表示当前 target 的名称，通常是可执行文件或库文件的名称

# 综上所述，当执行 make main 时，将执行：gcc main.c print.c -o main
# NOTE: 当 make 不带 target 时，默认执行 Makefile 文件中从上到下定义的第一个 target
