在Enclave中使用ECALL函数直接计算两个整数之间的所有整数的累加和（包括这两个整数）

修改文件：
- Enclave.edl：定义接口MyAccum，删除ocall的接口以及相关函数导入
- Enclave.cpp：定义可信函数MyAccum
- App.cpp：在main函数中调用MyAccum并打印返回值
- App.h：删除与Edger8rSyntax和TrustedLibrary相关的函数声明
- Makefile：修改App_Cpp_Files、Enclave_Cpp_Files
