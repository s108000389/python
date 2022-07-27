- [input()函式](https://ithelp.ithome.com.tw/articles/10201956)
- [暫停執行_參考](https://www.delftstack.com/zh-tw/howto/python/python-pause/)
- [暫停執行視窗](#暫停執行視窗)

### input
input()函式會讓程式暫停，等待使用者輸入一些文字，  
python在取得使用者輸入文字後，會把我們輸入的文字存到一個變數內  
  - 範例
  ```python
  name = input("please enter your name : ")
  print("hello,"+name) # 因為name是字串所以可以直接跟"hello,"字串相加
  ```
  - 輸出結果
  ```
  please enter your name : bonny
  hello,bonny
  ```
  
  - 用int()來取得輸入的字串
  ```python
  i=1
  while(i != 0):
    i=input("選擇執行程式")
    i=int(i) # 要先轉為int
    if  (i==0):
        break
    elif (i==1):
        print("hello world")
  ```
  
### 暫停執行視窗
暫停程式的執行，直到使用者按下任意鍵
```python
import os

os.system("pause")
```
