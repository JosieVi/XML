# XML
GIT Homework 1. XML
 1. Создать внешний репозиторий c названием XML.
 Выполняю действия на сайте: New repository -> XML, ставлю галочку "Добавить Readme file", чтобы при клонировании на локальный компьютер не было предупреждения о клонировании пустой папки.

 2. Клонировать репозиторий XML на локальный компьютер.
 $ git clone https://github.com/JosieVi/XML.git

 3. Внутри локального XML создать файл “new.xml”.
 $ cd XML 
 $ touch new.xml

 4. Добавить файл под гит.
 $ git add new.xml
 
 5. Закоммитить файл.
 $ git commit -m "add new.xml to repository XML"

 6. Отправить файл на внешний GitHub репозиторий.
 $ git push

 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 $ nano new.xml
<?xml version="1.0" encoding="utf-8"?>
<site_winnote>
 <article>About me</article>
 <content>Name: Olga</content>
 <content>Age: 36</content>
 <content>Number of pets: 0</content>
 <content>Desired salary: 3000$</content>
</site_winnote>
Ctrl+C
Ctrl+X

 8. Отправить изменения на внешний репозиторий.
 $ git add . 
 $ git commit -m "add completed file new.xml to repository XML"
 $ git push
 
 9. Создать файл preferences.xml
 $ touch preferences.xml

 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, страна, которую хотели бы посетить) в формате XML.
 $ nano preferences.xml
<?xml version="1.0" encoding="utf-8"?>
<site_winnote>
 <article>My preferences</article>
 <content>Favorite movie: Lord of the Rings</content>
 <content>Favorite TV show: Queen's Gambit</content>
 <content>Favorite food: Fruits</content>
 <content>Favorite time of year: Spring</content>
 <content>Desired country: Finland</content>
</site_winnote>
Ctrl+C
Ctrl+X

 11. Создать файл skills.xml добавить информацию о скиллах, которые будут изучены, на курсе в формате XML
 $ cat > skills.xml
<?xml version="1.0" encoding="utf-8"?>
<site_winnote>
 <article>Skills:</article>
 <content>Linux terminal commands</content>
 <content>JavaScript</content>
 <content>Git</content>
 <content>Postman</content>
 <content>DBeaver</content>
</site_winnote>
Ctrl+C
Ctrl+X

 12. Сделать коммит в одну строку.
 $ git add . && git commit -m "add files preferences.json, skills.json to repository XML"

 13. Отправить сразу 2 файла на внешний репозиторий.
 $ git push

 14. На веб интерфейсе создать файл bug_report.xml.
 Repository XML -> Add file -> Create new file -> bug_report.json

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit new file

 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
<?xml version="1.0" encoding="utf-8"?>
<site_winnote>
 <article>Bug #1</article>
 <content>Summary: "Login: Error messages in the login from are displayed in English"</content>
 <content>Environment: "All browsers / devices"</content>
 <content>Severity: "Major"</content>
 <content>Steps for reproduce: 1. Open https://. 2. Follow 'Inloggen' link. 3. Fill required fields with invalid data. 4. Click 'Inloggen' button. 5. Pay attention to error messages</content>
 <content>Actual results: "Error messages in the login form are displayed in English"</content>
 <content>Expected results: "Error messages in the login form are displayed in the chosen language"</content>
/site_winnote>

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Commit changes

 18. Синхронизировать внешний и локальный репозиторий XML
 $ git pull
