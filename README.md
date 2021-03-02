# git_HW
Первая попытка. https://github.com/Gazman2013/Git

111. git config --global user.email "rodionov.gazman2013@gmail.com"
112. git init
1. Создать отдельный репозиторий на github.
2. Создать локально три текстовых файла.
3. Поместить в стейдж, закомитить, запушить.
4. Создать две новые ветки.
5. Внести изменения в ветку 1 и 2 
6. Смерджить между собой вновь созданные ветки.
7. Смерджить ветку с веткой мастер
8. Отменить предыдущий комит
9. Все изменения запушить в гит репозиторий.

1. mkdir dev
2. cd dev
3. touch HW1.txt HW2.txt HW3.txt
4. git status
5. git add * начать отслеживать (добавить под версионный контроль) новые файлы
6. root@instance-3:/home/dev# git status определяем состояние файлов
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   HW1.txt
        new file:   HW2.txt
        new file:   HW3.txt

7. git commit -m "test commit" фиксация изменений
[master (root-commit) 6462711] test commit
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 dev/HW1.txt
 create mode 100644 dev/HW2.txt
 create mode 100644 dev/HW3.txt

8.  git push https://github.com/
9. git branch one
10. git branch two
11. git checkout one
12. echo "test1" > one.txt
13. git add .
14. git commit -m "Edit one.txt"

15. git checkout two
16. Switched to branch 'two'
17. echo "test2" > two.txt
18. git add .
19. git commit -m "Edit two.txt"

20. git merge one  -m "Merge two with one"

21. git checkout main
22. git merge two -m "Merge main with two"

23. git reset --hard HEAD~1
24. git push
