# Мой блог

Это рабочий репозиторий моего блога, доступного по адресу https://noggatur.github.io/.

Поддерживаются посты с разметкой [Markdown](http://daringfireball.net/projects/markdown/) и возможностью вставки формул [LaTeX](https://ru.wikipedia.org/wiki/LaTeX).
Также в постах можно пользоваться [специальными вставками на Ruby](http://octopress.org/docs/plugins/).

## Установка

```sh
git clone git@github.com:noggatur/noggatur.github.io.git blog && cd blog
bundle install
rake install
```

Настраиваем систему публикации
```sh
rake setup_github_pages
  # потом ввести вот это
  git@github.com:noggatur/noggatur.github.io.git

# для того, чтобы можно было спокойно пользоваться "git push"
git push --set-upstream origin source
```

## Доступные команды

Команда | Действие
------- | --------
./run                  | режим разработки на сервере http://localhost:4000/
./run post "Заголовок" | написание нового поста
./run upd              | обновить стили шаблона
./run deploy           | опубликовать текущую версию блога
./run help             | перечень доступных команд


## Дополнительная информация

Блог работает на базе фреймворка [Octopress](http://octopress.org/) и шаблона [Oct2](http://bijumon.github.io/oct2/).