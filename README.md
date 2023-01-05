# **git_tutorial1**
最初に知っておいたほうが良いかもしれないことを説明してるので、「もう知ってる！」という方は読み飛ばしてください  
Qiitaで書けよってくらい長いです  
GitHubアカウント作成済の方は、[README2.md](https://github.com/wassy310/NITOC_Robocon_git_tutorial/blob/master/README2.md)から行ってください

## **そもそもGitとは何か、なぜ使うのか**
Gitとは「バージョン管理を行うシステム」のこと  
- バージョン管理でできること
  - 変更箇所の確認
  - 過去の状態に戻す  
など

## **リポジトリとは**
Gitによって管理されているファイル群のこと
- 主に2種類のリポジトリを駆使して、バージョン管理を行う
  - ローカルリポジトリ  
    PC(エディタなど)で書き、コミットした状態のものがローカルリポジトリ  
    ※ コミットに関しては後々説明があります
  - リモートリポジトリ  
    GitHubなどで公開されているのはリモートリポジトリ

## **GitHubとは**
- リモートリポジトリの集約先  
- チーム開発でもよく使われる  
- 他人のコードレビューもできる

## **Gitのインストール**
### **Mac**
不要(デフォルトでインストール済み)
### **Windows**
1. [インストーラをダウンロード](https://gitforwindows.org/)
1. ダウンロード後、起動
1. オプションとかの質問は全部デフォルトのままでOK(Nextボタン連打しててOK)
1. 最後はInstallボタンを押してインストールしてください
1. Git Bashを起動(検索バーで"git"って検索すると出てくる)
1. 以下のコマンドを実行  
`git --version`  
画像のような表示が出ればGitのインストールは終了  
![image](https://user-images.githubusercontent.com/74349349/210730423-d1e8b0ee-0ec4-41e0-8402-079a4cde1b8d.png)

## **初期設定**
Macはターミナル、WindowsはそのままGit Bashで操作していきます  
Gitでの変更履歴などを辿るために、まずは自分の情報を登録します  
### **ユーザ名**
以下のコマンドを実行  
`git config --global user.name 任意のユーザ名`
### **メールアドレス**
以下のコマンドを実行  
`git config --global user.email 任意のメールアドレス`
### **確認**
登録情報(ユーザ名・メールアドレス)の確認  
`git config --list`  
確認コマンドを実行後、文字がぶわーって出てくると思いますが(語彙力)、その中に先ほど登録したユーザ名とメールアドレスがあればOKです

## **GitHubのアカウント作成**
既につくってあるよ～って方は飛ばしてください  
GitHubのアカウントをつくります。
1. [GitHub](https://github.com/)にアクセス
1. GitHubで使うユーザ名、メールアドレス、パスワードを設定し、Sign upを押します
1. プランを訊かれますが、特にこだわりがなければfree planで大丈夫です
1. "Welcome to GitHub"と表示されたら、下のほうにある"Complete setup"を押します
1. メール認証があるので、先ほど入力したメールアドレスに届いたメール通りに進めます
1. これでアカウント作成は終了

キリが良いので、[次のファイル](https://github.com/wassy310/NITOC_Robocon_git_tutorial/blob/master/README2.md)に移ります。  
次からは、実際にリポジトリを作ってGitHubにアップロードまでします。