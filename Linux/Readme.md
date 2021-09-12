# print working directory
```
pwd
```

# clear console
```
clear
```

# change directory
```
cd
```

# level up
```
cd ..
```
# list file

```
ls
ls docs/s*
ls docs/*.jpg
```
# make directory
```
mkdir
```
# to create multiple levels of directories (e.g. mkdir -p dir1/dir2/dir3)
```
mkdir -p
```
# create file
```
touch file.py
```
# remove file
```
rm file.py
```
# remove directory (--force --recursive)
```
rm -rf
```
# displays network connections
```
netstat -plutn
```
# add ruleto firewall list
```
sudo firewall-cmd --zone=public --add-port=3000/tcp
```

# add permanent rule
```
firewall-cmd --permanent --add-port=3000/tcp
```
# show process
```
ps -aux | grep *name*
```
# add user
```
adduser *username*
```
# add user in sudo group
```
usermod -aG sudo *username*
```
# to add permissions(rwx - read write execute   -R - recursive )
```
chmod -R +rwx *filename/directory*
```