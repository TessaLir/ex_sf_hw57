# Docker LAMP

Выполнено в рамках обучающей программы SkillFactory.

## Инструкция

В дерикторрии `code` располагается код будущих систем. Для нового проекта, требуется создать новую дерикторию

В дерикторрии `dbdata` при поднятии Docker образов будут храниться закешированные данные с MySQL. Для данного репозитория, что бы папка была в GIT был создан пустой файл `.local`

В дерикторрии `fpm` располагается конфигурационные настройки `php.ini` и это стандартный контейнер для PHP-FPM. **Вносить изменения при добалвлении новых подпроектов не нужно**.

В дерикторрии `mysql` располагается конфигурационные настройки `my.cnf` и это стандартный контейнер для MySQL.

В дерикторрии `nginx` выполняется настройка Nginx. В директории `./hosts` необходимо создавать новую директорию, для отдельного сайта-проекта. Так же в `Dockerfile` требуется создавать для данного проекта-сайта свой `COPY ****`

`docker-compose` редавтрировать при добавлении сайтов-проектов, не требуется.