# log函数

## log函数介绍

1. `log()`：以e为底的对数函数
2. `log10()`：以10为底的对数函数
3. `log(n)/log(m)`：以m为底求log(n)

## 补充：

1. $e=2.71828···$
2. `exp(n)`：e的n次方
3. `exp2(n)`：2的n次方，返回double型数据

> 注意：函数返回值为float或者double形式时，和整数进行比较要将float、double强制转换为int或long long，即使它是float、double型的整数
>
> 比如都是表示2的n次方的整数：`exp2(n)`与`(1ll<<n)`，前者为double型，后者为ll型，进行比较时如果为对前者进行强制类型转换，可能会出错
>
> ```c++
> exp2(60)==(1ll<<n)-1;//前者比后者大1，但是结果为1（错误）
> (ll)exp2(60)==(1ll<<n)-1;//结果为0（正确）
> ```
