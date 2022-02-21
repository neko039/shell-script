# saferm
## 介紹
* 功能類似於window的資源回收桶，會在刪除時，將檔案備份到隱藏的資料夾中，並且為了避免隱藏資料夾占用過多空間，會每天清理一次隱藏資料夾
* 有指令使用歷史查看與檔案恢復(使用指令，不需要手動複製回來)的功能
* 指令與rm通用，可以直接使用saferm來運行rm
## 前置步驟
以root權限運行setting執行檔，此執行檔會運行以下動作：
* 建立 "/.Recycle_Bin"
* 建立系統排程: "0 12 * * * /usr/bin/rm /.Recycle_Bin/*"
* 將saferm放到 "/usr/local/sbin" 路徑
* 將README放到 "/usr/share/doc/saferm" 路徑
## 參考來源
https://ithelp.ithome.com.tw/articles/10228425

# ugrep
## 介紹
* 將/etc/passwd的內容以較整齊格式查看，並可以自行選擇要顯示的欄位(功能類似ps -o)，也可以依照系統帳號與一般使用者帳號(類似yum list顯示)做分類
