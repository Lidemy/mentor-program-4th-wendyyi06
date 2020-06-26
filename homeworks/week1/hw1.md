## 交作業流程

1.新開一個 branch： `git branch hw1`

2.切換到 branch： `git checkout hw1`

(也可以直接使用：`git checkout -b hw1`)

3.開始寫作業(記得要先確認有切到 branch )

4.確認是否改動：`git status`

5.看改動了哪裡：`git diff`，按 q 可以離開。

6.如果有新增的檔案，記得加進去 git：`git add.`

7.提交改動：`git commit -am " hw1 "`

8.把本地端的 hw1 branch 同步到遠端上：`git push origin hw1` (origin 是 github 遠端的意思)

9.到 github 頁面的" Pull reguests "，會出現新的提示，按" Compare & pull request "。

10.往下拉確認自己改的東西都有上去，在上面的框框打"第一週作業"，如果有任何問題可以打在下方框框，最後按" Create pull request "。(助教會在" Files changed "看作業並留言)

11.到學習系統的"作業列表"，按"新增作業"，選擇是第幾週的作業，並到 github 把 Pull requests (簡稱 PR )的連結貼上去(網址會有 pull)，下方兩個框框確認後打勾並送出，就可以在列表看到自己交的作業。

12.助教改完作業確認沒問題後，會按" Merge pull request "，merge 完後會把遠端的 branch 刪掉。

13.確認遠端被 merge 後，在 local 端切換到 master ：`git checkout master`

14.把遠端最新的 master 跟 local 端的 master 同步：`git pull origin master`

15.把本地的 hw1 branch 刪除：`git branch -d hw1`

16.用 `git branch -v` 確認只剩下 master 這個 branch。

17.用 `git log` 看，會看到 hw1 已經完成的 commit 進去。

18.完成交作業流程。