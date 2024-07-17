## Шпаргалка по git
**Git (Global Information Tracker) - система контроля версий (Version Control System - VCS)**, позволяющая хранить, изменять и анализировать историю изменений продукта, а также синхронизировать изменения между участниками команды.

Git реализует интерфейс командной строки - Command-line Interface (CLI).


### Базовые команды CLI:
```bash
pws, cd, ls, touch, mkdir, mkdir -p, cp что [что[ что]] куда, mv, cat, rmdir, rm -r, grep, clip, pbcopy (mac)

~  &&  ||  &  |  ;  !!  !$  !^  !:2
```

### Настройки git
~/.gitconfig
```bash
git config -l
git config user.name "" && git config user.email ""
```

#### Инициализация
git init

#### Обслуживание 
git status

git add --all

git commit -m ""

git log

#### Генерация SSH
**SSH (Secure Shell Protocol)** - протокол обмена данными по сети. Для Git генерируется два ssh-ключа в ~/.ssh. 
```bash
ssh-keygen -t ed25519 -C "git@email"
ssh-keygen -t rsa -b 4096 -C "git@mail"
ssh -T git@github.com #проверка
```

#### Добавление удаленного репозитория
```bash
git remote add origin адрес
git remote -v #проверка
```

#### Отправка изменений
git push -u origin main #для новых веток

#### Работа с ветками
git branch -M main