# HW git_branches
> 1. На локальном репозитории сделать ветки для:
> - Postman
> - Jmeter
> - CheckLists
> - Bug Reports
> - SQL
> - Charles
> - Mobile testing


Создаем репозиторий внешний git_branches.

Клонируем: 

`git clone https://github.com/setter-getter/git_branches.git`

`cd git_branches`	

Создаем ветки:
```
git branch Postman
git branch Jmeter
git branch CheckLists
git branch BugReports
git branch SQL
git branch Charles
git branch MobileTesting
```
***
> 2. Запушить все ветки на внешний репозиторий

`git push -u origin Postman Jmeter CheckLists BugReports SQL Charles MobileTesting`
***
> 3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта

`git checkout BagReports`
```
vim bug_report.txt
 i

*******************************************************************************************************
* № * Summary * Description * Steps to reproduce * Environment * Reproducibility * Severity * Priority*
*******************************************************************************************************
*   *         *		    *                    *             *                 *          *         *
*   *         *             *                    *             *                 *          *         *
*   *         *             *                    *             *                 *          *         *
*******************************************************************************************************

Esc
:wq 
```
***
> 4. Запушить структуру багрепорта на внешний репозиторий
```
git add bug_report.txt
git commit -m "bug_report strgitucture"
git push
```
***
> 5. Вмержить ветку Bag Reports в Main
```
git checkout main
git merge BugReports
```
***
> 6. Запушить main на внешний репозиторий.

`git push`
***
> 7. В ветке CheckLists набросать структуру чек листа.

`git checkout CheckLists`
```
vim CheckList.txt
i

*****************************************************************
*   *                                   *                       *
* № *		Procedure		*	 Result		*
*   *                                   *                       *
*****************************************************************
* 1 * Registration on the site		* 	 Passed		*
*****************************************************************
* 2 * Site authorization		*	 Passed 	*
*****************************************************************
* 3 * Send email to mailing page	*	 No run		*
*****************************************************************

Esc
:wq 
```
***
> 8. Запушить структуру на внешний репозиторий
```
git add CheckList.txt
git commit -m "Checklist structure"
git push
```
***
> 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
```
На внешнем репозитории выбираем "Pull Requests"
Далее "Compare & pull request"
Выбираем, откуда и куда нужно вмержить информацию
Далее "Create pull request" -> "Merge pull request" -> "Confirm merge"
```
***
> 10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main
git pull
``` 
***
