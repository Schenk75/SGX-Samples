向Enclave可信函数传递参数，并进行参数字符串拷贝

修改文件：
- Enclave.edl：定义接口StrCpy，删除ocall的接口以及相关函数导入
- Enclave.cpp：定义可信函数StrCpy，删除可信的printf函数
- App.cpp：在main函数中调用StrCpy并打印
- App.h：删除与Edger8rSyntax和TrustedLibrary相关的函数声明
- Makefile：修改App_Cpp_Files、Enclave_Cpp_Files
