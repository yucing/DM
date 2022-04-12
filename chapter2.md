# chapter2 基本結構:集合、函數、序列、總和與矩陣
# chapter2-1
## 集合 set
* 無順序之物件的聚集
* 集合中的物件稱為「集合的元素( element \ member )」
* 稱集合包含( contain )他的元素
* 「a ∈ A」表示元素 a 為集合 A 的元素，亦指 a 屬於 A
* 「a ∉ A」表示元素 a 並非集合 A 的元素，亦指 a 不屬於 A

## 列舉法 roster method
* 使用「大括號 {}」包含起來
### 例子
* {a,b,c,d} : 表示一個包含 4 個元素的集合

## 集合建構式 set builder
* 一種描述集合的方式
### 例子一
* 若 O 為小於 10 之正奇數所形成的集合
1. 解 : O = {x | x 是小於 10 之正奇數}
2. 或 : O = {x∈𝐙⁺ | x 是奇數，而且 x<10}
### 例子二
* 所有正有理數所形成的集合
1. 解 : 𝐐⁺ = {x∈𝐑 | x=p/q，其中 p 與 q 為正整數}

## 重要集合
### 自然數 𝐍 natural number
* N = {0,1,2,3,...}
* 有些人不把 0 當自然數，請小心其用法
### 整數 𝐙 integer
* 𝐙 = {...,-2,-1,0,1,2,...}
### 正整數 𝐙⁺ positive integer
* 𝐙⁺ = {1,2,3,...}
### 有理數 𝐐 rational number
* 𝐐 = {p/q | p,q∈𝐙，且 q≠0}
### 實數 𝐑 real number
* 為實數的集合
### 正實數 𝐑⁺
* 為正實數的集合
### 複數 𝐂
* 為複數的集合

## 區間 intervals
1. [a,b] = {x | a≤x≤b}
2. [a,b) = {x | a≤x<b}
3. (a,b] = {x | a<x≤b}
4. (a,b) = {x | a<x<b}
### 閉區間 closed interval
* [a,b]
### 開區間 open interval
* (a,b)

## 兩集合相等 equal
* 兩集合相等，且包含相同元素 : 也就是說 A B 兩皆為集合，A B 相等且 ∀x(x∈A ↔ x∈B)，記為 A = B
* 元素的排列不重要
* 出現多次的元素，仍算一個
### 例子一
* 集合 A = {1,3,5} ,B = {5,3,1}
1. A B 皆為集合
2. A B 裡的元素相等
3. A = B
### 例子二
* 集合 A = {1,3,5} ,B = {5,5,5,5,5,3,3,3,1,1,1,1}
1. A B 皆為集合
2. A B 裡的元素相等
3. A = B

## 空集合 empty set / null set
* 記為「∅ 或 {}」
* 只包含一個元素的集合稱為「單點集 single set」

## 范氏圖 Venn diagram
* 考慮到的物件的集合以「矩形」表示，稱為「字集 universal set」
### 例子
* 畫出表示母音集合V的范氏圖
1. 矩形 U 代表字集
2. 在U裡面再畫一個圓集合 V
3. 在圓形內標出點表示 V 中的元素

![](https://github.com/yucing/DM/blob/main/picture/VD.png)

## 子集合 subset
* 集合 A 為集合 B 的子集合，且集合 A 的每一個元素都是集合 B 的元素
* 用符號「A ⊆ B」表示
### 定理
* 對所有集合 S
1. ∅ ⊆ S
2. S ⊆ S

## 真子集 proper subset
* 集合 A 為集合 B 的子集合，且 A ≠ B時
* 用符號「A ⊂ B」表示
* 也就是 ∀x(x∈A → x∈B) ∧ ∃x(x∈B ∧ x∉A)

![](https://github.com/yucing/DM/blob/main/picture/subset.png)

## 集合大小
* 若 S 為集合
* 若 S 中有 n 個相異元素，其中 n 為非負整數，我們說 S 是「有限集合 infinite set」
* n 為 S 的「基數 cardinality」，記為 |S|
* 若一個集合不是有限的，稱為「無限集合 infinite set」，Ex: 正整數集合
### 例題一
* 令 A 為所有小於10之正奇數所形成的集合
* A={1,3,5,7,9}，則 |A| = 5
### 例題二
* 令 B 為所有英文字母所形成的集合
* 則 |B| = 26
### 例題三
* 空集合中沒有元素
* 所以 |∅| = 0

## 冪集合 power set
* 一個集合 S，其冪集合是由所有 S 的子集合所形成的集合，記為「Ρ(S)」
### 例子一
* {0,1,2}的冪集合為何?
* 解 : P({0,1,2}) = {∅,{0},{1},{2},{0,1},{0,2},{1,2},{0,1,2}}
### 例子三
* 空的冪集合為何?
* 解 : P(∅) = {∅}
* 空集合的冪集合只有一個元素，就是他自己
### 例子三
* {∅}的冪集合為何?
* 解 : P({∅}) = {∅,{∅}}
* {∅}的冪集合有兩個元素

## 笛卡兒積 Cartesian product
* 若 A B 皆為集合
* A 與 B 的笛卡兒積，記為 A x B
* 是所有有序對(a,b)的集合，其中 a∈A ∧ b∈B
* A x B ={(a,b) | a∈A ∧ b∈B}
### 例子一
* A = {1,2} 和 B ={a,b,c} 的笛卡兒積為?
* 解 : A x B = {(1,a),(1,b),(1,c),(2,a),(2,b),(3,b)}
### 例子二
* A = {0,1} 和 B = {1,2} 和 C = {0,1,2} 的笛卡兒積為?
* 解 : A x B x C = {(0,1,0),(0,1,1),(0,1,2),(0,2,0),(0,2,1),(0,2,2),(1,1,0),(1,1,1),(1,1,2),(1,2,0),(1,2,1),(1,2,2)}
### 例子三
* A = {1,2}
* A² = {(1,1),(1,2),(2,1),(2,2)}
* A³ = {(1,1,1),(1,1,2),(1,2,1),(1,2,2),(2,1,1),(2,1,2),(2,2,1),(2,2,2)}

# chapter2-2
## 聯集 union
* 令 A B 皆為集合
* A 和 B 的聯集，記為「A ∪ B」
* 若一個 x 屬於集合 A 和 B 的聯集
* A ∪ B = {x | x∈A ∨ x∈B}

![](https://github.com/yucing/DM/blob/main/picture/union.png)

### 例子
* 集合{1,2,3}和集合{1,3,5}的聯集為{1,2,3,5}
* 即 : {1,2,3} ∪ {1,3,5} = {1,2,3,5}

## 交集 intersection
* 令 A B 皆為集合
* A 和 B 的交集，記為「A ∩ B」
* 若一個 x 屬於集合 A 和 B 的交集
* A ∩ B = {x | x∈A ∧ x∈B}

![](https://github.com/yucing/DM/blob/main/picture/intersection.png)

### 例子
* 集合{1,2,3}和集合{1,3,5}的交集為{1,3}
* 即 : {1,2,3} ∩ {1,3,5} = {1,3}

## 互斥 disjoint
* 兩集合的交集為空集合，稱為互斥

![](https://github.com/yucing/DM/blob/main/picture/disjoint.png)

### 例子
* A = {1,3,5,7,9}，B = {2,4,6,8,10}
* A ∩ B = ∅
* A 和 B 互斥

## 差集 difference
* 令 A B 皆為集合
* A 和 B 的差集，記為「A \ B」或「A - B」
* 若一個 x 屬於集合 A 和 B 的差集，且 x 屬於 A 不屬於 B
* A - B = {x | x∈A ∧ x∉B}

![](https://github.com/yucing/DM/blob/main/picture/difference.png)

### 例子
* 集合{1,2,3}和集合{1,3,5}的差集為{2}
* 即 : {1,2,3} - {1,3,5} = {2}

## 補集 complement
* 令 U 為字集，集合 A 的補集，記為「U - A」

![](https://github.com/yucing/DM/blob/main/picture/complement.png)

### 例子
* 令 A 為大於10之正整數所形成的集合
* A 的補集 : {1,2,3,4,5,6,7,8,9,10}

## 集合等式
### 同一律 identity laws
* A ∩ U = A
* A ∪ ∅ = A
### 支配律 domination laws
* A ∪ U = U
* A ∩ ∅ = ∅
### 冪等律 idempotent laws
* A ∩ A = A
* A ∪ A = A
### 補集律 complementation law
* 補數(補數A) = A
### 交換律 commutative laws
* A ∪ B = B ∪ A
* A ∩ B = B ∩ A
### 結合律 associative laws
* A ∩ (B ∩ C) = (A ∩ B) ∩ C
* A ∪ (B ∪ C) = (A ∪ B) ∪ C
### 分配律 distributive laws
* A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)
* A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)
### 迪摩根定律 De Morgan's laws
* 補數(A ∩ B) = 補數(A) ∪ 補數(B)
* 補數(A ∪ B) = 補數(A) ∩ 補數(B)
### 吸收律 absorption laws
* A ∪ (A ∩ B) = A
* A ∩ (A ∪ B) = A
### 補律 complement laws
* A ∪ 補數(A) = U
* A ∩ 補數(A) = ∅

## 一般化的聯集與交集
### 例題
* A = {0,2,4,6,8}，B = {0,1,2,3,4}，C = {0,3,6,9}
* A ∩ B ∩ C = {0}
* A ∪ B ∪ C = {0,1,2,3,4,6,8,9}

# chapter2-3
## 函數 function
## 定義一
* 若 A B 皆為非空集合
* 由 A 到 B 的函數是將恰巧一個 B 中的元素指定給每個 A 的元素
* 若 b 是集合 B 中唯一指定給 a (屬於 A)的元素，寫成「f(a) = b」
* 記為「A → B」
## 定義二
* 若 f 是一個由 A 到 B 的函數，也可稱 f 將 A 映射到 B
* A 為函數 f 的「定義域(domain)」
* B 為函數 f 的「對應域(codomain)」
* 若 f(a) = b，稱「b 為 a 的映象(image)，a 為 b的前象(preimage)」
* f 的值域(range)是所有 A 之元素的映象所形成之集合

![](https://github.com/yucing/DM/blob/main/picture/function.png)

### 例子
* 函數 f 將長度大於或等於 2 的位元字串，指定成此字串之最後兩個位元
* Ex : f(11010) = 10
* 函數 f之定義域為所有長度大於等於 2 之位元字串所形成的集合
* 則 對應域和值域都是集合 : {00,01,10,11}

## 實數函數 (real-valued function)
* 函數的定義域為實數集合
## 整數函數 (integer-valued function)
* 函數的定義域為整數集合

## 定義三
* f₁ 與 f₂ 為由 A 到 𝐑 的函數
* f₁+f₂ 和 f₁f₂ 也是由 A 到 𝐑 的函數
* (f₁+f₂)(x) = f₁(x)+f₂(x)
* (f₁f₂)(x) = f₁(x)f₂(x)
### 例子
* f₁ 和 f₂ 為由 𝐑 到 𝐑 的函數，其中 f₁(x) = x² 且 f₂(x) = x-x²，求 f₁+f₂ 和 f₁f₂?
* 解 : (f₁+f₂)(x) = f₁(x)+f₂(x) = x²+x-x² = x
* (f₁f₂)(x) = f₁(x)f₂(x) = -x⁴+x³

## 定義四
* 函數 f 由集合 A 對應到集合 B，S 為 A 的子集合
* 則 S 在函數 f 的映像是 B 的一個子集合
* S 在函數 f 的映像記為「f(S)」
* f(S) = {t | ∃s∈S (t = f(S))}
* 可簡單記成 f(S) = {f(s) | s∈S}
### 例子
* A = {a,b,c,d,e}，B = {1,2,3,4}，f(a)=2，f(b)=1，f(c)=4，f(d)=1，f(e)=1
* 解 : 集合 S = {b,c,d} 之映像 f(S) = {1,4}

## 一對一函數
* 稱為「一對一(one to one)」或「嵌射(injunction)」
* 對所有定義域的元素 a b，若 f(a)=f(b)，可推論 a=b
### 例子一
* 判斷由{a,b,c,d}對應到{1,2,3,4,5}，定義為 f(a)=4, f(b)=5, f(c)=1, f(d)=3，畔對函數 f 是否為一對一
* 解 : 是，參考下圖

![](https://github.com/yucing/DM/blob/main/picture/oto.png)

### 例子二
* 判斷整數集合對應到整數集合的函數 f(x)=x²，是否為一對一 ?
* 解 : 否，f(-1)=f(1)=1，-1≠1

## 映成函數
* 稱為「映成(onto)」或「蓋射(surhection)」
* 對每一個元素 b∈B，都存在一個元素 a∈A，使得 f(a)=b
### 例子一
* 另 f 為由{a,b,c,d}對應到{1,2,3}的函數，定義 f(a)=3, f(b)=2, f(c)=1, f(d)=3，f 是否為映成函數 ?
* 解 : 是，因為所有對應域的元素都是某定義域元素的映象

![](https://github.com/yucing/DM/blob/main/picture/surjection.png)

### 例子二
* 由整數集合對應到整數集合的函數 f(x)=x² 是否為映成函數 ?
* 解 : 否，找不到整數 x 使 x²=-1

## 一對一對應關係
* 既為一對一，也為映射，稱為一對一對應關係(one-to-one correspondence)

## 補充
* 假設 f:A → B
### 證明 f 為嵌射
* 對任意 x,y ∈ A，若 f(x)=f(y)，則 x=y

### 證明 f 不為嵌射
* 找出特定對任意 x,y ∈ A，使 x≠y，但 f(x)=f(y)
### 證明 f 為蓋射
* 考慮任意元素 y ∈ B，找出元素 x ∈ A，使 f(x)=y
### 證明 f 不為蓋射
* 找出特定元素 y ∈ B，使 x ∈ A，但 f(x)≠y