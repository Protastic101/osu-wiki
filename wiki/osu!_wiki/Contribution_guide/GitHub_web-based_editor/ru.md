# Веб-редактор GitHub

*Примечание: в этой статье указаны сочетания горячих клавиш для Windows.*\
*См. также: [The github.dev web-based editor - GitHub Docs](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor)*

[github.dev](https://github.dev) — это публичная веб-версия [Visual Studio Code](https://code.visualstudio.com), настроенная на работу с GitHub и принадлежащая его владельцам. Она намного удобнее встроенного редактора GitHub и имеет больше инструментов и возможностей. При работе с osu! wiki рекомендуется пользоваться именно github.dev, особенно если вы правите несколько статей сразу.

## Навигация

*Примечание: чтобы работать с osu! wiki, сначала нужно **[сделать форк репозитория `ppy/osu-wiki`](/wiki/osu!_wiki/Contribution_guide#редактирование-вики).***

Чтобы открыть osu! wiki в веб-редакторе, откройте форк и либо замените `github.com` в адресе на `github.dev`, либо нажмите на точку (`.`) на клавиатуре.

::: Infobox
![](img/command-palette.gif "Пример использования палитры команд")
:::

До всех меню можно добраться и через интерфейс, но удобнее всего перемещаться по редактору, пользуясь **палитрой команд**:

- Нажмите `F1` и введите название действия или настройки, к которой хотите перейти. Если ничего не нашлось, поищите название нужного пункта, кликнув по трём полоскам (`≡`) в левом верхнем углу.
- Чтобы быстро открыть файл, нажмите `Ctrl` + `P` и введите часть его имени.

## Создание веток

Посте того, как вы прочли раздел «[Как правильно работать с вики § Внесение правок](/wiki/osu!_wiki/Contribution_guide/Best_practices#внесение-правок)», создайте под ваши изменения отдельную ветку.

1. Кликните по имени текущей ветки в левом нижнем углу, или нажмите `F1` и введите `branch`, чтобы показать имеющиеся ветки.

  - Выберите пункт `Create new branch...`, введите имя новой ветки и нажмите `Enter`.
  - Чтобы через несколько дней вспомнить, над чем вы работали, выбирайте содержательное имя. Например, ветку для русского перевода статьи [Beatmap discussion](/wiki/Beatmap_discussion) можно назвать `ru-modding-v2`.

2. Чтобы в будущем вернуться к своим изменениям, откройте список веток и выберите нужную.

## Редактирование

### Существующие файлы

1. Чтобы быстро открыть файл, нажмите `Ctrl` + `P` и введите его название, а затем нажмите `Enter`. Редактор умеет искать по неполным совпадениям: если вы напишете `nominators veto ru`, то сможете найти файл `wiki/People/The_Team/Beatmap_Nominators/Beatmap_Veto/ru.md`.
2. Отредактируйте файл. Незакоммиченные изменения **хранятся в браузере** на вашем компьютере — к ним можно будет вернуться даже после ухода с `github.dev`.
3. Когда всё будет готово, [закоммитьте изменения](#коммит-изменений).

### Новые статьи и переводы

Каждая статья хранится в отдельной папке в виде оригинального текста (`en.md`) и переводов в файлах с похожим наименованием.

- Чтобы добавить новый **перевод** имеющейся статьи, кликните правой клавишей по её папке и создайте новый файл с именем, состоящим из [одного из языковых кодов](/wiki/Article_styling_criteria/Formatting#локали) и расширения `.md`.
- Для новой **статьи** нужно будет сделать чуть больше:
  - Создайте в нужной категории папку [с нужным названием](/wiki/Article_styling_criteria/Formatting#файловая-структура). Если у статьи нет имеющейся логической категории, создайте её папку в директории `/wiki/`.
  - В новой папке создайте файл `en.md` и вставьте туда текст статьи.

### Операции с файлами

- Чтобы открыть встроенный проводник по файлам, нажмите `Ctrl` + `Shift` + `E`.
- Файлы и папки можно перемещать, перетаскивая их курсором мыши. Чтобы выделить несколько объектов, зажмите `Ctrl`.
- Удалять или переименовывать объекты можно с помощью контекстного меню или горячих клавиш из Проводника Windows.
- Чтобы залить файл в редактор, перетащите его в нужное место в проводнике.

## Коммит изменений

::: Infobox
![](img/commit-and-push.gif "Чтобы сохранить изменения, их нужно закоммитить")
:::

1. Откройте список изменённых файлов, нажав `Ctrl` + `Shift` + `G`.
2. Прокликайте `+` около файлов, которые вы хотите вместе сохранить.
3. Опишите на английском свои изменения. **Давайте коммитам ёмкие и понятные описания**, чтобы другие люди могли сразу понять суть изменений.
4. Нажмите `Ctrl` + `Enter` или кликните по кнопке `✓`, чтобы закоммитить и выгрузить свои изменения.

## Что дальше?

Когда вы закончили вносить правки, откройте список из раздела «[Руководство по работе с osu! wiki § Самопроверка](/wiki/osu!_wiki/Contribution_guide#self-check)» и пройдитесь по нему. После этого [откройте пулл-реквест](/wiki/osu!_wiki/Contribution_guide#пулл-реквест) в репозитории `ppy/osu-wiki`.
