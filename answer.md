# 第1次隨堂題目-隨堂-QZ1
>
>學號：112111234   (學號和姓名都要寫)
><br />
>姓名：阮陳家興
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x] 說明內容

## 說明程式與內容

開始寫說明，該說明需說明想法，
並於之後再對上述想法的每一部分將程式進一步進行展現，
若需引用程式區則使用下面方法，
若為.cs檔內程式除了於敘述中需註明檔案名稱外，
還需使用語法` ```語言種類 程式碼 ``` `，其中語言種類若是要用python則使用py，java則使用java，C/C++則使用cpp，
下段程式碼為語言種類選擇csharp使用後結果：

```csharp
public void mt_getResult(){
    ...
}
```

若要於內文中標示部分網頁檔，則使用以下標籤` ```html 程式碼 ``` `，
下段程式碼則為使用後結果：

```html
<%@ Page Language="C#" AutoEventWireup="true" ...>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
<meta http-equiv="Content-Type" ...>
    <title></title>
</head>
<body>
    <form id="form1" runat="server">
        <div>
        </div>
    </form>
</body>
</html>
```
更多markdown方法可參閱[https://ithelp.ithome.com.tw/articles/10203758](https://ithelp.ithome.com.tw/articles/10203758)

請在撰寫"說明程式與內容"該塊內容，請把原該塊內上述敘述刪除，該塊上述內容只是用來指引該怎麼撰寫內容。

1. 

Ans: # 課堂作業報告

## 任務三觀察結果

在將分支 `add_course` 合併到 `main` 時，發生了衝突（merge conflict）。原因是兩個分支同時修改了 `Introduction.md` 檔案的最後部分，導致 Git 無法自動判斷應該採用哪一個版本。

具體來說，Git 會在檔案中標示衝突區域，使用如 `<<<<<<< HEAD`、`=======` 和 `>>>>>>> add_course` 等符號，表示存在兩個不同版本的內容需要進行合併。

為了解決這個問題，我採取了以下步驟：
- 開啟 `Introduction.md` 檔案並檢查衝突內容  
- 比較兩個分支之間的差異  
- 保留雙方重要且必要的資訊  
- 刪除 Git 的衝突標記符號  
- 儲存修改後的檔案  

接著，我使用 `git add` 和 `git commit` 指令完成合併流程。最終成功將內容整合，且檔案中不再存在任何衝突。
![alt text](image.png)
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
![alt text](image-6.png)
![alt text](image-7.png)
###
    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1 (main)
    $ mkdir my-project

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1 (main)
    $ cd my-project

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git init
    Initialized empty Git repository in C:/Users/Hag/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project/.git/

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (master)
    $ git branch -M main

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git add Introduction.md
    fatal: pathspec 'Introduction.md' did not match any files

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git add Introduction.md

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git commit -m "Khởi tạo dự án và thêm giới thiệu bản thân"
    [main (root-commit) 1a6a11f] Khởi tạo dự án và thêm giới thiệu bản thân
    1 file changed, 2 insertions(+)
    create mode 100644 Introduction.md

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git push -u origin main
    fatal: 'origin' does not appear to be a git repository
    fatal: Could not read from remote repository.

    Please make sure you have the correct access rights
    and the repository exists.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git remote -v

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git remote add origin git@github.com:hag01292/114-2QZ1.git

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git push -u origin main
    To github.com:hag01292/114-2QZ1.git
    ! [rejected]        main -> main (fetch first)
    error: failed to push some refs to 'github.com:hag01292/114-2QZ1.git'
    hint: Updates were rejected because the remote contains work that you do not
    hint: have locally. This is usually caused by another repository pushing to
    hint: the same ref. If you want to integrate the remote changes, use
    hint: 'git pull' before pushing again.
    hint: See the 'Note about fast-forwards' in 'git push --help' for details.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git pull origin main --rebase
    remote: Enumerating objects: 4, done.
    remote: Counting objects: 100% (2/2), done.
    remote: Compressing objects: 100% (2/2), done.
    remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 2 (from 1)
    Unpacking objects: 100% (4/4), 453.44 KiB | 687.00 KiB/s, done.
    From github.com:hag01292/114-2QZ1
    * branch            main       -> FETCH_HEAD
    * [new branch]      main       -> origin/main
    Successfully rebased and updated refs/heads/main.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git push -u origin main
    Enumerating objects: 4, done.
    Counting objects: 100% (4/4), done.
    Delta compression using up to 20 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 1.05 KiB | 1.05 MiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
    To github.com:hag01292/114-2QZ1.git
    1768d9f..cd4db58  main -> main
    branch 'main' set up to track 'origin/main'.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git checkout -b add_plan
    Switched to a new branch 'add_plan'

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_plan)
    $ git add Introduction.md

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_plan)
    $ git commit -m "Thêm kế hoạch học tập"
    [add_plan ef5c127] Thêm kế hoạch học tập
    1 file changed, 6 insertions(+), 1 deletion(-)

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_plan)
    $ git push -u origin add_plan
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 20 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 879 bytes | 879.00 KiB/s, done.
    Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
    remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
    remote: 
    remote: Create a pull request for 'add_plan' on GitHub by visiting:
    remote:      https://github.com/hag01292/114-2QZ1/pull/new/add_plan
    remote: 
    To github.com:hag01292/114-2QZ1.git
    * [new branch]      add_plan -> add_plan
    branch 'add_plan' set up to track 'origin/add_plan'.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_plan)
    $ git checkout main
    Switched to branch 'main'
    Your branch is up to date with 'origin/main'.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git checkout -b add_course
    Switched to a new branch 'add_course'

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_course)
    $ git add Introduction.md

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_course)
    $ git commit -m "Thêm phân tích dữ liệu khóa học"
    [add_course 7b1e1c3] Thêm phân tích dữ liệu khóa học
    1 file changed, 8 insertions(+), 1 deletion(-)

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_course)
    $ git push -u origin add_course
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 20 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 1.41 KiB | 1.41 MiB/s, done.
    Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    remote: 
    remote: Create a pull request for 'add_course' on GitHub by visiting:
    remote:      https://github.com/hag01292/114-2QZ1/pull/new/add_course
    remote: 
    To github.com:hag01292/114-2QZ1.git
    * [new branch]      add_course -> add_course
    branch 'add_course' set up to track 'origin/add_course'.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (add_course)
    $ git checkout main
    Switched to branch 'main'
    Your branch is up to date with 'origin/main'.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git merge add_plan
    Updating cd4db58..ef5c127
    Fast-forward
    Introduction.md | 7 ++++++-
    1 file changed, 6 insertions(+), 1 deletion(-)

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git merge add_course
    Auto-merging Introduction.md
    CONFLICT (content): Merge conflict in Introduction.md
    Automatic merge failed; fix conflicts and then commit the result.

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main|MERGING)
    $ git add Introduction.md

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main|MERGING)
    $ git commit -m "Giải quyết xung đột hợp nhất giữa add_plan và add_course"
    [main 6d1ea6c] Giải quyết xung đột hợp nhất giữa add_plan và add_course

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ git push
    Enumerating objects: 7, done.
    Counting objects: 100% (7/7), done.
    Delta compression using up to 20 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 966 bytes | 966.00 KiB/s, done.
    Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
    remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
    To github.com:hag01292/114-2QZ1.git
    cd4db58..6d1ea6c  main -> main

    Hag@Helagion-IU45PJOE MINGW64 ~/OneDrive/Tài liệu/亞東-114/商業智慧/114-2QZ1/my-project (main)
    $ 

###