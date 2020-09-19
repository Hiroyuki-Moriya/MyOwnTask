# penguin numbers (ペンギン数)

## Description(説明)


A natural number in which the sum (number sum) and product (number product) of each digit of an integer are equal is called a penguin number.
整数の各桁の和(数字和)と積(数字積)が等しい自然数をペンギン数と呼ぶ。

22,123,132,213,231,312,321 is penguin number.
22,123,132,213,231,312,321はペンギン数です。

It is not clear at this time whether there are other penguin number.
ペンギン数がほかにもあるのかどうか今のところ不明です。

オンライン整数列大辞典 http://oeis.org/?language=japanese  
[オンライン整数列大辞典](http://oeis.org/?language=japanese)  

## example(例)
### 22  
 2+2=4 2*2=4  

### 123  
  1+2+3=6 1*2*3=6  

### 132  
  1+3+2=6 1*3*2=6  

### 213  
  2+1+3=6 2*1*3=6  

### 231  
  2+3+1=6 2*3*1=6  

### 312  
  3+1+2=6 3*1*2=6  

### 321  
  3+2+1=6 3*2*1=6  


## algorithm(アルゴリズム)
  整数iの発生 11から指定する値までカウントアップ
  整数iの桁を調べる j=len(i)
  整数iを桁にばらす i[0],i[1],i[2],,,i[j-1]
  数字和を求める numberSum = i[0]+i[1]+i[2]+,,,+i[j-1]
  数字和を求める numberProduct= i[0]*i[1]*i[2]*,,,*i[j-1]
  数字和と数字積が等しければ、ペンギン数iと数字和を表示する
