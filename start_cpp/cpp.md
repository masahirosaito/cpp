# 1. 基礎
## 1.1 プログラムの基本形
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
}
```

## 1.2 出力とコメント
### 出力
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    // 通常の出力
    cout << "Hello, world!" << endl;

    // 複数の出力
    cout << "a";
    cout << "b" << endl;
    cout << "c" << "d" << endl;

    // 数値の出力
    cout << 2525 << endl;
}
```

## 1.3 四則演算
### 四則演算
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    cout << 1 + 1 << endl; // 2
    cout << 3 - 4 << endl; // -1
    cout << 2 * 3 << endl; // 6
    cout << 7 / 3 << endl; // 2
}
```
### 剰余演算
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    cout << 7 % 3 << endl; // 1
    cout << 4 % 5 << endl; // 4
}
```

## 1.4 変数と型
### 変数の初期化
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    // 基本
    int name_1;
    name_1 = 10

    // 宣言 + 代入
    int name_2 = 10

    // 複数の変数を同時宣言
    int a = 10, b = 5;
}
```
### 型
|型|書き込むデータの種類|
|:---|:---|
|int|整数|
|double|少数|
|string|文字列|

## 1.5 入力
### 入力
```cpp
#include <bits/stdc++.h>
using namespace std;

int main()
{
    int a;
    int x, y, z;
    cin >> a; //基本
    cin >> x >> y >> z; //つなげて入力
    cout << a * 10 << endl;
    cout << x * y * z << endl;
}
```

## 1.6 if文・比較演算子・論理演算子
### if文
```cpp 
if (条件式1) {
    処理1
}
else if (条件式2) {
    処理2
}
else {
    処理3
}
```
### 比較演算子
|演算子|意味|
|:---|:---|
|x == y|xとyは等しい|
|x != y|xとyは等しくない|
|x > y|xはyより大きい|
|x < y|xはyより小さい|
|x >= y|xはy以上|
|x <= y|xはy以下|
### 論理演算子
|演算子|意味|真になる時|
|:---|:---|:---|
|!(条件式)|条件式の結果の反転|条件式が偽|
|条件式1 && 条件式2|条件式1が真 かつ 条件式2が真|条件式1と条件式2のどちらも真|
|条件式1 \|\| 条件式2|条件式1が真 または 条件式2が真|条件式1と条件式2の少なくとも片方が真|

## 1.7 複合代入演算子
### 複合代入演算子
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  int x = 5, a = 5, b = 3, c = 4, d = 5;
  x += 1 + 2; // x = x + (1 + 2)
  a -= 2; // a = a - 2
  b *= 1 + 2; // b = b * (1 + 2)
  c /= 2; // c = c / 2
  d %= 2; // d = d % 2

  cout << x << endl; // 8
  cout << a << endl; // 3
  cout << b << endl; // 9
  cout << c << endl; // 2
  cout << d << endl; // 1
}
```
### インクリメントとデクリメント
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  int x = 5;
  x++;
  cout << x << endl; // 6

  int y = 5;
  y--;
  cout << y << endl; // 4
}
```

## 1.8 繰り返し処理
### while文
```cpp
while (条件式) {
    処理
}
```

### for文
```cpp
for (int i = 0; i < N; i++) {
    処理
}
```
- **break文**を使うとループを途中で抜けられる。  
- **continue文**を使うと後の処理を飛ばして次のループへいける。

## 1.9 文字列と文字
### 文字列
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string str1, str2; // string型を使う
  cin >> str1;
  str2 = ", world!";

  cout << str1 << str2 << endl;
}
```
### 文字列の長さ
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string str = "Hello";
  cout << str.size() << endl; //文字列変数.size()
}
```
### *i*番目の文字
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string str = "hello";
  cout << str.at(0) << endl; // h //文字列.at()
  cout << str.at(4) << endl; // o //文字列.at()
}
```

### 文字型
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  char c = 'a'; // char型を使う, ''で囲う
  cout << c << endl; // a
}
```

### 文字列の比較
|演算子|意味|
|:---|:---|
|==|2つの文字列が完全に一致している|
|!=|2つの文字列に違いがある|
|<, <=, >, >=|辞書順による比較|

### 文字列の連結
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string hello = "Hello";

  // +演算子による連結
  cout << hello + ", world!" << endl; // Hello, world!

  // +=演算子による連結
  hello += ", AtCoder!";
  cout << hello << endl; // Hello, AtCoder!
}
```

### 文字列と文字の連結
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string str = "Hello";

  char c = str.at(0);
  cout << str + c << endl; // HelloH
}
```

### char型の変数への入力
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  char a, b;
  cin >> a >> b;

  cout << a << endl;
  cout << b << endl;
}
```

### 行単位での入力
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  string s, t;
  getline(cin, s); // 変数sで入力を一行受け取る
  getline(cin, t); // 変数tで入力を一行受け取る

  cout << "一行目 " << s << endl;
  cout << "二行目 " << t << endl;
}
```

## 1.10 配列
### 宣言と代入
```cpp
#include <bits/stdc++.h>
using namespace std;
 
int main() { 
  // {0, 0, 0}で初期化
  vector<int> vec_1(3); // vector<型> 配列名(要素数);
  for (int i = 0, i < 3, i++) {
      cin >> vec_1.at(i); // atで入力
  }

  // {1, 1, 1}で初期化
  vector<int> vec_2(3, 1); // vector<型> 配列名(要素数, 初期値);

  // {1, 2, 3}で初期化
  vector<int> vec_3 = {1, 2, 3};

  // 初期化2
  vector<int> vec = vector<int>(100, 2);
}
```

### 要素の追加
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  vector<int> vec = { 1, 2, 3 };

  vec.push_back(10); // 末尾に10を追加

  for (int i = 0; i < vec.size(); i++) {
    cout << vec.at(i) << endl;
  }
}
```

### 要素の削除
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
  vector<int> vec = { 1, 2, 3 };

  vec.pop_back(); // 末尾の要素を削除

  // vecの全要素を出力
  for (int i = 0; i < vec.size(); i++) {
    cout << vec.at(i) << endl;
  }
}
```

## 1.11 STL関数
### min関数
2つの引数のうち、小さい方の値を返す。  
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int answer = min(10, 5);

    cout << answer << endl; // 5
}
```

### max関数
2つの引数のうち、大きい方の値を返す。  
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int answer = max(10, 5);

    cout << answer << endl; // 10
}
```

### swap関数
2つの引数の値を交換する。  
```cpp
#include <bits/stdc++.h>
using namespace std;
 
int main() {
    int a = 10, b = 5;
 
    swap(a, b);
 
    cout << a << endl; // 5
    cout << b << endl; // 10
}
```

### reverse関数
配列の要素の並びを逆にする。
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    vector<int> vec = {1, 5, 3};
    reverse(vec.begin(), vec.end()); // {3, 5, 1}

    for (int i = 0; i < vec.size(); i++) {
        cout << vec.at(i) << endl;
    }
}
```

### sort関数
配列の要素を小さい順に並び替えることができる。
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    vector<int> vec = {2, 5, 2, 1};
    sort(vec.begin(), vec.end()); // {1, 2, 2, 5}

    for (int i = 0; i < vec.size(); i++) {
        cout << vec.at(i) << endl;
    }
}
```

### sort関数 + reverse関数
配列の要素を大きい順に並び替えることができる。
```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    vector<int> vec = {2, 5, 2, 1};
    sort(vec.begin(), vec.end()); // {1, 2, 2, 5}
    reverse(vec.begin(), vec.end()); // {5, 2, 2, 1}

    for (int i = 0; i < vec.size(); i++) {
        cout << vec.at(i) << endl;
    }
}
```

## 1.12 関数
### 関数の定義
```cpp
返り値の型 関数名(引数1の型 引数1の名前, 引数2の型 引数2の名前) {
    処理
    return 返り値;
}
```
- 関数は宣言した行より後でしか呼び出せない。  

### プロトタイプ宣言
「関数の名前」と「引数の返り値の型」だけ先に宣言すること。  
関数を定義する前に呼び出すことができるようになる。
```cpp
#include <bits/stdc++.h>
using namespace std;

// プロトタイプ宣言
void hello();

int main() {
  // プロトタイプ宣言をしたので呼び出せる
  hello();
}

void hello() {
  cout << "hello!" << endl;
  return;
}
```

### 関数のオーバーロード
- 「引数の型」または「引数の数」が異なる場合は、同じ名前の関数を定義することができます。
- 引数の型や引数の数に応じて、呼び出される関数が変わる。

# 2. 複雑な計算処理の書き方
##