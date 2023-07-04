# my-git-repo
## 2. Клонирование репозитория

### Задание
- Клонируйте репозиторий "my-git-repo" на свой компьютер с использованием команды `git clone`.
- Убедитесь, что репозиторий успешно склонирован на ваш компьютер.

### Решение
```bash
git clone git@github.com:gram-code/my-git-repo.git
cd my-git-repo
ls -alh
```

## 3. Добавление файлов и коммит

### Задание
- Внесите некоторые изменения в файл `README.md`, добавьте некоторый текст или контент.
- Используйте команду `git status`, чтобы увидеть, какие файлы были изменены.
- Используйте команду `git add`, чтобы добавить измененные файлы в индекс.
- Используйте команду `git commit`, чтобы зафиксировать изменения с информативным сообщением о коммите.
- Повторите процесс изменения файлов, добавления в индекс и коммита несколько раз.

### Решение
Внесли некоторые изменения в `README.md`. Вывод команды `git status`:
```bash
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
Добавим изменения с помощью команды `git add`:
```bash
git add README.md
```
Создадим коммит:
```bash
git commit -m "Added info in README.md"
```
И запушим на GitHub
```bash
git push
```
Сделаем еще один коммит и запушим его
```bash
git add README.md
git commit -m "Added info in README.md - second commit"
git push
```

## 4. Использование `.gitignore`
### Задание
- Создайте файл `log.txt` и напишите в нем некоторый текст.
- Создайте файл `notes.txt` и напишите в нем некоторый текст.
- Создайте файл `.gitignore` в корневом каталоге вашего репозитория.
- В файле `.gitignore` добавьте следующие строки: `log.txt`. Это гарантирует, что файл `log.txt` будет игнорироваться Git.
- Сохраните изменения в файле `.gitignore` и зафиксируйте его в вашем репозитории.
- Убедитесь, что файл `log.txt` больше не отображается при выполнении команды `git status`, но файл `notes.txt` по-прежнему видим.

### Решение
Cоздадим файлы
```bash
echo "некоторый текст" > log.txt
echo "некоторый текст" > notes.txt
echo "log.txt" > .gitignore
```

Фиксируем изменения
```bash
git add README.md .gitignore README.md
git commit -m "Task No. 4"
git push
```
