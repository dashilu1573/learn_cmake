PROJECT (HELLO)
#SET指令可以用来显式的定义变量
#如果有多个源文件,也可以定义成: SET(SRC_LIST main.c t1.c t2.c)
SET(SRC_LIST main.c)
#变量使用${}方式取
#CMake预定义了 PROJECT_BINARY_DIR 和 PROJECT_SOURCE_DIR
#MESSAGE这个指令用于向终端输出用户定义的信息
MESSAGE(STATUS "This is BINARY dir ${PROJECT_BINARY_DIR}")
MESSAGE(STATUS "This is SOURCE dir ${PROJECT_SOURCE_DIR}")
#可执行文件
ADD_EXECUTABLE(hello ${SRC_LIST})
