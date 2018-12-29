Within this folder is a small application that runs as a food service hub for planning and delegation of duties.
Administrators can add, update and delete records pertaining to events, customers, and services provided.

To run the application:
1. Run the following commands:
	a. On Windows: 'python -m venv c:\path\to\myenv'
	b. On Mac: 'python3 -m virtualenv myvenv'
2. On Windows, go to the scripts directory and type 'activate'
3. On Mac, go to '/bin inside venv and issue the command: 'source activate'
4. Your venv is now activated. You can leave the venv at any time by typing 'deactivate'
5. Navigate to the MaverickFoodServices directory and issue this command: 'pip install -r requirements.txt'

Database creation and management:
1. Upon initial download, the application has no database for customers and services.
2. Navigate to the base folder (where 'manage.py' is located) and issue this command: 'python manage.py makemigrations'
3. Following this, type the following and press enter: 'python manage.py migrate'
4. Remain in the base folder (containing 'manage.py') and issue this command: 'python3 manage.py runserver'
5. Navigate to http://127.0.0.1:8000 in a web browser and the project will be running on a local server at this address.

Creating user and admin accounts:
1. Exit the running server by pressing Command+C on your keyboard.
2. First you must create a superuser that will be used to create all other user accounts.
3. In the base folder, issue this command: 'python manage.py createsuperuser'
4. Enter the preferred username and password for the superuser account.
5. Upon completion, you can issue 'python3 manage.py runserver' again to start the server and this time navigate
	to http://127.0.0.1:8000/admin in your web browser.
6. Log in with the credentials you created. Here you're able to add, update, and delete:
	a. Customer records
	b. Services provided by customers
	c. Products provided by customers
7. These CRUD features are also available on the main website for a more streamlined experience. 
