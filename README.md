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
- Внесли некоторые изменения в `README.md`.
- Вывод команды `git status`:
```bash
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
- Добавим изменения с помощью команды `git add`:
```bash
git add README.md
```
- Создадим коммит:
```bash
git commit -m "Added info in README.md"
```
- И запушим на GitHub
```bash
git push
```
- Сделаем еще один коммит и запушим его
```bash
git add README.md
git commit -m "Added info in README.md - second commit"
git push
```


