This is a Flask application that can store the birthdays of anyone who inputs their name and birthdate.

Anatomy of this site:
I use Python in the backend to process GET and POST requests. Each POST registers the user's name and birthdate in a SQLite database. The birthday posted is then rendered at the index.html. Moreover, I use JINJA to loop through the posted birthdays to render each birthday whenever a new one is posted.

What I learned:
I learned how to create a Flask app from scratch and I learned how the client interacts with the server. Moreover, I learned how to use JINJA syntax for the purpose of rendering things in my HTML pages. I also learned how to add items to the render_template() functions by defining variables in the app.py then using JINJA to utilize such variables in the HTML page. I learned how a web app interacts with various languages to create a cohesive application. Moreover I learned how to use SQLite with real-world application.

Conclusion:
This project was invaluable for reinforcing my understanding that web applications operate by having intercessors as though in some sort of conversation with each other in real-time.
