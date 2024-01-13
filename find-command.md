# 2⃣ find command

**Syntax - find \[options] \[path…] \[expression]**

## 1. Search file based on their size

```sh
 find /path/ -size 50M 
```

* M for MB
* k for KB
* G for GB
* c for bytes

## 2. Find a filetype in a given path

```sh
find /path/ -type f
```

* f for file
* d for directory
* l for symbolic link
* b for block device
* s for socket

## 3. Ignore upper and lowercase in file name while searching files

```sh
find /path/ -iname <file_name>
```

## 4. Search files for a given user only

```sh
find /path/ -user root
```

## 5. Search a file based on their permissions

```sh
find /path/ -perm /u=r 
find /path/ -perm 777
```

## 6. Search all files that start with letter \`a\`&#x20;

```sh
find /path/ -iname a*
```

## 7. Search all files which are modified/created after last.txt file

```sh
find /path/ -newer last.txt
```

## 8. Search all empty files in a directory

```sh
find /path/ -empty
```

## 9. **Find and delete empty files**

```sh
find /path/ -empty -delete
```

## 10. Search all files whose size are between 1-50MB

```sh
find /path/ -size +1M -size -50M
```

## 11. Search 15 days old files

```sh
find /path/ -mtime 15
```
