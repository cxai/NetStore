# AppSec Demo .Net App

Based on the bookstore app with improved code security in each successive commit

Commits are tagged v1, v2 and v3

javalibs.zip is a set of vulnerable open source jars (struts 2.5.10)

## How to recreate

create github repo

mkdir NetStore
create README.md

```
cd NetStore/

cp -R "Bookstore_CS-SCAN 3" .
git add *
git commit -am "First commit"
git tag v1

cp -R "Bookstore_CS-SCAN 2" .
git commit -am "Second commit"
git tag v2

cp -R "Bookstore_CS-SCAN 0" .
git commit -am "Third commit"
git tag v3

git remote add origin yourlink/NetStore.git
git push -u origin master --tags
```
