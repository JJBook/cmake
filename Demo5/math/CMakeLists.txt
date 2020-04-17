# 查找当前目录下的所有源文件
# 并将名称保存到DIR_LIB_SRCS
aux_source_directory(. DIRLIB_SRCS)

# 指定生成 MathFunctions 链接库
add_library(MathFunctions ${DIRLIB_SRCS})

# 指定生辰 MathFunctions 的库安装路径
install(TARGETS MathFunctions DESTINATION lib)
install(FILES MathFunctions.h DESTINATION include)