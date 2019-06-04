## Q. フォルダー内のファイルを修正するブランチを作成し、関数の修正を行い master ブランチにマージを行うこと


## Answer

1.ターミナルからブランチを作成、Masterから作成したbranchにきりかえる。

 `git branch <ブランチ名>`
 `git checkout <ブランチ名>`


2.ファイルを修正し保存した後、ターミナルからgitにadd、commitし、リモートの新規ブランチにpushする。

 `git add .`
 `git commit -m "<コミットメッセージ>"`
 `git push origin <ブランチ名>`
 

3.githubのリモートリポジトリ上表示されるブランチ名に表示されるcompare & pull requestボタンを押し、pull requestをつくる。


4.file changedタブを開き変更された内容に問題がないことが確認できたら、Merge pull request ボタン、comfilm mergeボタンを押しmergeを完了させる。マージ完了後、作成したbranchは削除。


5.ターミナル上でブランチをmasterにきりかえ、リモートのmasterデータをpullしてローカルのmasterブランチを最新の状態にする。
  `git checkout master`
  `git pull origin master`
