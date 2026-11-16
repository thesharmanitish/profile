---
title: 'Watch A Single File For Any Type Of Changes And Display On Change'
date: 2016-12-12
type: docs
aliases:
  - /projects/til/2016-12-12_native-watch-using-inotify-tools/
---
## Native Watch Using `inotify-tools`

Don't bother installing node or ruby gems when you can simply run the following inline command on any UNIX system with inotify-tools installed:

```bash
# watch a single file for any type of changes and display on change
while inotifywait someText.txt; do cat someText.txt; done

# watch a folder for any type of change and run make if there is
while inotifywait -r src; do make; done
```

