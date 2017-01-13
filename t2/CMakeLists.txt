PROJECT (HELLO)
#ADD_SUBDIRECTORY指令用于向当前工程添加存放源文件的子目录,并可以指定中间二进制和目标二进制存放的位置
ADD_SUBDIRECTORY(src bin)
#安装COPYRIGHT/README
INSTALL(FILES COPYRIGHT README DESTINATION share/doc/cmake/t2)
#安装runhello.sh
INSTALL(PROGRAMS runhello.sh DESTINATION bin)
