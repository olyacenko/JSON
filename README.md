# JSON
 1. Создать внешний репозиторий c названием JSON. - 
 
 зайти в GitHub аккаунт ; 
 
 нажать на кнопку `new repository` ;
 
 ввести Repository name «JSON» ; 
 
 нажать на кнопку `Public` ; 
 
 поставить галочку `Add a README file` ; 
 
 нажать на кнопку `Create repository`
 
 ----

 2. Клонировать репозиторий JSON на локальный компьютер. - `git clone https://github.com/olyacenko/JSON.git`
 
  ----
  
 3. Внутри локального JSON создать файл “new.json”. - `touch new.json`

 ----

 4. Добавить файл под гит. - `git add "new.json"`

 ----

 5. Закоммитить файл. - `git commit -m "add file new.json"`

 ----

 6. Отправить файл на внешний GitHub репозиторий. - `git push`

 ----

 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON. - 
 
 `vim new.json` ; 
 
 `i` - начать редактирование ; 
 
 ввести текст в формате json ; 
 
 клавишa `esc` - выйти из режима редактирования ; 
 
 клавиши `shift+:` - назначить команду ; 
 
 `wq` - записать и закрыть редактор

 ----

 8. Отправить изменения на внешний репозиторий. - `git add "new.json"` => `git commit -m "add data to file"` => `git push`

 ----

 9. Создать файл preferences.json - `touch preferences.json`

 ----

 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON. - 
 
`vim preferences.json` ; 

`i` - начать редактирование ;

ввести текст в формате json ; 

клавишa `esc` - выйти из режима редактирования ; 

клавиши `shift+:` - назначить команду ; 

`wq` - записать и закрыть редактор

 ----

 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON. - 
 
 `vim sklls.json` ; 
 
 `i` - начать редактирование ; 
 
 ввести текст в формате json ; 
 
 клавишa `esc` - выйти из режима редактирования ; 
 
 клавиши `shift+:` - назначить команду ; 
 
 `wq` - записать и закрыть редактор

 ----

 12. Отправить сразу 2 файла на внешний репозиторий. - `git add "preferences.json" "sklls.json"` => `git commit -m "add new files sklls.json and preferences.json"` => `git push` 

 ----

 13. На веб интерфейсе создать файл bug_report.json. - 
 
 Нажать кнопку `Add file` ; 
 
 `Create new file` ; 
 
 ввести имя файла «bug_report.json» 

 ----

 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе. - 
 
 `Commit new file` ввести описание «create new file bug_report.json» ;
 
 нажать на кнопку `Commit directly to the main branch` ; 
 
 нажать на кнопку `Commit new file`

 ----

 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON. - 
 
 нажать на файл «bug_report.json» ;  
 
 нажать `edit this file` ;
 
 ввести текст в формате json 

 ----
 
 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе. -  
 
 `Commit changes` ввести описание «add data to file bug_report.json» ; 
 
 нажать на кнопку `Commit directly to the main branch` ; 
 
 нажать на кнопку `Commit changes`

 ----

 17. Синхронизировать внешний и локальный репозиторий JSON - `git pull`
