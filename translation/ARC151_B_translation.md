## 题意 

已知一个 $(1,2,...,N)$ 的置换 $P=(P_1,P_2,...,P_N)$。

求有多少个长度为 $N$ 的序列 $A=(A_1,A_2,...,A_N)$ 满足以下条件，答案对 $998244353$ 取模。

- 对于 $1\le i\le N$，满足 $1\le A_i\le M$。
- $A$ 的字典序比 $(A_{P_1},A_{P_2},...,A_{P_N})$ 小。

## 数据范围

- $1\le N\le 2\times 10^5$
- $1\le M\le 10^9$
- $1\le P_i\le N$
- $P_i$ 两两不同。

## 输入格式

第一行两个数 $N,M$。

第二行 $N$ 个数表示 $P$。

## 输出格式

一行一个数，表示答案。

## 样例

### 样例输入1

```
4 2
4 1 3 2
```

### 样例输出1

```
6
```

### 样例解释1

满足条件的 $A$ 有 $(1,1,1,2), (1, 1, 2, 2), (1, 2, 1, 2), (1, 2, 2, 2), (2, 1, 1, 2),(2, 1, 2, 2)$。

比如对于 $A=(1,1,1,2)$，$(A_{P_1},A_{P_2},A_{P_3},A_{P_4})=(2,1,1,1)$，$A$ 的字典序比后者小。

### 样例输入2

```
1 1
1
```

### 样例输出2

```
0
```

### 样例输入3

```
20 100000
11 15 3 20 17 6 1 9 5 19 10 16 7 8 12 2 18 14 4 13
```

### 样例输出3

```
55365742
```