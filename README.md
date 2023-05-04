## Git_branch
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

`git branch postman`

`git branch jmeter`

`git branch checklists`

`git branch bug_reports`

`git branch SQL`

`git branch charles`

`git branch mobile testing`

2. Запушить все ветки на внешний репозиторий

`git push --all`

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта 

`git checkout bug_reports`

`vim bug.report.txt`

1. Title

2. Bug severity and priority
- Bug severity: Blocker/Critical/Major/Minor/Trivial
- Bug priority: High/Medium/Minor

3. Description

4. Environment:
- Device manufacturer and model number
- OS version
- Application version
- Network connectivity
- Screen orientation
- Browser

5. Steps to reproduce

6. Expected result

7. Actual result

8. Attachments:
- Screenshot
- Video
- Log-fil

4. Запушить структуру багрепорта на внешний репозиторий 

`git add bug.report.txt`

`git commit -am "Bug_report"`

`git push -u origin bug.report.txt`


5. Вмержить ветку Bag Reports в Main 

`git checkout main`

`git merge bug_reports`

6. Запушить main на внешний репозиторий 

`git commit -am "branch"`

`git push -u origin main`

7. В ветке CheckLists набросать структуру чек листа ===

`vim checklist.txt`

 1. ID
 
 2. Title
 
 3. Inputs
 
 4. Expected result
 
 5. Actual result
 
 6. Status
 
 7. Bug

8. Запушить структуру на внешний репозиторий 

`git add cheklist.txt`

`git commit -m "new checklist"`

`git push -u origin checklist`

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main 

10. Синхронизировать Внешнюю и Локальную ветки Main 

`git fetch`

`git pull`
