cmake_minimum_required(VERSION 3.16)
project(reactor)
set(CMAKE_CXX_STANDARD 17)

# 取出当前目录中所有的源文件, 存储到一个变量中
aux_source_directory(./ SRC)
# 把源文件制作成静态库文件
add_library(reactor STATIC ${SRC})
# 生成的静态库文件全名 libhttp.a
# 生成的动态库文件全名 libhttp.so