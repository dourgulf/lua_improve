lua_improve
===========

改进LUA 的string.format，支持参数位置的格式化字符串

基于LUA5.2.1版本的源文件的lstrlib.c 修改其中的str_format 和scanformat两个方法实现的方案。
测试用例：
print(string.format("%10$10.10d, %9$09d, %8$08d, %7$07d, %6$06d, %5$05d, %4$04d, %3$03d, %2$02d, %1$1d", 1, 2, 3, 4, 5, 6, 7, 8, 9, 10))
print(string.format("%10.10d, %09d, %08d, %07d, %06d, %05d, %04d, %03d, %02d, %1d", 1, 2, 3, 4, 5, 6, 7, 8, 9, 10))

