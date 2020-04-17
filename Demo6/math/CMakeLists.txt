# 查找当前目录下的所有源文件
# 并将名称保存到DIR_LIB_SRCS
aux_source_directory(. DIR_LIB_SRCS)

# 指定生成 MathFunctions 链接库
add_library(MathFunctions ${DIR_LIB_SRCS})

# 指定生辰 MathFunctions 的库安装路径
install(TARGET MathFunctions DESTINATION lib)
install(FILES MathFunctions DESTINATION include)