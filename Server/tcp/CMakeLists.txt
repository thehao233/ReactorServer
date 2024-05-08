cmake_minimum_required(VERSION 3.16)
project(tcp)
set(CMAKE_CXX_STANDARD 17)

# 取出当前目录中所有的源文件, 存储到一个变量中
aux_source_directory(./ SRC)
# 把源文件制作成静态库文件
add_library(tcp STATIC ${SRC})
#add_library(tcp STATIC
#        TcpConnection.cpp
#        TcpConnection.h
#        TcpServer.cpp
#        TcpServer.h
#)