1.

![image-20220503133732790](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503133732790.png)

![image-20220503133745779](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503133745779.png)

**思路**

倒着想，若b中出现连续的数字，那后面的这些数字一定是由前面的位置转移过来的，将能转移的数字的数量存下来，扫一遍a，遇到不匹配的情况就从计数器里取一个，若存在不匹配并且库存不够时就说明满足不了，输出NO

2.

![image-20220503133951761](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503133951761.png)

![image-20220503134001551](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503134001551.png)

**思路**

无解和无穷的情况十分容易判断，这里就讲一讲有有限解的情况，已知c的公差和b的公差，若要使c的每一项都在a中出现，前提条件一定是a的公差能整除c的公差，接下来考虑a和b除c外没有重复的元素，那就是要求a和b从同一个起点开始，相同的位置在c1+d或在其之后，d为c的公差，也即是说lcm(d1,d2)>=d才行，结合两者，根号n复杂度分解质因数，用数组存下来就行了

3.

![image-20220503134349772](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503134349772.png)

![image-20220503134400709](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503134400709.png)

**思路**

完全背包

4.

![image-20220503134642711](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503134642711.png)

![image-20220503134656608](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503134656608.png)

**思路**

我们发现除了s>0的情况，另外两种情况的最优解一定是长度为1的时候，所以我们只要考虑s>0的情况，dp[i]表示到当前位置为止的最大值。

5.

![image-20220503135140900](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135140900.png)

![image-20220503135151363](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135151363.png)

**思路**

有向图的强连通分量，缩点之后为拓扑图，当且仅当只有一个强连通分量为终点时有解

6.

![image-20220503135307909](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135307909.png)

![image-20220503135318582](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135318582.png)

**思路**

有向图的强连通分量，第一个问题的答案是起点的个数(入度为0)，第二个问题转化一下就是添加多少条边，能使一个图变成强连通的，答案是max(p,q)，p为起点(入度为0)的数量，q为终点,(出度为0)的数量

7.

![image-20220503135622863](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135622863.png)

![image-20220503135629865](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503135629865.png)

**思路**

对缩点之后的强连通分量建新图，可以发现他是个拓扑图，并且dfn值越小越靠后，于是可以用dp来求解，f[i]表示大小，g[i]表示数量

8.

![image-20220503140044444](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140044444.png)

![image-20220503140051963](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140051963.png)

**思路**

差分约束+dfs版spfa

9.

![image-20220503140126601](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140126601.png)

![image-20220503140135091](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140135091.png)

**思路**

无向图的边双连通分量，将一个图变成边双连通最少需要加的边的数量是ceil(叶子结点数/2.0)

10.

![image-20220503140406252](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140406252.png)

![image-20220503140413650](C:\Users\fyq20020501\AppData\Roaming\Typora\typora-user-images\image-20220503140413650.png)

**思路**

完全背包求解最大无关向量组，对于一种货币，若其能被比他小的货币表达出来，则这种货币是多余的，利用完全背包判断能否被表达即可

