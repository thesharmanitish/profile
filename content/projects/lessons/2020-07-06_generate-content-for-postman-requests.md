---
title: 'Generate Content For Postman Requests'
date: 2020-07-06
type: docs
aliases:
  - /projects/til/2020-07-06_generate-content-for-postman-requests/
---
## Generate content for Postman requests

Postman provides dynamic variables which can be used to generate content for requests e.g.

```json
{
    "name": "Test Variant {{\$randomInt}}",
    "id": "{{\$guid}}"
}
```

See: https://learning.postman.com/docs/postman/variables-and-environments/variables-list/

