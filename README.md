# GitHub_HW_2

### 1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing
```
git branch "имя ветки"
```
### 2. Запушить все ветки на внешний репозиторий
```
git push origin --all
```
### 3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
```
git checkout Bag_Reports
touch bug_report_structure.txt
vim bug_report_structure.txt
i
```
```	
  Шапка
Короткое описание (Summary)
Проект (Project)
Компонент приложения (Component)
Номер версии (Version)
Серьезность (Severity)
Приоритет (Priority)
Статус (Status)
Автор (Author)
Назначен на (Assigned To)
  Окружение
Информация об окружении, на котором был найден баг: 
операционная система, сервис пак, 
для WEB тестирования - имя и версия браузера и т.д.
  Описание:
Шаги воспроизведения (Steps to Reproduce)
Фактический Результат (Result)
Ожидаемый результат (Expected Result)
  Дополнения:
Прикрепленный файл (Attachment)
```
ESC ```:wq``` ENTER

### 4. Запушить структуру багрепорта на внешний репозиторий
```
git add bug_report_structure.txt
git commit -m "add file bug_report_structure.txt"
git push --set-upstream origin Bag_Reports
```
### 5. Вмержить ветку Bag Reports в Main
```
git checkout main
git merge Bag_Reports
```
### 6. Запушить main на внешний репозиторий.
```
git push
```
### 7. В ветке CheckLists набросать структуру чек листа.
```
git checkout CheckLists
touch check_list_structure.txt
vim check_list_structure.txt
i
```
```
Проверка (что проверяем)
Окружение (Информация об окружении)
Результат (Passed, Failed, Blocked, Skipped, Not run)
Комментарии
```
### 8. Запушить структуру на внешний репозиторий
```
git add check_list_structure.txt
git commit -m "add file check_list_structure.txt"
git push --set-upstream origin CheckLists
```
### 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

### 10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main
git pull
```
