---
description: Pipes are used to redirect a stream from one program to another program
---

# 3⃣ Pipe in Linux

\-> The output of one commad redirect it to the input of other command

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 3.51.22 AM.png" alt=""><figcaption></figcaption></figure>

## Pipe syntax

We use '|' symbol to separate two commands. Output of first command passed to second command

```
command1 | command2
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 3.58.26 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 3.56.11 AM.png" alt=""><figcaption></figcaption></figure>

## Q1. Find number of files in a directory

```sh
ls -1 | wc -l
```

### Breakdown of the command used above

```sh
ls -1 
```

The command lists all files in a directory in a single column i.e. a single line represents name of one file.

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.05.39 AM.png" alt=""><figcaption><p>Output of ls command</p></figcaption></figure>

```sh
wc -l
```

This prints the number lines in file. Together the commands will print the number of files in a directory.

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.08.12 AM.png" alt=""><figcaption></figcaption></figure>

## Q2. Combine two files and sort them

Combining 2 files using cat command and then sorting them using pipe

```sh
cat file1.txt file2.txt | sort
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.14.13 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.15.21 AM.png" alt=""><figcaption><p>sorted output of concatenation of two files</p></figcaption></figure>



## Q3. Unique names in a file

{% code fullWidth="true" %}
```sh
cat file3.txt | sort | uniq
```
{% endcode %}

We can only use `uniq` command with sorted data only

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.24.01 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.22.44 AM.png" alt=""><figcaption></figcaption></figure>



## Q4. See 30-37 lines in a file

`head -37` to view first 37 lines , `tail -7` to view last 7 lines from the 37 lines, which makes 30-37

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 4.54.56 AM.png" alt=""><figcaption></figcaption></figure>

## Tee command -&#x20;

`tee` command reads from _**stdin**_ and saves the content to a file and also displays it to _**stdout**_

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.03.51 AM.png" alt=""><figcaption><p>writes and displays output of the ls command</p></figcaption></figure>
