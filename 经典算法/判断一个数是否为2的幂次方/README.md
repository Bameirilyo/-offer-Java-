# 判断一个数是否为2的幂次方


## 思路：
将2的幂次方写成二进制形式后：二进制中只有一个1，并且1后面跟了n个0。如果将这个数减去1后会发现，仅有的那个1会变为0，而原来的那n个0会变为1；因此将原来的数与减去1后的数字进行与运算后会发现为零。 


```Java
(n & (n - 1) ) == 0;  
```
