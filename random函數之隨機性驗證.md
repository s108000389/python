```python
import random
# 生成10個名為count_(i)之變數,且值為0
i=0
for i in range(1,11):
    globals()['count_'+str(i)]=0

#count_help()
#函數說明
def count_help():
    print("count_set() : 重設count_系列變數之值為0")
    print("count_test(n) : 生成亂數n次 並記錄出現次數")
    print("count_print()  : 印出各個數出現次數")
    print("count_loop(n) : 循環n次上述程序 並在最後重設計數器")
    print("count_N(n) : 不經統計直接印出n個數")
    print("count_help() : 呼叫此說明表")

count_help()

# count_set()
#重設count_系列變數之值為0
def count_set():
    i=0
    for i in range(1,11):
        globals()['count_'+str(i)]=0

# count_test(n)
# 亂數生成n次 並記錄出現次數
def count_test(n):
    for i in range(1,n+1):
        x=random.randint(1,10)
        y=0
        for i in range(1,11):
            y +=1
            if (x==y):
                globals()['count_'+str(y)] +=1
            

#count_print()
 # 印出各個數出現次數
def count_print():
    for i in range(1,11):
        print(globals()['count_'+str(i)])


#count_loop(n)
#循環n次上述程序 並在最後重設計數器
def count_loop(n):
    count_set()
    count_test(n)
    count_print()
    count_set()


#count_N(n)
#不經統計直接印出n個數
def count_N(n):
    for i in range(1,n+1):
        print(random.randint(1,10))
        

```
