# Regex - regular expression notes


## Notes

```bash
# go to root
cd /

```

- tail -> outputs the end of a file
- head -> outputs the beginning of a file

Use `grep -E` for regex search
```bash
# always use single quote
grep -E 'root' passwd 
```

'^root' -> starts with 'root'
'bash$' -> ends with 'bash'

# character class [] and quantifier +
head passwd | grep -E
'^[a]' -> matches all that starts with 'a'
'^[ko]' -> starts with k OR o
'^[a-z]+' -> matches all that starts with characters between a-z
'[a-z]+' -> matches all character small a-z
'[a-zA-Z0-9]+' -> matches a-z A-Z and numbers 0-9
'[^a-z]+' -> matches everything else besides a-z
'[0-9]{4}' -> matches those number with 4 digits
'(bash|sync)$' -> ends for 'bash' or 'sync'

grep -E '/home[^:]+' -> matches characters after 'home' before ':'

### /etc

directory for system config files -> applies to all users in the system

ex: `/etc/passwd` contains info about users




