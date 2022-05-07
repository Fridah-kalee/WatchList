 

filter_by is used for simple queries on the column names using regular kwargs, like

db.users.filter_by(name='Joe')

The same can be accomplished with filter, not using kwargs, but instead using the '==' equality operator, which has been overloaded on the db.users.name object:

db.users.filter(db.users.name=='Joe')

You can also write more powerful queries using filter, such as expressions like:

db.users.filter(or_(db.users.name=='Ryan', db.users.country=='England'))



asgiref==3.2.3
autopep8==1.5.2
certifi==2020.4.5.1
click==7.1.2
dominate==2.5.1
Flask==1.1.2
Flask-Bootstrap==3.3.7.1
Flask-Script==2.0.6
Flask-WTF==0.14.3
gunicorn==20.0.4
itsdangerous==1.1.0
Jinja2==2.11.2
MarkupSafe==1.1.1
pycodestyle==2.6.0
pyperclip==1.8.0
pytz==2019.3
sqlparse==0.3.0
visitor==0.1.3
Werkzeug==1.0.1
WTForms==2.3.1