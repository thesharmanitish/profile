---
title: 'Example'
date: 2016-05-18
type: docs
aliases:
  - /projects/til/2016-05-18_copy-paste-for-files-in-linux/
---
## Copy paste for files in linux

`xclip` is an awesome tool which can be used to pipe output to the clipboard. Use `-selection c` so that you can paste using `Ctrl` + `V`.

```bash
# example
xclip -selection c ~/somefile.txt
```
