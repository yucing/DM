# chapter1 邏輯與證明

# chapter1-1
## 命題 proposition
* 有真假值的「述句 ( declaractive sentence )」
### 為命題的例子
* 1 + 1 = 2 ---> 真
* 2 + 2 = 3 ---> 假
### 非命題的例子
* 天氣如何 ? ---> 疑問句
* x + 1 = 2 ---> 無真假

## 命題變數 propositional variable
* 述言變數 statement variable
* 代表命題的變數
* 真 : T，假 : F
* 將原有命題用邏輯運算符號形成的新命題，稱之為 「複合命題 ( compound proposition )」
### 例如
* 「我今天早餐吃吐司」的否定句 ---> 我今天早餐沒有吃吐司

## 命題 : 連言 ( conjuntion )
* 令 p 和 q 為任兩命題，p 和 q 的連言為 「p 和 q」
* 以 「 p ∧ q 」 表示

p | q | p ∧ q
--|--|-------
T | T|  T
T | F|  F
F | T|  F
F | F|  F

### 例如
* p : 我今天早餐吃了薯餅蛋餅
* q : 我今天早餐喝了鮮奶茶
* p ∧ q : 我今天早餐吃了薯餅蛋餅，而且喝了一杯鮮奶茶

## 命題 : 選言 ( disjuntion )
* 令 p 和 q 為任兩命題，p 和 q 的選言為 「p 或 q」
* 以 「 p ∨ q 」 表示
* 有 「兼容性 (inclusive)」或 「互斥性 (exclusive)」

p | q | p ∨ q
--|--|-------
T | T|  T
T | F|  T
F | T|  T
F | F|  F

### 例如
* p : 我今天早餐想吃薯餅蛋餅
* q : 我今天早餐想吃薯餅吐司
* p ∨ q : 我今天早餐想吃薯餅蛋餅，或吃薯餅吐司
### 兼容性
* 修過 「張老師」 或  「陳老師」 課的學生可以修這門課
### 互斥性
* 主菜附贈湯或沙拉 ---> 只能選 「湯」 或 「沙拉」 其中一個

## 命題 : 互斥 ( exclusive )
* 令 p 和 q 為任兩命題，以 「p ⊕ q」 表示
* 恰為一真一假時， p ⊕ q 為真

p | q | p ⊕ q
--|--|-------
T | T|  F
T | F|  T
F | T|  T
F | F|  F

## 條件句 Conditional Statements
* 蘊含 ( implications )
* 令 p 和 q 為任兩命題，以 「 p → q 」 表示，代表 「如果 p，則 q」 

p | q | p → q
--|--|-------
T | T|  T
T | F|  F
F | T|  T
F | F|  T

### 例如
* p : 我認真讀書
* q : 我會有好工作
* p → q : 我如果認真讀書，就會有好工作
### 逆命題 converse
* 「q → p」 為 「p → q」 的逆命題
### 反命題 inverse
* 「¬p → ¬q」 為 「p → q」 的反命題
### 質位互換命題 contrapositive
* 「¬q → ¬p」 為 「p → q」 的逆命題

p | q | ¬p | ¬q | p → q | ¬q → ¬p
--|--|-------|-------|-------|-------
T | T | F | F | T | T
T | F | F | T | F | F
F | T | T | F | T | T
F | F | T | T | T | T

## 命題 : 雙條件句
* 雙蘊含 ( bi-implications)
* 令 p 和 q 為任兩命題，以 「p ↔ q」 表示
* 具有相同質時， p ↔ q 為真

p | q | p ↔ q
--|--|-------
T | T|  T
T | F|  F
F | T|  F
F | F|  T

### 例如
* p : 我可以搭飛機
* q : 我買了機票
* p ↔ q : 我可以搭飛機，因為我買了機票

# chapter1-2
## 日常語言轉換邏輯符號
### 例子一
* 「只有在主修電腦或不是大一生時，才能使用學校網路」
* p : 主修電腦
* q : 大一生
* r : 使用學校網路
* 轉換---> r → ( p ∨ ¬q )
### 例子二
* 「16歲以下和孕婦，不能搭乘雲霄飛車」
* p : 16歲以下
* q : 孕婦
* r : 搭乘雲霄飛車
* 轉換---> ( p ∧ q ) → ¬r

## 一致性 consistent
* 以下情形可同時為真時，就有一致性
### 例子
1. 「此訊息儲存於緩衝記憶體或被重新傳送」
2. 「此訊息並未儲存於緩衝記憶體」
3. 「如果此訊息儲存於緩衝記憶體，則他將被重新傳送」
* p : 訊息儲存於緩衝記憶體
* q : 訊息被重新傳送
* 1 : p ∨ q
* 2 : ¬p
* 3 : p → q
* 可同時為真，因此有一致性

p | q | ¬p | p ∨ q | p → q 
--|--|-------|-------|-------|
F | T | T | T | T

# chapter1-3
## 等值命題
* 任複合命題，永遠為真時，稱為 「恆真句」 或 「套套邏輯 ( tautology )」
* 永遠為假時，稱為「矛盾句 ( contradiction )」 
* 非恆真句或矛盾句之複合命題，稱為「適真句 ( contingency )」

### 例子

p | p ∨ ¬p | p ∧ ¬p 
--|--|-------
T | T |  F
F | T |  F

* p ∨ ¬p : 恆真句
* p ∧ ¬p : 矛盾句


## 邏輯上的等值
* 若 p ↔ q 為一個恆真句，複合命題 p 和 q 邏輯上等值
* 符號表示 「 p ≡ q 」
* 也可用 「 p ⇔ q 」表示

## 笛摩根定律 De Morgan's Laws
* ¬(p ∨ q) ≡ ¬p ∧ ¬q 
* ¬(p ∧ q) ≡ ¬p ∨ ¬q 

p | q | ¬p | ¬q | p ∨ q | ¬(p ∨ q) | ¬p ∧ ¬q 
--|--|-------|-------|-------|-------|-------
T | T | F | F | T | F | F
T | F | F | T | T | F | F
F | T | T | F | T | F | F
F | F | T | T | F | T | T

## 邏輯等式
### 同一律 identity laws
* p ∧ T ≡ p
* p ∨ F ≡ p
### 支配律 domination laws
* p ∨ T ≡ T
* p ∧ F ≡ F
### 冪等律或重複增減法 idempotent laws
* p ∨ p ≡ p
* p ∧ p ≡ p
### 雙重否定律 double negation law
* ¬(¬p) ≡ p
### 交換律 commutative laws
* p ∨ q ≡ q ∨ p
* p ∧ q ≡ q ∧ p
### 結合律 associative laws
* p ∨ ( q ∨ r ) ≡ ( p ∨ q ) ∨ r
* p ∧ ( q ∧ r ) ≡ ( p ∧ q ) ∧ r
### 分配律 distributive laws
* p ∨ ( q ∧ r ) ≡ ( p ∨ q ) ∧ ( p ∨ r )
* p ∧ ( q ∨ r ) ≡ ( p ∧ q ) ∨ ( p ∧ r )
### 笛摩根定律 De Morgan's laws
* ¬(p ∨ q) ≡ ¬p ∧ ¬q 
* ¬(p ∧ q) ≡ ¬p ∨ ¬q 
### 吸收律 absorption laws
* p ∨ ( p ∧ q ) ≡ p
* p ∧ ( p ∨ q ) ≡ p
### 否定律 negative laws
* p ∨ ¬p ≡ T
* p ∧ ¬p ≡ F

## 命題可滿足性
* 一複合命題存在組真假值能使命題為真，稱為 「複合命題是可滿足的 ( satisfiable )」
* 若找不到一組值為真，稱為「複合命題為不可滿足的 ( unsatisfiable )」

# chapter1-4
## 述詞
* 述句「x 大於 3」
* 主詞 : 變數 x
* 述詞 ( predicate ) : 大於 3
* 命題函數 ( propositional function) : P(x) 代表述詞「x 大於 3」
* 一旦變數 x 值被設定，P(x) 就成為一個具有真假值的命題
### 例子
* P(x) 代表數句「 x > 3 」，求 P(2) 和 P(4) 的真假值
* P(2) : 2 > 3 ? ---> 假
* P(4) : 4 > 3 ? ---> 真

## 量詞 quantification
## 全稱量詞 ∀ universal quantifier
* 符號 ∀xP(x) 代表 P(x) 之全稱量化
* 讀作「對所有的 x 而言，P(x)」
* P(x) 為假的元素，稱為 ∀xP(x) 之 反例( counterexample )或異例

述句 | 真 ? | 假 ?
-----|-----|-----
∀xP(x)|每一個 x 都讓 P(x) 為真|存在一個 x 讓 P(x) 為假

### 例子一
* P(x) 代表述句「x+1 > x」。倘若論域包含所有實數，請問 ∀xP(x) 的真假值為何?
解 : 對所有實數而言， P(x) 皆為真 : 因此 ∀xP(x) 真假值為真
### 例子二
* P(x) 代表述句「x < 2」。倘若論域包含所有實數，請問 ∀xP(x) 的真假值為何?
解 : P(3)為假。x = 3 為 ∀xP(x) 的一個反例 : 因此 ∀xP(x) 真假值為假

## 存在量詞 ∃ existential quantifier
* 符號 ∃xP(x) 代表 P(x) 之存在量化
* 讀作「論域中存在一元素 x ，P(x)」

述句 | 真 ? | 假 ?
-----|-----|-----
∃xP(x)|存在一個 x 讓 P(x) 為真|每一個 x 都讓 P(x) 為假

### 例子一
* P(x) 代表述句「x > 3」。倘若論域包含所有實數，請問 ∃xP(x) 的真假值為何?
解 : x = 4 時， P(x) 皆為真 : 因此 ∃xP(x) 真假值為真
### 例子二
* P(x) 代表述句「x+1 = x」。倘若論域包含所有實數，請問 ∃xP(x) 的真假值為何?
解 : 對所有實數而言， P(x) 皆為假 : 因此 ∃xP(x) 真假值為假

## 唯一量詞 uniqueness quantifier
* 以符號「∃!」或「∃₁」表示
* ∃!xP(x) 意指「存在一獨特 x，使 P(x) 為真」

### 例子
* ∃!x(x-1=0)之真假值為何?
解 : 此述句為真，x = 1 是唯一滿足 x-1=0 的實數。此述句說明存在唯一實數 x 使得 x-1=0

