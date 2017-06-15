Item-Catalog--
An application that provides a list of items within a variety of categories as well as provide a user registration and authentication system. Registered users will have the ability to post, edit and delete their own items.

##Project Description

An item catalog application written in Flask and sqlite3. The application provides lists of items grouped into various categories, and provides user authentication with google account and facebook account and user registeration system.

--Homepage of the application shows all the cuurent categories and selecting particular category shows you all the available items for that  category.
--The application also provides JSON API for any catalog, or any item.
--Any user can see all the items and item details.
--Only authenticated users can make any changes to the items and item details such as edit, delete and update.

## Run the virtual machine!

Using the terminal, change directory to oauth (**cd item-catalog**), then type **vagrant up** to launch your virtual machine.


## Running the Restaurant Menu App

Once it is up and running, type **vagrant ssh**. This will log your terminal into the virtual machine, and you'll get a Linux shell prompt. When you want to log out, type **exit** at the shell prompt.  To turn the virtual machine off (without deleting anything), type **vagrant halt**. If you do this, you'll need to run **vagrant up** again before you can log into it.


Now that you have Vagrant up and running type **vagrant ssh** to log into your VM.  change to the /vagrant directory by typing **cd /vagrant**. This will take you to the shared folder between your virtual machine and host machine.

Type **ls** to ensure that you are inside the directory that contains project.py, database_setup.py, and two directories named 'templates' and 'static'

Now type **python database_setup.py** to initialize the database.

Type **python lotsofmenus.py** to populate the database with restaurants and menu items. (Optional)

Type **python project.py** to run the Flask web server. In your browser visit **http://localhost:5000** to view the restaurant menu app.  You should be able to view, add, edit, and delete menu items and restaurants.
