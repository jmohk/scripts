1) Find all the SUID/SGID executables

```bash
find / -type f -a \( -perm -u+s -o -perm -g+s \) -exec ls -l {} \; 2> /dev/null
```
2) Find SUID Files

```bash
find / -perm -u=s -type f 2>/dev/null
```
