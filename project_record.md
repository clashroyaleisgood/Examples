[TOC]

# 實驗記錄
## 2024/02/13
- 初次上傳紀錄至 Github
- step by step 說明使用方式 [**如下**](#Hackmd-與-Github-連接)

### Hackmd 與 Github 連接
[reference](https://hackmd.io/c/tutorials-tw/%2Fs%2Flink-with-github-tw)  

1. 註冊 Github 帳號 & 建立 Repository
2. 註冊 Hackmd 帳號 & 新增筆記
3. 從 Hackmd 筆記，連接至 Github
4. (Optional) [more you can do with github](https://medium.com/starbugs/用-hackmd-與-github-action-打造你的靜態網站-線上文章編輯平台-1d9b1a663e18)

#### step 1 創 Github
- 註冊 Github 帳號  
  (對了現在 Github 可能會要你使用更安全的 2FA 認證，之後每次登入帳號都會更安全，也更麻煩；若是把認證的東西弄丟也會很危險，所以小心操作，密碼/金鑰等資料備份好)
- 建立 Repository  
  到主頁按下綠色的 `New`  
  ![image](https://hackmd.io/_uploads/By3hUGFip.png =400x)  
  寫好 Repository Name 這項是必要的，  
  Description 可以跳過，後面選擇 `Public`，其他都先保留預設就好，除非你知道自己選的是什麼  
  ![image](https://hackmd.io/_uploads/HyVkcGYo6.png)
  Done!
#### step 2 創 Hackmd
- 註冊 Hackmd 帳號(對了! Hackmd 是台灣新創，有夠猛)
- 建立筆記  
  到主頁按下綠色的 `建立筆記`  
  ![image](https://hackmd.io/_uploads/B12zRGtip.png =300x)
- 筆記內容  
  新增一些內文，寫上標題...  
  ![image](https://hackmd.io/_uploads/BySDCztsT.png)
- ==[重要]== 將換行方式更換  
  點擊下方的 `換行`，選擇 `CommonMark 標準換行`，  
  目的是採用 Github MD 文件的換行方式  
  選擇之後，所有希望在內文中換行的地方都需要 `空格` `空格` `換行`  
  ![image](https://hackmd.io/_uploads/ry80J7YjT.png =300x)
#### step 3 連接
- 右上角的 ...，選 `版本與 Github 同步`  
  ![image](https://hackmd.io/_uploads/BJY717Fia.png =400x)
- 選 `推送至 Github`  
  (拉取/推送 分別對應到 Git 操作的 Pull/Push)  
  ![image](https://hackmd.io/_uploads/ryovymFoT.png)  
  - 第一個授權: 授權 Hackmd 存取資料  
    ![image](https://hackmd.io/_uploads/Byj7H7FsT.png =300x)  
  - 第二個授權: 授權某個 Repository 的編輯權(也就是剛創的那個)
    選擇 `授權更多 Repo`  
    ![image](https://hackmd.io/_uploads/SyMtSXFiT.png =200x)  
    在 `Repository Access` 中，選擇要授權給 Hackmd 操作的 Repository  
    ![image](https://hackmd.io/_uploads/H1K1wQYoT.png)
    回到剛剛 `推送` 後進入的頁面，選擇...  
    Repo: 剛剛操作的那個 Repository,  
    Branch: main，若是不能選擇，那就直接用輸入的  
    同步的檔案: 自己新增一個檔案，名稱自己選，副檔名記得要是 `.md` 就好  
    ![image](https://hackmd.io/_uploads/SytEdQtjp.png)  
    完成後確認送出~
#### 後續操作
之後每次完成紀錄，要推送至 Github 時只需要
- 按右上角的 ...，選 `版本與 Github 同步`
- 按 `推送變更`  
  ![image](https://hackmd.io/_uploads/B1UqeNti6.png)
- `建立新版本並推送`
  ![image](https://hackmd.io/_uploads/HJ1B-VKo6.png)  
  (這裡也可以自定義 `版本名稱` 與 `版本敘述`，對應到的是 Github 上顯示的 `commit 標題與細節敘述`；用來註記我的 code 這次做了什麼更新/調整
  ![image](https://hackmd.io/_uploads/HyiCZEFo6.png)
