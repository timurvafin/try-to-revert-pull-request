Try to revert merged pull request
=================================

1. Always Use the Green Button!
2. Revert merged pull request.

```bash
gco -b revert-pr-1
git revert -m 1 40a7
ggpush
```

Open and merge pull request

3. Fix the original pull request.

```bash
gco master
ggpull
gco -b fix-pr-1
git revert 8382
ga .
gc -m 'Fixup original pull request'
ggpush
```

Open and merge pull request
