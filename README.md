JSON
	https://github.com/npopova02/JSON

 4. Создать внешний репозиторий c названием JSON.
 зайти в GitHub и создать новый репозиторий-  Repositories-> New->JSON(name)-Public-Add a README file->Create repository
 
 5. Клонировать репозиторий JSON на локальный компьютер.
	$ git clone https://github.com/npopova02/JSON
	
 6. Внутри локального JSON создать файл “new.json”.
	$ cd JSON (зайти в папку JSON на локальном компьютере)
	$ touch new.json (создание файла)

 7. Добавить файл под гит.
	$ git status
	$ git add new.json
	 
 8. Закоммитить файл.
	$ git commit -m "Adding a new empty file"
	
 9. Отправить файл на внешний GitHub репозиторий.
	$ git push 
 
 10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
	vim new.json -редактируем файл
	нажимаем I(Insert)-вносим данные
	{
	"ФИО":"Попова Надежда Анатольевна",
	"Возраст":38,
	"Количество домашних животных":1,
	"ЗП":"$500"
	} 
	Esc- выходим из редактирования
	:wq->Enter - сохраняем изменения
 
 11. Отправить изменения на внешний репозиторий.
	$ git status
	$ git add new.json
	$ git commit -m "Adding personal information"
	$ git push

 12. Создать файл preferences.json
	$ touch preferences.json 
	
 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
	vim preferences.json 
	{
	"Любимый фильм":"Достучаться до небес",
	"Любимый сериал":"нет",
	"Любимая еда":"Борщ",
	"Любимое время года":"лето",
	"Страна которую хотели бы посетить":"Индия"
	}
	
 14. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
	$ cat> skills.json
	добавить данные
	{
	"terminal": "Командная строка (terminal) Linux GitBash",
	"mobile": " Мобильное тестирование. Особенность iOS, Android, гайдлайны",
	"tools": "Dev Tools веб браузеров (Google Chrome, FireFox)",
	"SQL": "Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)",
	"Postman": "Тестирование API через Postman (JS, автотесты API)",
	"Jmeter": "Нагрузочное тестирование"
	} 
	Cntr+C - сохранение 
 
 15. Отправить сразу 2 файла на внешний репозиторий.
	$ git . && git commit -m "Adding preference and skills information" && git push
	
 16. На веб интерфейсе создать файл bug_report.json.
	зайти в репозиторий JSON-> кнопка Add file-> ввести bug_report.json в поле для названия файла 
 
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
	ввести текст коммита в поле для названия коммита-> нажать кнопку Commit new file  
	
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
	открыть файл-> выбрать Edit this file (карандашик)-> добавить баг репорт в формате JSON
	{
  "id" : 1,
  "summary": "No login with valid username/password",
  "severity": "Blocker",
  "priority": "High",
  "status": "Open",
  "precondition": "Valid data: Username- standard_user, password-secret_sauce",
  "steps_to_reproduce": ["Go to www.saucedemo.com", "Enter valid Username/password combination", "Click [LOGIN] button"],   
  "actual_resul": "Login is not sucssesfull. Error message Epic sadface: Username and password do not match any user in this service appears",
  "expected_result": " Login is sucssesfull. The home page of the site appears"
	}

 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
	 ввести текст коммита в поле Commit changes-> нажать кнопку Commit changes  
	 
 20. Синхронизировать внешний и локальный репозиторий JSON 
	$ git pull

