# Find
✰✰✰✰✰✰
## **-type**
> Input 
```
$ find ~/public -type d
```

> Output 
```
/Users/simonscholar/public
/Users/simonscholar/public/Drop Box
```

> Explanation

**- This command filters the search result by only listing the directories within the user's home directory and its subdirectories.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

> Input
```
$ find ~/public -type f
```

> Output
```
/Users/simonscholar/public/.localized
/Users/simonscholar/public/Drop Box/.localized
```

> Explanation

**- This command specifies the type of search result by only listing the regular files within the user's home directory and its subdirectories.** 

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

## **-empty**
> Input 
```
$ find ~ -type f -empty
```

> Output
```
/Users/simonscholar/Music/.localized
/Users/simonscholar/Pictures/.localized
find: /Users/simonscholar/Pictures/Photos Library.photoslibrary: Operation not permitted
/Users/simonscholar/Desktop/code shit/Icon
```

>Explanation

**- The command searches for empty files within the user's home directory and subdirectories.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

> Input
```
$ find ~ -type d -empty
```

> Output
```
find: /Users/simonscholar/Pictures/Photos Library.photoslibrary: Operation not permitted
/Users/simonscholar/Library/Application Support/com.apple.replayd
/Users/simonscholar/Library/Application Support/SyncServices/Local/ClientsWithChanges
/Users/simonscholar/Library/Application Support/Mozilla/Extensions
```

> Explanation

**- The command searches for empty directories within the user's home directory and subdirectories.** 

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

## **-mtime**
> Input 
```
$ find technical/911report -mtime +12
```

> Output 
```
technical/911report
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-13.1.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
```

> Explanation

**- This command gives you a list of files in the directory `technical` that has been modified more than 12 days ago.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

> Input
```
$ find technical/911report -mtime +13
```

> Output
```

```

> Explanation

**-  This command gives you a list of files in the directory `technical` that has been modified more than 13 days ago, in which are none.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

## **-size**
> Input 
```
$ find technical -size 1
```

> Output 
```
technical
technical/government
technical/government/Env_Prot_Agen
technical/government/Alcohol_Problems
technical/government/Post_Rate_Comm
```

> Explanation

**-This command gives you a list of files within the `technical` directory that have a size of 1 block.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰

> Input
```
$ find technical -size 2
```

> Output
```
technical/government/About_LSC
technical/plos/pmed.0020191.txt
technical/plos/pmed.0020226.txt
technical/911report
```

> Explanation

**- This command gives you a list of files within the `technical` directory that have a size of 2 blocks.**

>[Citation](https://www.redhat.com/sysadmin/linux-find-command#:~:text=The%20find%20command%20is%20one,and%20not%20just%20by%20filename.)

✰✰✰✰✰✰
