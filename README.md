# GitHub_HW_2
Продолжаем изучать GitHub: создание и слияние веток
<hr>

**1. На локальном репозитории сделать ветки для:**
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing
```
$ git branch postman 
$ git branch jmeter и т.д.
```
**2. Запушить все ветки на внешний репозиторий**
```
$ git push -u origin 'postman' 'jmeter' 'bug_reports' 'charles' 'check_lists' 'mobile_testing' 'sql'
```
**3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта**
```
$ git checkout bug_reports

$ cat > bug_report.txt
ID - 
Severity - 
Priority - 
Status - 
Title - 
Author - 
Environment -
Steps -   
AR - 
ER - 
Attachment -
```
**4. Запушить структуру багрепорта на внешний репозиторий**
```
$ git add .
$ git commit -m "add bug_report.txt"
$ git push
```
**5. Вмержить ветку Bug Reports в Main**
```
$ git checkout main
$ git merge bug_reports
```
**6. Запушить main на внешний репозиторий**
```
$ git push
```
**7. В ветке CheckLists набросать структуру чек листа**
```
$ git checkout check_lists

$ cat > check_list
#
Проверка
Статус
Комментарии
```
**8. Запушить структуру на внешний репозиторий**
```
$ git add .
$ git commit -m 'add check_list'
$ git push
```
**9. На внешнем репозитории сделать Pull Request ветки CheckLists в main**

**10. Синхронизировать Внешнюю и Локальную ветки Main**
```
$ git checkout main
$ git pull
```
