---
title: 'Filter Json Array Using Jq'
date: 2021-10-06
type: docs
---
## Filter JSON array using jq

If you are trying to find a specific element within a JSON array you can use jq's `select()` filter.

Example:

```bash
jq '.services[] | select(.name == "awesome-service") | .version' services.json
```

