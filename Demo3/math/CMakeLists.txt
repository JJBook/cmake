# 添加当前所有的源文件
aux_source_directory(. DIR_LIB_SRCS)

# 生成链接库
add_library(MathFunctions ${DIR_LIB_SRCS})