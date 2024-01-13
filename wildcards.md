---
description: >-
  A wildcard is a character or a string of characters that can be used as a
  substitute for any other character(s) in a command-line expression.
---

# 6⃣ Wildcards

* `*` - zero or more characters
* `?` - single character
* `[]` - range of characters

```sh
ls -l file*
```

this command prints all the files with expression `file` and anything after that. More clearly, it prints files starting with `file` and upto any characters after that.

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.38.20 AM.png" alt=""><figcaption><p>prints file with <code>file</code> as starting</p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.40.55 AM.png" alt=""><figcaption><p>prints only <code>txt</code> files</p></figcaption></figure>

```sh
ls -l [abc]123
```

can only have characters a,b and c and 123 after that

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.43.27 AM.png" alt=""><figcaption></figcaption></figure>

```sh
ls -l ?[123]
```

prints files with any first character and after that any number from 1-3

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.46.03 AM.png" alt=""><figcaption></figcaption></figure>

* `^` - beginning of line

```sh
cat states.txt | grep ^A
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.49.22 AM.png" alt=""><figcaption></figcaption></figure>

* `$` - end of line

```sh
cat states.txt | grep sh$
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.50.01 AM.png" alt=""><figcaption></figcaption></figure>
