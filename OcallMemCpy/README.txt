在Enclave中向Ocall传递参数，并对参数字符串拷贝

修改文件：
- Enclave.edl：定义接口ecall_memcpy和ocall_strcpy
- Enclave.cpp：定义可信函数ecall_memcpy
- App.cpp：定义ocall_strcpy，并在main函数中调用ecall_memcpy
