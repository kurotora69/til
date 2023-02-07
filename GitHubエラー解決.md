 #デスクトップからリモートへPushができない

***
エラー文  
error: /Applications/GitHub Desktop.app/Contents/Resources/app/desktop-trampoline/desktop-trampoline died of signal 9
error: unable to read askpass response from '/Applications/GitHub Desktop.app/Contents/Resources/app/desktop-trampoline/desktop-trampoline'
fatal: could not read Username for 'https://github.com': terminal prompts disabled
***

原因は認証情報がないこと(らしい)。

参考資料  
https://docs.github.com/ja/desktop/installing-and-configuring-github-desktop/installing-and-authenticating-to-github-desktop/authenticating-to-github

https://christina04.hatenablog.com/entry/handle-error-when-go-get-private-repo

解決法  

1.リモートGitHubで一度sigh outし、sign inし直す。

2.メニューバーの [GitHub Desktop] ドロップダウンメニューで、 [Preferences](環境設定) をクリックする。

3.[Preferences](環境設定) ウィンドウで、 [Accounts] (アカウント) を選択。

4.[GitHub.com] の右にある [サインイン] をクリック。

5.[Sign in Using Your Browser](ブラウザーを使用してサインイン) で、 [Continue With Browser](ブラウザーで続行) をクリックする。  
  GitHub Desktop はデフォルトのブラウザを開く。
  
6.GitHub に対して認証するために、自分の GitHub.com の資格情報を入力し、 [Sign in](サインイン) をクリックする。  
  (すでにGitHubにサインインしてる場合は、プロンプトに従ってGitHub Desktopに戻り、認証を完了させる。)
  

上記解決法を実施し、無事リモートリポジトリへPushができた。
 
