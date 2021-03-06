
#数据结构_算法复杂度

##基本概念：
**算法复杂度**
	包括时间复杂度、空间复杂度。复杂度表示算法程序运行对时间、空间的需求，是程序效率的一种描述。
	
 **大O表示法**
	算法的复杂度计算依赖于操作（operation）次数；
	O(5) = O(1)
	O(2n+1) = O(n)
	O(2n^2+1) = O(n^2)
	O(n^3+n^2+1) = O(n^3)
	时间复杂度主要包括了：线性阶、对数据、平方阶

##算法复杂度的计算：
实例1：O(n)

``` c
for(int i = 0; i < n; i++)
{
	// O(1)
}
```

实例2：O(log2(n))

``` cpp
while(i<n)
{
	// O(1)
	i * = 2;
}

```

实例3：O(n^2)

``` c
for(int i = 0; i < n; i++)
	for(int j = 0; j < n; j++)
	{
		// O(1)
	}
```

实例 4

``` c
for(int i = 0; i < n; i++)
	for(int j = i; j < n; j++)
	{
		//O(1)
	}
```
算术：
	i				  j
	0				n
	1				n-1
	... 			...
	n-1			  1
	算法操作次数：1+...+n=1/2*(n^2 + 1) 
	算法复杂度 = O(n^2)
	
