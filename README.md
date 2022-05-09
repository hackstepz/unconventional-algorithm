# 非常规算法
> 常见算法包找不到的，工作里面可能会涉及到的算法哈，无依赖，可以直接拷贝.java文件使用

## Linux cksum 命令兼容算法 

因为Linux cksum命令默认执行不同于常规CRC32算法，因此Cksum.java实现了兼容，

常规用法
- 通过readFile方法读取文件计算校验值
- 通过getValue方法进行输出

```shell
CRC (via Java's CRC32 library)  = 4124803878
CRC (via Java's Cksum)  = 190271139
CRC (via Linux cksum)  = 190271139 92992 xxx.xlsx
```