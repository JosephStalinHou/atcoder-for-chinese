### 题意 

构造一个长度为 $N$ 的只包含 $01$ 的字符串 $s$，需要满足 $M$ 个条件，第 $i$ 个条件给出两个数 $L_i,R_i(1\le L_i < R_i \le N)$，表示$s$ 在 $[L_i,R_i]$ 位置上的 $0$ 的个数和 $1$ 的个数相同。

构造满足条件的，字典序最小的 $s$，可以证明一定有解。

### 数据范围

- $2\le N\le 10^6$
- $1\le M \le 2\times 10^5$
- $1\le L_i < R_i \le N$
- $(R_i-L_i+1) \equiv 0 \pmod 2$

---

### 输入格式

第一行两个数 $N,M$。

接下来 $M$ 行，每行两个数 $L_i,R_i$ 表示一个限制条件。

### 输出格式

输出构造的字符串。

---

### 样例输入1

```
4 2
1 2
3 4
```

### 样例输出1

```
0101
```

---

### 样例输入2

```
6 2
1 4
3 6
```

### 样例输出2

```
001100
```

---

### 样例输入3

```
20 10
6 17
2 3
14 19
5 14
10 15
7 20
10 19
3 20
6 9
7 12
```

### 样例输出3

```
00100100101101001011
```