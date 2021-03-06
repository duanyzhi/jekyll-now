---
layout: post
title: Sort Algorithms
---

# 常用的几个排序算法详细解析



# 各种排序算法复杂度:smile:

 算法名称|复杂度       
 -------------- | ------------ 
 快速排序| **O**(nlogn) 
 插入排序| O({n}^2)     
 二分法插入排序| O(logn)      





# 快速排序

12，15， 1， 18， 2， 35， 30， 11

以12为基准排一次

法一： 12不动，从左找比12大的，从右找比12小的，交换

           12， 11，1，18，2，35，30，15
    
          循环上面找法直到左右两个索引相遇：
    
          12， 11，1，2，18，35，30，15
    
          把12放到中间：
    
         11，1，2，12，18，35，30，15

法二：一直交换12，从右找比12小的和12交换，在从左找比12大的在交换，再从右找比12小的交换，一直下去

       11，15，1，18，2，35，30，12
    
       11，12，1，18，2，35，30，15
    
       11，2，1，18，12，35，30，15
    
       11，2，1，12，18，35，30，15



# 插入排序

# 希尔排序

# 选择排序

# 冒泡排序

# 二分法插入排序

二分法插入排序是假设已经排好了几个数，那么新的数字怎么插入其中。或者二分法查找一个数组中有没有某个数也是一个意思。方法就是左右两边分别一个指针，然后取两个数的中间值，把中间值和比较的值进行比较，然后通过大小关系就可以确定要比较的数是在中间值的左边还是右边。这样可以把比较的序列缩小一半。假设数据长度为N。那么第二次比较长度为N/2，第三次为N/2/2，第k次为N/(2^k^),最差的时候第k次才找到，此时只剩下一个元素，最后长度为 1，即:
$$
\frac{N}{2^k}=1
$$
则根据:
$$
a^b=c
$$

$$
loga^c=b
$$

计算次数/复杂度: k = log(N)

