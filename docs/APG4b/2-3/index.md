# 2.03.多次元配列

[APG4bの該当ページ](https://atcoder.jp/contests/APG4b/tasks/APG4b_t){:target="_blank"}

## コメント

APG4bにも書かれていましたが、大事なのでもう一度書いておきます。

多次元配列を使う時に一番混乱しがちな部分は宣言をするところだと思います。  
2次元配列は

```cpp
vector<vector<int>> vec(10, vector<int>(5));
vec[9][4] = 0;
```

3次元配列は

```cpp
vector<vector<vector<int>>> vec(5, vector<vector<int>>(6, vector<int>(7)));
vec[4][5][6] = 0;
```

のように書きます。
1次元配列の宣言の仕方を思い出してください。

```c++
vector<型> vec(個数, 全てこれで埋める)
```

1次元配列はこのようにして宣言するのでした。すると、

- **2次元配列**は**配列**の**型**の部分が**1次元配列**になっている
- **3次元配列**は**配列**の**型**の部分が**2次元配列**になっている

ということが分かります。
多次元配列の宣言で困ったら1次元配列の宣言の仕方を思い出してみてください。

### 演習問題

- [EX18 - ゲーム大会](https://atcoder.jp/contests/apg4b/tasks/APG4b_ce){:target="_blank"}
