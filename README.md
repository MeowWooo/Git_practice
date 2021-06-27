Git_practice : Practicing to use git

## 練習紀錄:
*第一次使用須將 GitGub 權限授權給 Git <br>
*Message中不能有`Space`

### 1. 安裝Git 註冊GitHub
> * Git官網 [https://git-scm.com/](https://git-scm.com/ "Git官網") 
> * GitHub首頁 [https://github.com/](https://github.com/ "GitHub首頁") 

### 2. 設定本機端Git資訊
    git config --global user.name [名字]
    git config --global user.email [電子信箱]
    git config --global user.username [GitHub的名字]

### 3. 建立本機端Git
    D: C: cd [路徑]   // 進入要設置Git的目錄
    git init          // 設置Git

### 4. 各式操作
    git add [檔案路徑]         // 將檔案或目錄加入追蹤
    git commit -m [Message]   // 紀錄更改

    rm -rf [檔案路徑]            // 刪除該路徑下所有檔
    git rm [檔案路徑]            // 同上(未測試)
    git commit -a -m [Message]  // 紀錄更改(刪除用)

### 5. 跟GitHub連結
    git remote add origin [GitHub專案網址]  // 連結到專案網址

    git pull                    // 下載更新本機端專案資料
    git pull origin             // 同上
    git pull --rebase origin    // 同上
    git pull origin [檔案路徑]             // 下載更新某指定的資料
    git pull --rebase origin [檔案路徑]    // 同上

    git push -u origin master   // 首次連結GitHub進行Push
    git push                    // 之後都可以用簡寫

### 6. 資料/狀態查詢
    git --version   // git版本
    git status      // 當前git狀態查詢
    git diff        // 顯示此次修改了什麼(commit之後用)
    ls -la          // 列出目錄內的資料 -l:列出詳細資料, -a:列出隱藏項目
      
    git --help          // 指令清單&介紹
    git [指令] --help   // 指令細部介紹(網頁)
      
## 可能遇到的問題:
### Q1:  
> ```
> ! [rejected]        master -> master (non-fast-forward)
> error: failed to push some refs to 'https://github.com/MeowWooo/Git_practice.git'
> ```
#### A1: 檢查 .git -> config 內的 [branch "master"] 是否遺失, 是的話: `git pull origin master`
      
## 參考來源:
https://blog.techbridge.cc/2018/01/17/learning-programming-and-coding-with-python-git-and-github-tutorial/
http://ryan0210.blogspot.com/2014/11/git-statuscommitpush.html
https://www.cnblogs.com/bigtreei/p/10180383.html

https://www.itread01.com/content/1546207602.html <- GitHub排版教學(暫存)

## 圖片測試:
> [Picture]:https://images2.gamme.com.tw/news2/2017/49/24/q6CVnZ2YlKOeqKQ.jpg "圖片來自:facebook.com/HappyCatsOnline"
> [![Picture]](https://news.gamme.com.tw/1494924)

## 程式碼測試:
> ```cpp
> #include <iostream>
> using namespace std;
> int main(){
>   cout << "Hello, World" << endl;
>   return 0;
> }
> ```
