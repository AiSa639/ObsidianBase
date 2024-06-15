документация: [01 Start here - Git Documentation - Obsidian Publish](https://publish.obsidian.md/git-doc/01+Start+here)


1) Cгенерировать PERSONAL_ACCESS_TOKEN, который будет использоваться вместо **пароля**. 

	Github -> Settings -> Developer Settings -> Personal Access Token -> Tokens (classic) -> Generate New Token


Создать репозиторий (HTTPS)
>https://github.com/AiSa639/ObsidianBase.git

**Username** 
>{USERNAME_В_GITHUB}

**Password** 
>{PERSONAL_ACCESS_TOKEN}


# Для MacOs

## Открытие боковой view-шки в Obsidian:

Для **открытия** git view:
> Obsidian git: Open source and control view

![[Pasted image 20240616034034.png]]

##  Установка

1) Установка и настройка Git с терминала (вариант с Xcode):
>  xcode-select --install
>  sudo xcode-select --reset
>  git config --global credential.helper osxkeychain

2) Инициализировать git-репозиторий

либо с самого Obsidian:
> Obsidian Git: Initialize a new repo

либо c терминала
>     git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/AiSa639/ObsidianBase.git
git push -u origin main


3) Открыть приложение "Связка ключей"
 ![[Pasted image 20240616033728.png]]

> Связка ключей -> Связки ключей по умолчанию ->  Вход ->  Создать новый объект связки ключей

**Инструкция** по заполнению:

![[Pasted image 20240616032134.png]]

4) Настроить в Obsidian Git регулярный **backup** (commit & push) и **pull**.

![[Pasted image 20240616041907.png]]

# Для Android

## Гит клиент

Скачать гит-клиента - [Приложения в Google Play – MGit](https://play.google.com/store/apps/details?id=com.manichord.mgit&pcampaignid=web_share)
Нужен чтобы скачать свой репозиторий.
Остальные функции (commit, pull, push и т.д) можно вызывать из самого Obsidian. 

## Настройки Obsidian Git
В настройках Obsidian Git ввести данные:
- Commit author
- Commit email
- Username - USERNAME_В_GITHUB
- Password - PERSONAL_ACCESS_TOKEN

# Для iOS
## Гит клиент
Скачать гит-клиента - [PolyGit Git Client on the App Store](https://apps.apple.com/us/app/polygit-git-client/id1508942822)
Нужен чтобы скачать свой репозиторий.
Остальные функции (commit, pull, push и т.д) можно вызывать из самого Obsidian. 

Нужно скопировать скачанный проект в папку Obsidian

> Мой iPhone -> PolyGit -> ObsidianBase

скопировать в:

>  Мой iPhone ->  Obsidian


## Настройки Obsidian Git
В настройках Obsidian Git ввести данные:
- Commit author
- Commit email
- Username - USERNAME_В_GITHUB
- Password - PERSONAL_ACCESS_TOKEN

# Настройка .gitignore (optional)

Чтобы применить настройки изменения .gitignore:

>git rm -rf --cached .
 git add .
