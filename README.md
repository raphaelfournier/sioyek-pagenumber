# Sioyek: visually select some pages from a document

Put this in `.config/sioyek/prefs_user.config`:

```
new_command	_mypage bash /home/raph/.scripts/pagenumber.sh %{file_name} %{page_number}
```

and that in `.config/sioyek/keys_user.config`:

```
_mypage !
```

So that when you press `!`, the script `pagenumber.sh` gets called. It should
just append the current page number into a file (with a filename close to the
current file).

**To get started, do not forget to change the `/home/raph/` sequence in
`prefs_user.config` and in `pagenumber.sh`**
