---
description: converts from `stdin` to command line arguments
---

# 5⃣ xargs

Some commands accept command line arguments only, so we have to use `xargs` in order to achieve the desired result

```sh
For example

cat filenames.txt | echo
```

The wouldnt execute without `xargs` as `echo` accepts command line arguments only

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.23.20 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.23.38 AM.png" alt=""><figcaption></figcaption></figure>

### Create files given in a file called \`filenames.txt\`&#x20;

```sh
cat filenames.txt | xargs touch 
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-13 at 5.24.49 AM.png" alt=""><figcaption></figcaption></figure>
