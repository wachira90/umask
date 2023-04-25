# umask
umask setting

## Check Umask 

```bash
ubuntu@DESKTOP-MKE4SPH:~$ umask
0022
ubuntu@DESKTOP-MKE4SPH:~$
```

### To permanently change your umask you need to update your shell profile:

```bash
~/.profile
~/.bashrc
~/.zshrc
~/.cshrc
```

### OR

```bash
/etc/profile   
/etc/bashrc 
/etc/.bash_profile    
/root/.bashrc   
/root/.bash_profile
```

## How to setting

Place end file  Relogin and test

```bash
umask 0027
```

### Table setting general

| Umask	File | result | Directory result |
|----|----|----|
| 000 | 666 rw- rw- rw-| 777 rwx rwx rwx |
| 002 | 664 rw- rw- r--| 775 rwx rwx r-x |
| 022 | 644 rw- r-- r--| 755 rwx r-x r-x |
| 027 | 640 rw- r-- ---| 750 rwx r-x --- |
| 077 | 600 rw- --- ---| 700 rwx --- --- |
| 277 | 400 r-- --- ---| 500 r-x --- --- |

### Table setting 

| Umask	File | result | Directory result |
|----|----|----|
| 0000 | 0666 rw- rw- rw-| 0777 rwx rwx rwx |
| 0002 | 0664 rw- rw- r--| 0775 rwx rwx r-x |
| 0022 | 0644 rw- r-- r--| 0755 rwx r-x r-x |
| 0027 | 0640 rw- r-- ---| 0750 rwx r-x --- |
| 0077 | 0600 rw- --- ---| 0700 rwx --- --- |
| 0277 | 0400 r-- --- ---| 0500 r-x --- --- |

