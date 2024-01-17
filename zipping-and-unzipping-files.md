---
description: gzip, gunzip, tar
---

# 7⃣ zipping and unzipping files

## gzip

gzip (GNU zip)  - used to compress individual files(single files only)

**Note: replaces original file with zipped file**

Usage ->

```sh
gzip [filename]
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-16 at 10.47.03 PM.png" alt=""><figcaption></figcaption></figure>

## gunzip

By default it replaces the compressed file with decompressed file

```shell
gunzip [filename]
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-16 at 10.51.46 PM.png" alt=""><figcaption></figcaption></figure>

### By using \`-k\` we can keep the original compressed file too

```
gunzip -k [filename]
```

<figure><img src=".gitbook/assets/Screenshot 2024-01-17 at 11.34.36 PM.png" alt=""><figcaption></figcaption></figure>

