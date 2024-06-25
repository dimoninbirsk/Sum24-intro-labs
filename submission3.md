# Lab3 Version Control

## Task 1: Understanding Version Control Systems

1. ```Git Log``` to find __commit hash__
``` 
PS A:\Project\devops-labs\Sum24-intro-labs> git log
commit 3bd17ee295ad882de6dbe8987631a2029a0583a4 (HEAD -> lab-3-kolokolov-dmitriy)
Author: dimoninbirsk <dimoninbirsk@gmail.com>
Date:   Tue Jun 25 12:51:51 2024 +0300

    Commit №3

Author: dimoninbirsk <dimoninbirsk@gmail.com>
Date:   Tue Jun 25 12:51:18 2024 +0300
```

2. ```git cat-file -p f02292aca82fc7de6064b379ce83a9ce66bdc61e``` to inspect the __commit hash__
```
PS A:\Project\devops-labs\Sum24-intro-labs> git cat-file -p b90da87936aa59f4769559bd2b62a3e76f683dd4
tree f02292aca82fc7de6064b379ce83a9ce66bdc61e
parent bff366f80cc728443e2be3e65c274854bfcf54ad
author dimoninbirsk <dimoninbirsk@gmail.com> 1719309078 +0300
committer dimoninbirsk <dimoninbirsk@gmail.com> 1719309078 +0300
```

3. ```git cat-file -p f02292aca82fc7de6064b379ce83a9ce66bdc61e``` to inspect the __tree hash__
```
PS A:\Project\devops-labs\Sum24-intro-labs> git cat-file -p f02292aca82fc7de6064b379ce83a9ce66bdc61e
100644 blob ede183da8ef201e5f5737eea502edc77fd8a9bdc    README.md
100644 blob 5738bc15a0416ad2624df13badfb235052777e79    index.html
100644 blob c54a520ec380d5cc77c55f2e40fe921fc5580de5    lab1.md
100644 blob 1b99cc0044f93f556a0f6a599c7edf2f33f4944a    lab2.md
100644 blob 2f8463cc188ec6ca69ae7a0f98d38e132280becb    lab3.md
040000 tree 37b67809f46a68cbe58e807e891c5376a822bc3d    lab3
100644 blob ee2e111d04704f3b786d6de30381034edc0fefb6    lab4.md
```
```
PS A:\Project\devops-labs\Sum24-intro-labs> git cat-file -p 37b67809f46a68cbe58e807e891c5376a822bc3d
100644 blob d5681d168131ce13ff70fa8425dfb433edc566f1    file.md
```
4. ```git cat-file -p d5681d168131ce13ff70fa8425dfb433edc566f1``` to inspect __BLOB__
```
# Some text

# Even more text
```