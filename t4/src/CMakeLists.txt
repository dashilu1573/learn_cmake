#引入非系统标注的头文件搜索路径
INCLUDE_DIRECTORIES(/Users/luyafei/GitHub/include/hello)
ADD_EXECUTABLE(main main.c)
#添加非系统标准的共享库搜索路径
LINK_DIRECTORIES(/Users/luyafei/GitHub/lib)
TARGET_LINK_LIBRARIES(main libhello)
ADD_EXECUTABLE(main main.c)
