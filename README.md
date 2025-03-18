# Garbage Level Monitoring System in Django with Source Code

The **Garbage Level Monitoring System Project created based on Python, Django, and SQLITE3 Database**.

When the garbage reaches its maximum capacity, a notification will be sent to the corporation’s office, and staff will be able to take action to empty the bin.

This system will aid in the improved cleaning of the city.

A **Garbage Level Monitoring System in Django** is an easy project for beginners to learn how to build a web-based python Django project.

We will provide you with the complete source code and database for the **Python** project so that you can easily install it on your machine and learn how to program in Python Django.

> [!NOTE]
> To start creating a **Garbage Level Monitoring System Project in Python Django**, makes sure that you have PyCharm Professional IDE Installed in your computer.

## Admin Features of Garbage Level Monitoring System Project in Django

### Login Page

The page where the system administrator enters their system credentials in order to gain access to the system’s administrative side.

### New Dustbin Page

This is the page where an administrator can add a new dustbin.

### Dustbin List 

The page with a list of dustbin that can be navigated to change or delete a dustbin.

### New Readings Page

The page on which an administrator can add new readings.

### Readings List

The page on which the list of readings can be viewed, modified, or readings.

### New User Page

The page where a new admin credentials are created by an admin.

### Users list

This is the page that lists and manages the added users.

## How to Create a Project Garbage Level Monitoring System in Django?

Here are the steps on how to create a **Django Garbage Level Monitoring System with Source Code**.

1. **Open file.**

Open **"pycharm professional"** after that click **"file"** and click **"new project"**.

2. **Choose Django**.

After click **"new project"**, choose **"Django"** and click.

3. **Select file location**.

Then, select a file location wherever you want.

4. **Create application name**.

After that, name your application.

5. **Click create**.

Finish creating project by clicking "create" button.

6. **Start Coding.**

Finally, we will now start adding functionality to our Django Framework by adding some functional codes.

## Functionality and Codes

* **Create template for the homepage**

In this section, we will learn on how create a templates for the homepage. 

To start with, add the following code in your base.html under the folder of /templates/.

```
{% load static %}
<html>
    <head>
        <meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1">
        <title>
            Garbage Level Monitoring System
        </title>
        <link rel='stylesheet' href='{% static "css/bootstrap.min.css" %}'>
        <link rel='stylesheet' href='{% static "css/base.css" %}'>
    </head>
    <body>
         <!-- data-spy="scroll" data-target=".navbar" data-offset="10" -->
        <nav class="navbar navbar-default navbar-fixed-top" style="background-color: skyblue;">
	        <div class="container">
		        <div class="navbar-header">
    		        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
    		            <span class="sr-only">Toggle navigation</span>
    		            <span class="icon-bar"></span>
    		            <span class="icon-bar"></span>
    		            <span class="icon-bar"></span>
    		        </button>
    		        <a class="navbar-brand" href="/">
    		          	GLMS
    		        </a>
		        </div><!-- ./navbar-header -->
		        <div id="navbar" class="navbar-collapse collapse">
			        <ul class="nav navbar-nav" id="navbar-links">
			          	<li>
                            <a href="/dashboard"><span class="glyphicon glyphicon-dashboard"></span> DASHBOARD </a>
                        </li>
			        </ul>
                    <ul class="nav navbar-nav navbar-right">
                        <!-- <li><a href="/accounts/register"><span class="glyphicon glyphicon-user"></span> Sign Up</a></li> -->
                        {% comment %} If user is logged in, show his/her username {% endcomment %}
                        {% if request.user.username %}
                            <li><a href="#">Hello, {{ request.user.username }}</a></li>
                            <li>
                                <a href="/logout">
                                  <span class="glyphicon glyphicon-log-out"></span> Logout
                                </a>
                            </li>
                        {% else %}
                            <li><a href="/login"><span class="glyphicon glyphicon-log-in"></span> Login</a></li>
                        {% endif %}
                    </ul>
		        </div><!--/.nav-collapse -->
	        </div><!-- ./container-->
	    </nav>
        <div class="add-margin-top"></div>
        {% block content %}

        {% endblock %}
    </body>
    <script src="{% static 'js/jquery.min.js' %}"></script>
    <script src="{% static 'js/bootstrap.min.js' %}"></script>
    <script src="{% static 'js/base.js' %}"></script>
    <script src="{% static 'js/chart.min.js' %}"></script>
    <script src="{% static 'js/utils.js' %}"></script>
</html>
```

### 📌 Here's the full documentation for the [Garbage Level Monitoring System in Django](https://itsourcecode.com/free-projects/python-projects/garbage-level-monitoring-system-project-in-django-with-source-code/)




