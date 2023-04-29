# A Simple Forum Application using Flask, PyMongo, and Pagination

## Introduction

In this report, we present a simple forum application that allows users to interact with data from a MongoDB database in an intuitive and effortless manner. The application is built using Python, Flask, and PyMongo, and deployed on the NYU CS Department's web server and MongoDB server. The application meets the given requirements and features a comment function, search functionality, and pagination.

### 1. Technologies Used
The following technologies were used to build the application:

Python: The programming language used to develop the application.
Flask: A lightweight web framework for Python that allows the creation of web applications quickly and easily.
PyMongo: A Python library that provides tools for working with MongoDB databases.
Pagination: A utility from Flask that allows easy navigation through large collections of data.

### 2. Application Features
The application consists of the following features:

Post Creation: Users can create new posts.
Comment Function: Users can comment on specific posts. The commenter's name is also displayed.
Search Function: Users can search for posts based on the author's name or the content of the post.
CRUD Operations: The application supports Create, Read, Update, and Delete (CRUD) operations on documents in the database.
Consistent Design: The web pages have a consistent design, and the code is well-organized and modular.

### 3. Comment Function

The comment function was implemented using the following route in the `app.py` file:

```python
@app.route('/add_comment/<mongoid>', methods=['GET', 'POST'])
```
This route handles both GET and POST requests, displaying a form for users to add a comment to an existing post and updating the database with the new comment.

### 4. Search Function
The search function was implemented by modifying the read.html template to include a search form and using Flask's Pagination utility to navigate through the search results.

### 5. Pagination
Pagination was implemented using the Pagination utility from Flask. This allowed for easy navigation through large collections of data in the application.

### 6. Conclusion
In conclusion, we have successfully built a simple forum application that meets the given requirements and allows users to interact with data in an intuitive and effortless manner. The application features a comment function, search functionality, and pagination, and demonstrates the power and flexibility of Flask and PyMongo in building web applications.