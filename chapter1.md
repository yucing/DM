# chapter1 邏輯與證明

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