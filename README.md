# 109NS-IC 109南山校內資訊競賽 題目

[1].中位數 10%
中位數是統計學裡面的一個名詞，代表將一群數字從小排到大之後，位於正中
間的那個數字，例如有 5 個數字分別為 1、2、3、4、5，則中位數則是 3，而當
數字個數為偶數時，則是最中間兩個數字的平均，例如 2、4、6、8，中位數則
是(4+6)÷2=5。
為了方便計算，本題只考量數字個數為奇數的情況，給你這些數字，請你找出
其中位數是多少。
例：
input: 1 2 3 4 5
output: 3

input: 90 80 70 60 50 40 45 55 65 75 85
output: 65

[2]. (10%) 3025 這個數字有個巧合，如果你將這數字看成字串，將其分為兩
半，每一半也都是一個十位數，亦即 30 和 25，則其和平方
(30+25)^2 = 3025
又變成原來的數字了。你的題目是找出這種類似的巧合數字出來，你的程式要
讀取一個位數(2、4、6、或 8)，然後找出該位數的所有類似巧合的數字。例如
4 位數，從 0000 到 9999。請注意，0 也要算在內，也就是說 0001 也等於
(00+01)^2，也是 4 位數中的巧合數。例如輸入 2 時，輸出是
00
01
81


[3].計算含有 s 或 S 字母的字數。 (程式執行限制時間: 2 秒) 15%
每列測試資料(每組測試資料)有多個英文字，字和字之間用一個或多個空白
開。 ”, ;! .” 這四個符號會與英文字相鄰。寫一程式計算每列測試資料(每組
測試資料)含有 s 或 S 字母的字數。
例:
Input: This is a sample file.
Output: 3

Input: Hello World!!
Output: 0

Input: SOS!
Output: 1


[4]. 統計答案得分 15%
統計答案得分，O 得分，X 沒得分，連續 O 得分就多。將每個連續的 O 的分
數累加起來即可 得解。 統計答案分： O O X X O X X O O O 得分： 1 2 0 0 1 0 0
1 2 3 統計答案得分：OOXXOXXOOO 得分：1+2+0+0+1+0+0+1+2+3=10
統計答案分： O O X X O O X X O O 得分： 1 2 0 0 1 2 0 0 1 2 統計答案得分：
OOXXOOXXOO 得分：1+2+0+0+1+2+0+0+1+2=9
統計答案分： O X O X O X O X O X O X 得分： 1 0 1 0 1 0 1 0 1 0 1 0 統計答案得
分：OXOXOXOXOXOX 得分：1+0+1+0+1+0+1+0+1+0+1+0=6
統計答案分： O O O O O O O O O O 得分： 1 2 3 4 5 6 7 8 9 10 統計答案得分：
OOOOOOOOOO 得分：1+2+3+4+5+6+7+8+9+10=55
統計答案分： O O O O X O O O O X 得分： 1 2 3 4 0 1 2 3 4 0 統計答案得分：
OOOOXOOOOX 得分：1+2+3+4+0+1+2+3+4+0=20

例:
Input: OOOOOXOOOOXOXOXOOOXOXXOOXOOXOOOOOOX
Output: 61


[5]. 給一個羅馬數字符號，轉為整數數字。(程式執行限制時間: 2 秒) 25%
羅馬數字是古羅馬所使用的數字系統，以羅馬符號來表示數值。如果要對應成
現在通用的阿 拉伯數字，只用 7 個符號，包括 I(1)，V(5)，X(10)，L(50)，
C(100)，D(500)，M(1000)。羅馬 數字並沒有 0。羅馬數字 I 代表阿拉伯數字
的 1，但 II 可不是代表 11，而是 1+1=2， III 為 3。 如果要用羅馬數字來表
示 4，不能寫成 IIII，而要寫成 IV，意思是 5-1=4。阿拉伯數字為 9 時， 要
寫成 IX。 (1)重複數次決定倍數：1 個羅馬數字重複幾次，就表示這個數的
幾倍。例如：ⅩⅩⅩ=30。數 碼有限制，同樣數碼最多只能出現 3 次，例如
40 不能表示為 XXXX，而要表示為 XL。
(2)右加左減：在 1 個較大的羅馬數字的右邊跟 1~3 個較小的羅馬羅馬數字，
表示大數字加小 數字。在一個較大的數字的左邊跟 1 個較小的羅馬數字，表
示大數字減小數字。左減數字不 能超過 1 位，比如 8 寫成 VIII，而非 IIX。
右加數字最多只能 3 位，例如 14 寫成 XIV，而非 XIIII。
(3)數字上加橫線乘千或乘百萬：在 1 個羅馬數字的上方加上 1 條橫線或者在
右下方寫 M，表 示將這個數字乘以 1000，即是原數的 1000 倍。同理，如果
上方有 2 條橫線，即是原數的 1000000 倍。
羅馬數字與十進位數字的轉換範例：
IX = 9
VI = 6
XI = 11
XVII = 17
CCLXVIII=100 + 100 + 50 + 10 + 5 + 1 + 1 + 1= 268
MMMCC=1,000 + 1,000 + 1,000 + 100 + 100 = 3200
DCCVII=500 + 100 + 100 + 5 + 1 + 1 = 707
MMCDLXIX= 1000 + 1000 + [500-100] + 50 + 10 + [10-1] = 2469
例:

Input: CCLXVIII
Output: 268

Input: MMCDLXIX
Output: 2469


[6]. 包含某個數字 25%
介於 [A, B] 之間，找一個包含數字 N，且[A, B] 之間的所有數字有包含 N 的
數字，找出有 N 的數字有幾個數。 例如： A = 3， B = 17， N = 3 ，[A, B] =
[3, 17] = [3,4,5,6,…,13,14,15,16,17]，包含數字 N,3 的整數有 3 和 13。 例如：
A = 0， B = 20， N = 0 ，[A, B] = [0, 20]，包含數字 N,0 的整數有 0 、10 和
20。 例如： A = 0， B = 150， N = 17 ，[A, B] = [0, 150]，包含數字 N,17 的整
數有 17 和 117。
輸入說明：三個整 數 A B N ，0=< A,B =<65535，0=< N =<999 ，以一個或多個
空白作為區隔。
輸出說明：每筆測試資料輸出一列。測試資料[A, B] 之間的所有數字有包含 N
的數字的個數。
例:
Input: 3 17 3
Output: 2

Input: 0 20 0
Output: 3

Input: 13 17 1
Output: 5
