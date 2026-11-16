---
title: 'Interactive Prompt Starts'
date: 2021-01-15
type: docs
aliases:
  - /projects/til/2021-01-15_renew-an-expired-pgp-key/
---
## Renew an expired PGP key

```bash
gpg --list-keys 2>/dev/null | grep <your_email> -C2
gpg --edit-key <the_key_id_you_want>

# interactive prompt starts
key 0 
# note you will not see a * next to the key, but unless there
# is an error the key is selected
expire
1y
key 1
expire
1y
# ... for all keys and subkeys
save

# publish the change
gpg --keyserver pgp.mit.edu --send-keys <the_key_id_you_want>
```

