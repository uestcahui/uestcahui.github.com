# 给定一个int 数，判读是否是2的幂的问题

> 今天一点资讯第一次电话面试，这是其中一道算法题

以前做过一个笔试题：

```c++
int value=xxx;
int i =0;
while(value){
  value= value & (value-1);
  i++;
}
//这其实是在求value的二进制表示中bits中为1的个数
```

判读一个数是不是2的幂，就是看这个数中的一个个数是否为1 ： 2^x 幂对应二进制数是100...00 (x-1个零)

所以答案是：

```c++
cout<<(value) & (vlaue-1)? "yes":"no"<<endl;
```

