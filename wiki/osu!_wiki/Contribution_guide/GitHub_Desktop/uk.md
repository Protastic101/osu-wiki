---
no_native_review: true
---

# GitHub Desktop

*Ця стаття є продовженням [основної сторінки](/wiki/osu!_wiki/Contribution_guide)* і припускає, що ви будут використовувати [GitHub Desktop](https://desktop.github.com). **Ви можете використовувати й інші Git клієнти за вашим бажанням**. Навіть якщо ви працюєте локально, вам у будь якому випадку потрібен доступ до GitHub, щоб створити пул реквест для внесення ваших змін.

## Встановлення GitHub Desktop

1. Інсталюйте [GitHub Desktop](https://desktop.github.com), якщо його ще немає.
2. Після завершення інсталяції, коли GitHub Desktop попросить увійти до акаунту, натисніть `Sign in to GiHub.com`.
3. Заповніть всі необхідні поля.
4. Перейдіть до [Клонування](#клонування).

## Клонування

1. Натисніть на `Clone a repository`.

2. Це покаже список ваших репозиторіїв; оберіть репозиторій `osu-wiki`.

3. Оберіть куди клонувати репозиторій. Не важливо де саме ви вирішите його зберегти, головне запам'ятайте куди.

   ![](img/github-desktop-select-repo.jpg)

4. Натисніть `Clone`. Це може зайняти деякий час в залежності від вашого з'єднання.

5. Перейдіть до [Створення гілок](#створення-гілок).

## Створення гілок

З технічної точки зору створення нових гілок не є необхідним, але це [дуже рекомендовано по кільком причинам](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow). Назвемо декілька:

- Гілки ізолюють різні логічні зміни одна від одної, тобто ви можете працювати більше ніж над однією статтею одночасно, при цьому вони можуть бути оглянуті та об'єднанні окремо.
- Якщо ваші зміни знаходяться поза гілкою `master`, ви можете [безпечно синхронізувати її](/wiki/osu!_wiki/Contribution_guide/Best_practices#синхронізація-форку) без конфліктів.

1. Натисніть на випадаючий список `Current branch`, що знаходиться зверху меню.

2. Введіть назву гілки. Рекомендовано використовувати підсумок ваших змін, як її назву. Наприклад, редагуючи статтю `Forums`, можна назвати гілку `update-forums`.

   ![](img/github-desktop-branch.jpg)

3. Перейдіть до [Редагування](#редагування).

## Редагування

1. У теці в яку ви склонували репозиторій, перейдіть до файлу який ви хочете редагувати. Статті організовані наступним чином: папки підписані іменами статей у яких файли з розширенням `.md` є локалізаціями.
2. Коли знайдете потрібний файл, відкрийте його у вашому улюбленому текстовому редакторі.
3. Тепер ви можете вносити свої зміни. Також, приділіть хвилинку [самоперевірці](/wiki/osu!_wiki/Contribution_guide#self-check).
4. Перейдіть до [Коміти і пуші](#коміти-і-пуші).

### Переміщення існуючих файлів

1. Використовуйте Провідник Windows для переміщення файлів.
2. Перейдіть до [Коміти і пуші](#коміти-і-пуші).

### Створення нових файлів

*Увага: Якщо ви будете створювати файли статей використовуючи Провідник Windows, переконайтеся, що у вас увімкнена опція `Розширення імен файлів`.* Перегляньте [Поширені розширення імен файлів у Windows](https://support.microsoft.com/uk-ua/windows/поширені-розширення-імен-файлів-у-windows-da4a4430-8e76-89c5-59f7-1cdbbc75cb01) для інструкції.

1. Використовуйте Провідник Windows, ваш улюблений редактор зображень, та/або ваш улюблений текстовий редактор, щоб створювати нові файли. Якщо ви створюєте нові статті або переклади, називайте файли відповідно до [Локалізації в Критеріях Стилізації Статей](/wiki/Article_styling_criteria/Formatting#локалізації).
2. Перейдіть до [Коміти і пуші](#коміти-і-пуші).

### Видалення файлів

1. Використовуйте Провідник Windows для видалення файлів.
2. Перейдіть до [Коміти і пуші](#коміти-і-пуші).

## Коміти і пуші

1. Відкрийте GitHub Desktop. Він повинен виглядати приблизно як тут:

  ![](img/github-desktop-changes.jpg "Ваш може трішки відрізнятися.")

2. За замовчуванням, GitHub Desktop буде автоматично вибирати ваші зміни.
3. Найкраще виділяти кожну "велику" зміну в окремий коміт.

Наприклад, на зображенні вище, [pippi](/wiki/Mascots#pippi) додав нову картинку, редагував файл `en.md`, щоб додати заголовок і прикріпити цю картинку, а також помітив переклади як застарілі. Судячи з цього, ми можемо мати два коміти, один для змін, які стосуються файлу `en.md`, другий для застарілих перекладів.

4. Виберіть файли, які попадуть в коміт.
5. Напишіть короткий підсумок коміту. Він має обмеження в 72 символи і **повинен бути написаний англійською**.
6. Напишіть опис. Писати його не обов'язково, він не має обмеження по кількості символів і може бути написаний будь-якою мовою.

  ![](img/github-desktop-first-commit.jpg "Перший коміт")

7. Натисніть на синю кнопку `Commit to` і, якщо потрібно, повторіть дії з 4 кроку для всіх інших комітів, які ви хочете зробити.

  ![](img/github-desktop-second-commit.jpg "Другий коміт")

8. Коли ви завершили робити коміти, натисніть кнопку `Publish branch`, яка знаходиться зверху.

  ![](img/github-desktop-push.jpg)

9. Перейдіть до [Огляд](/wiki/osu!_wiki/Contribution_guide#review), щоб отримати останню інформацію про пул реквести і внесення змін.
