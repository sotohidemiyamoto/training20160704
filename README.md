# training20160704

## 本日のマテリアル

[GitHub for developers](http://ikeike443.github.io/training-kit/courses/github-for-developers.html)

### gitツール

[Git for Windows](https://git-for-windows.github.io/)  
[GitHub Desktop](https://desktop.github.com/)  

### git資料

[Gitチートシート](https://services.github.com/kit/downloads/ja/github-git-cheat-sheet.pdf) - PDF  
[Pro Git 2 eBook](http://git-scm.com/book/ja/v2) - Gitの電子書籍。

### その他

[GitHub Guides](https://guides.github.com/)  
[GitHub Training & Guides](https://www.youtube.com/watch?v=FyfwLX4HAxM&list=PLg7s6cbtAD15G8lNyoaYDuKZSKyJrgwB-) - Youtube (日本語字幕付)  
[Emoji seacher](http://emoji.muan.co/) - 絵文字検索  

## git setup

### アカウント

nameとemailはGitHubのアカウントと一致させてください。  
`$ git config --global user.name "name"`  
`$ git config --global user.email "email address"`  

確認  
`$ git config --list | grep name`  
`$ git config --list | grep email`  

### 表示と改行コードの設定

`$ git config --global color.ui auto`  

Windows  
`$ git config --global core.autocrlf true`  
Mac/Linux  
`$ git config --global core.autocrlf input`  

改行コードを変更しない場合  
`$ git config --global core.autocrlf false`

### Windowsユーザ

Git Bashでの日本語の文字化け対策  
`$ git config --global core.quotepath false`  
  
CommitメッセージをvimではなくNotepadで入力する場合。  
`$ git config --global core.editor notepad`  
*NotepadはUTF-8ではないので、日本語はWEB上で文字化けしますのでご注意ください。*  
  
サクラエディタを指定してもOK。  
`$ git config --global core.editor "'C:/Program Files/sakura/sakura.exe' -CODE=4"`  
*sakura.exeのパスは、各自のローカルでご確認ください。*

秀丸(動作未確認 :bow: )  
`$ git config ?global core.editor “‘C:/program files/hidemaru/hidemaru.exe’ //fu8”`

## 以下は必要に応じて設定を行ってください

### HTTP Proxy

`$ git config --global http.proxy http://xxxx:8080`  

### その他

GitHub Enterpriseを自己署名証明書で運用する場合  
`$ git config --global http.sslVerify false`

