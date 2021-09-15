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

Запустить службу. После внедрения systemd постоянно путался и сначала писал имя службы, а потом команду start. Сейчас уже переучился. 
systemctl start mysql

Добавить в автозагрузку:
systemctl enable nginx

Добавить сервис в автозагрузку и сразу запустить. Заменяет две предыдущие команды. Я не так давно узнал и стал использовать именно объединённую команду:
systemctl enable --now mariadb

Перечитать настройки служб. Обязательно нужно выполнить после того, как изменили какие-то настройки юнитов systemd.
systemctl daemon-reload

Список всех unit-files, а так же их состояний:
systemctl list-unit-files
Список выше можно ограничить по типам:
systemctl -t service
systemctl -t timer
systemctl -t mount

Посмотреть статус конкретной службы:
systemctl | grep ssh

Проверить статус автозапуска:
systemctl is-enabled nginx

Посмотреть конфигурацию юнита:
systemctl cat sshd