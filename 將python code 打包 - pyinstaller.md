- [將你的python code 打包 - pyinstaller](https://peaceful0907.medium.com/%E5%B0%87%E4%BD%A0%E7%9A%84python-code-%E6%89%93%E5%8C%85-pyinstaller-6777d0e06f58)

### 安裝pyinstaller
```
pip install pyinstaller
```

### 相關參數
pyinstaller -F 要打包的檔案.py  

pyinstaller -F 檔名.py --noconsole #無控制台
```
-h :help
-F :將程式打包成單一執行檔(適合較簡易的代碼或只有單一.py檔)
-D :打包多個文件，exe檔及依賴的東西會一起放置在dist資料夾內(適合框架形式的程式)
```

