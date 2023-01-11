# umask
umask setting

## check umask 

```
ubuntu@DESKTOP-MKE4SPH:~$ umask
0022
ubuntu@DESKTOP-MKE4SPH:~$
```

### To permanently change your umask you need to update your shell profile:

```
~/.profile
~/.bashrc
~/.zshrc
~/.cshrc
```
### table setting 

| Umask	File | result | Directory result |
|----|----|----|
| 000 | 666 rw- rw- rw-| 777 rwx rwx rwx |
| 002 | 664 rw- rw- r--| 775 rwx rwx r-x |
| 022 | 644 rw- r-- r--| 755 rwx r-x r-x |
| 027 | 640 rw- r-- ---| 750 rwx r-x --- |
| 077 | 600 rw- --- ---| 700 rwx --- --- |
| 277 | 400 r-- --- ---| 500 r-x --- --- |

```
Umask	File result	Directory result
000	666 rw- rw- rw-	777 rwx rwx rwx
002	664 rw- rw- r–	775 rwx rwx r-x
022	644 rw- r-- r–	755 rwx r-x r-x
027	640 rw- r-- —	750 rwx r-x —
077	600 rw---- —	700 rwx — —
277	400 r-- — —	500 r-x — —
```
