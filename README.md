# Laravel 7 郵件編輯器

引入 qoraiche 的 laravel-mail-editor 套件來擴增輕鬆玩 Laravel Mailables，供 Laravel 應用程式使用 Web 使用者介面建立和管理 Mailables。可以使用此套件來開發 Mailables，而無需使用命令行，以及使用 WYSIWYG 編輯器以及其他功能來編輯與 Mailables 相關的模板。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/maileclipse` 來進行郵件編輯器瀏覽。

----

## 畫面截圖
![](https://i.imgur.com/B3nYFbs.png)
> 在 Laravel 中，應用程式送出的每種類型的郵件都是以「mailable」類別表示。這些類別存放在 app/Mail 資料夾中

![](https://i.imgur.com/mrDCgs0.png)
> 可以選擇使用拖曳式編輯器，能夠讓你輕輕鬆鬆就製作出獨一無二的郵件模板