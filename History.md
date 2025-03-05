### My first attempt in working on apply Hugo template:

```
Microsoft Windows [版本 10.0.26100.3194]
(c) Microsoft Corporation。保留所有权利。

C:\Users\25022>cd C:\Users\25022\Documents

C:\Users\25022\Documents>mkdir hugo-site

C:\Users\25022\Documents>cd hugo-site

C:\Users\25022\Documents\hugo-site>hugo new site .
Congratulations! Your new Hugo site was created in C:\Users\25022\Documents\hugo-site.

Just a few more steps...

1. Change the current directory to C:\Users\25022\Documents\hugo-site.
2. Create or install a theme:
   - Create a new theme with the command "hugo new theme <THEMENAME>"
   - Or, install a theme from https://themes.gohugo.io/
3. Edit hugo.toml, setting the "theme" property to the theme name.
4. Create new content with the command "hugo new content <SECTIONNAME>\<FILENAME>.<FORMAT>".
5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.

C:\Users\25022\Documents\hugo-site>git clone https://github.com/Git-SXQ6/Git-SXQ6.github.io.git
Cloning into 'Git-SXQ6.github.io'...
info: please complete authentication in your browser...
remote: Repository not found.
fatal: repository 'https://github.com/Git-SXQ6/Git-SXQ6.github.io.git/' not found

C:\Users\25022\Documents\hugo-site>hugo server -D
Watching for changes in C:\Users\25022\Documents\hugo-site\{archetypes,assets,content,data,i18n,layouts,static}
Watching for config changes in C:\Users\25022\Documents\hugo-site\hugo.toml
Start building sites …
hugo v0.145.0-666444f0a52132f9fec9f71cf25b441cc6a4f355+extended windows/amd64 BuildDate=2025-02-26T15:41:25Z VendorInfo=gohugoio

WARN  found no layout file for "html" for kind "taxonomy": You should create a template file which matches Hugo Layouts Lookup Rules for this combination.
WARN  found no layout file for "html" for kind "home": You should create a template file which matches Hugo Layouts Lookup Rules for this combination.

                   | EN
-------------------+-----
  Pages            |  4
  Paginator pages  |  0
  Non-page files   |  0
  Static files     |  0
  Processed images |  0
  Aliases          |  0
  Cleaned          |  0

Built in 6 ms
Environment: "development"
Serving pages from disk
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop

C:\Users\25022\Documents\hugo-site>git submodule add https://github.com/netlify-templates/hugo-profile themes/hugo-profile
fatal: not a git repository (or any of the parent directories): .git

C:\Users\25022\Documents\hugo-site>git init
Initialized empty Git repository in C:/Users/25022/Documents/hugo-site/.git/

C:\Users\25022\Documents\hugo-site>git submodule add https://github.com/netlify-templates/hugo-profile themes/hugo-profile
Cloning into 'C:/Users/25022/Documents/hugo-site/themes/hugo-profile'...
info: please complete authentication in your browser...
remote: Repository not found.
fatal: repository 'https://github.com/netlify-templates/hugo-profile/' not found
fatal: clone of 'https://github.com/netlify-templates/hugo-profile' into submodule path 'C:/Users/25022/Documents/hugo-site/themes/hugo-profile' failed

C:\Users\25022\Documents\hugo-site>git add .
warning: in the working copy of 'archetypes/default.md', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'hugo.toml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/categories/index.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/index.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/sitemap.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/tags/index.xml', LF will be replaced by CRLF the next time Git touches it

C:\Users\25022\Documents\hugo-site>git commit -m "add hugo profile theme"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got '25022@LAPTOP-VT5GNU86.(none)')

C:\Users\25022\Documents\hugo-site>git config --global user.name "Xiaoqian Shen"

C:\Users\25022\Documents\hugo-site>git config --global user.email "shengxiumuqi@outlook.com"

C:\Users\25022\Documents\hugo-site>git commit -m "add hugo profile theme"
[master (root-commit) 66a4423] add hugo profile theme
 7 files changed, 52 insertions(+)
 create mode 100644 .hugo_build.lock
 create mode 100644 archetypes/default.md
 create mode 100644 hugo.toml
 create mode 100644 public/categories/index.xml
 create mode 100644 public/index.xml
 create mode 100644 public/sitemap.xml
 create mode 100644 public/tags/index.xml

C:\Users\25022\Documents\hugo-site>hugo server
-D
Watching for changes in C:\Users\25022\Documents\hugo-site\{archetypes,assets,content,data,i18n,layouts,static}
Watching for config changes in C:\Users\25022\Documents\hugo-site\hugo.toml
Start building sites …
hugo v0.145.0-666444f0a52132f9fec9f71cf25b441cc6a4f355+extended windows/amd64 BuildDate=2025-02-26T15:41:25Z VendorInfo=gohugoio

WARN  found no layout file for "html" for kind "home": You should create a template file which matches Hugo Layouts Lookup Rules for this combination.
WARN  found no layout file for "html" for kind "taxonomy": You should create a template file which matches Hugo Layouts Lookup Rules for this combination.

                   | EN
-------------------+-----
  Pages            |  4
  Paginator pages  |  0
  Non-page files   |  0
  Static files     |  0
  Processed images |  0
  Aliases          |  0
  Cleaned          |  0

Built in 5 ms
Environment: "development"
Serving pages from disk
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop

C:\Users\25022\Documents\hugo-site>http://localhost:1313/http://localhost:1313/
'http:' 不是内部或外部命令，也不是可运行的程序
或批处理文件。

C:\Users\25022\Documents\hugo-site>git init
Reinitialized existing Git repository in C:/Users/25022/Documents/hugo-site/.git/

C:\Users\25022\Documents\hugo-site>git remote
 add origin https://github.com/Git-SXQ6/Git-S
XQ6.github.io.git

C:\Users\25022\Documents\hugo-site>git add .
warning: in the working copy of 'public/categories/index.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/index.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/sitemap.xml', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'public/tags/index.xml', LF will be replaced by CRLF the next time Git touches it

C:\Users\25022\Documents\hugo-site>git commit
 -m"Initial commit"
On branch master
nothing to commit, working tree clean

C:\Users\25022\Documents\hugo-site>git push -
u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Git-SXQ6/Git-SXQ6.github.io.git'

C:\Users\25022\Documents\hugo-site>git branch

* master

C:\Users\25022\Documents\hugo-site>git branch
 -m master main

C:\Users\25022\Documents\hugo-site>git push -
u origin main
remote: Repository not found.
fatal: repository 'https://github.com/Git-SXQ6/Git-SXQ6.github.io.git/' not found

C:\Users\25022\Documents\hugo-site>git remote
 -v
origin  https://github.com/Git-SXQ6/Git-SXQ6.github.io.git (fetch)
origin  https://github.com/Git-SXQ6/Git-SXQ6.github.io.git (push)

C:\Users\25022\Documents\hugo-site>git remote
 set-url origin https://github.com/Git-SXQ6/G
it-SXQ6.github.io.git

C:\Users\25022\Documents\hugo-site>git push -
u origin main
remote: Repository not found.
fatal: repository 'https://github.com/Git-SXQ6/Git-SXQ6.github.io.git/' not found

C:\Users\25022\Documents\hugo-site>git push -
u origin main
To https://github.com/Git-SXQ6/Git-SXQ6.github.io.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Git-SXQ6/Git-SXQ6.github.io.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Users\25022\Documents\hugo-site>git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.13 KiB | 105.00 KiB/s, done.
From https://github.com/Git-SXQ6/Git-SXQ6.github.io
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

C:\Users\25022\Documents\hugo-site>git pull origin main --allow-unrelated-histories
From https://github.com/Git-SXQ6/Git-SXQ6.github.io
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 README.md | 16 ++++++++++++++++
 1 file changed, 16 insertions(+)
 create mode 100644 README.md

C:\Users\25022\Documents\hugo-site>git add .

C:\Users\25022\Documents\hugo-site>git commit
 -m"Merged changes from remote with local cha
nges"
On branch main
nothing to commit, working tree clean

C:\Users\25022\Documents\hugo-site>git push -
u origin main
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 16 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (15/15), 1.60 KiB | 1.60 MiB/s, done.
Total 15 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/Git-SXQ6/Git-SXQ6.github.io.git
   03ab567..0f12efe  main -> main  ^A^A^A
branch 'main' set up to track 'origin/main'.
C:\Users\25022\Documents\hugo-site>
C:\Users\25022\Documents\hugo-site>

```
