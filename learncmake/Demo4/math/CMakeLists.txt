#查找当前目录下的所有文件并将名称保存到DIR_LIB_SRC
aux_source_directory(. DIR_LIB_SRC)

# 添加连接库
add_library(MathFunctions ${DIR_LIB_SRC})
