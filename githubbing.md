# some tips

### getting an error trying to push?
```
$ git push
error: The requested URL returned error: 403 Forbidden while accessing https://github.com/ewilbanks/lab_general.git/info/refs

fatal: HTTP request failed
```
### try this
`git remote set-url origin https://username@github.com/user/repo.git`

