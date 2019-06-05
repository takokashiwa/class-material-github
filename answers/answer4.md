### Q.下記に従い question フォルダー内の README.md を修正すること master ブランチにマージを行うこと

## Answer

1. ターミナルからブランチを作成、Masterから作成したbranchにきりかえる。

 `git branch <ブランチ名>`
 
 `git checkout <ブランチ名>`
 
2. Github上のリモートリポジトリに移動。README.mdファイル表示の右側にあるペンタブアイコンをクリックし、ファイルを修正した後、下部にある Commit directly to the master branch.　のラジオボタンにチェックをいれCommit changesボタンを押す。 

3. ローカルの READMD.md を修正したのち、ターミナル上からgitにadd、commit、pushを行う。

  `git add .`
  
  `git commit -m "<コミットメッセージ>"`
  
  `git push origin <ブランチ名>`


4. Githubのリモートリポジトリ上表示されるブランチ名に表示されるcompare & pull requestボタンを押し、pull requestをつくる。


5. pull requestの画面上に`This branch has conflicts that must be resolved`と表示がされているのでresolve conflictのボタンを押し、編集画面からファイルの修正を行う。（masterと新規ブランチとの変更箇所の差異が表示されるので、更新したいデータを残す。）修正が完了したら画面右上のmark as resolvedボタンを押す。次に表示されるcommit mergeを押した後、pullrequest画面からmerge pullrequestボタン、comfirm mergeボタンを押してmergeを完了し、作業ブランチは削除する。

6. ターミナル上でブランチをmasterにきりかえ、リモートのmasterデータをpullしてローカルのmasterブランチを最新の状態にする。

  `git checkout master`

  `git pull origin master`
