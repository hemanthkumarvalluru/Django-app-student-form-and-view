# Django-app-student-form-and-view
Form for student details entry and displaying student details table

Django Web app
==============
--Developed a form for adding student with name, age, gender details.
--On submission stores the results into database (in this project we use SQLite database)
--Another html page to view student records as a Table.


Steps to describe project briefly
---------------------------------
1. Select folder-- create virtual environment, activate, install django
	from command prompt commands
	----------------------------
	mkdir student
	virtualenv venv
	venv\Scripts\activate
	pip install Django
	python -m django --version
2. Start project by command django-admin startproject student
3. Change directory cd student and load project folder in sublime editor (you can choose any other).
4. Runserver- python manage.py runserver
5. Start app-- python manage.py startapp app1
6. Add app1 in settings
7. download and install DB Browser for SQLite software
8. Add path in urls, I have created 2 responses, one is for form filling another is for displaying student details.
9. Write defenition in views for urls form and index, to connect database write student class in models.
10. Makemigrations it will update database according to changes made in models -- 
	commands are
	============
	python manage.py makemigrations--which is responsible for creating new migrations based on the changes you have made to your 
	python manage.py migrate-- which is responsible for applying and unapplying migrations.
		


11. If we want to interact from cmd prompt use python manage.py shell
	commands
	========

	pip install ipython--- installing interactive python 
	python manage.py shell-- 

12. In form.html write form code with method type POST it will Appends form-data inside the body of the HTTP request (data is not shown is in URL). Here in this project we take student name, age, gender as input type as text. It will store in sqlite 		database by writing request.method=POST code as shown in project. For complete code refer views.py file in app1 folder and index.html in templates folder.
13. In index.html write code to retrieve data from database through index defenition in view.py file and show student details as a 		table. Refer index.html file and views.py file.
14. We can export data to CSV, JSON formats directly from DB Browser for SQLite software.

We can include css to add style to form and student details. I just done a samlpe simple app with Django, db browser sqlite database, simple html and python commands.

We can Further add colors to web page background, up to now I done simple app.

