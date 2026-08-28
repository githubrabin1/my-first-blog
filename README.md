# 📝 Django Blog

A simple and responsive blog web application built with **Python and Django**.

This is my first Django project, created while learning the fundamentals of Django and web development. The project allows users to view blog posts, create new posts, edit existing posts, and manage posts through Django's admin interface.

## 🌐 Live Demo

🚀 **[Visit My Live Blog](https://rabinl.pythonanywhere.com/)**

---

## 🚀 Features

* 📖 View all published blog posts
* 🔍 View individual blog posts
* ➕ Create new blog posts
* ✏️ Edit existing blog posts
* 👤 Assign posts to an author
* 📅 Automatically set the published date
* 🔐 CSRF protection for forms
* 🛠️ Django Admin interface for managing posts
* 🎨 Custom CSS styling
* 📱 Responsive layout using Bootstrap
* ⬇️ Display the latest published posts first
* 🗄️ SQLite database for storing blog data

---

## 🛠️ Technologies Used

| Technology      | Purpose                   |
| --------------- | ------------------------- |
| **Python**      | Programming language      |
| **Django**      | Web framework             |
| **HTML**        | Web page structure        |
| **CSS**         | Styling                   |
| **Bootstrap 5** | Responsive user interface |
| **SQLite**      | Database                  |
| **Git**         | Version control           |
| **GitHub**      | Source code hosting       |

---

## 📂 Project Structure

```text
Django/
│
├── blog/
│   ├── migrations/
│   │
│   ├── static/
│   │   └── css/
│   │       └── blog.css
│   │
│   ├── templates/
│   │   └── blog/
│   │       ├── icons/
│   │       ├── base.html
│   │       ├── post_detail.html
│   │       ├── post_edit.html
│   │       └── post_list.html
│   │
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
│
├── mysite/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── myvenv/
├── .gitignore
├── db.sqlite3
├── manage.py
└── requirements.txt
```

---

## ⚙️ Installation & Setup

Follow the steps below to run this project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/githubrabin1/my-first-blog.git
cd my-first-blog
```

### 2. Create a Virtual Environment

For **macOS/Linux**:

```bash
python3 -m venv myvenv
```

Activate the virtual environment:

```bash
source myvenv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply Database Migrations

```bash
python3 manage.py migrate
```

### 5. Create a Superuser

```bash
python3 manage.py createsuperuser
```

Follow the instructions in the terminal to create your admin account.

### 6. Run the Development Server

```bash
python3 manage.py runserver
```

Open the website in your browser:

```text
http://127.0.0.1:8000/
```

### Django Admin

The Django admin panel is available at:

```text
http://127.0.0.1:8000/admin/
```

---

## 📚 What I Learned

This project helped me understand the basic structure and workflow of a Django application.

### Django Fundamentals

* Creating a Django project and application
* Understanding Django project structure
* URL routing
* Function-based views
* Django templates
* Template inheritance
* Static files
* Django models
* Django ORM
* QuerySets
* Database migrations
* Django Admin
* Django Forms
* Creating forms using `ModelForm`
* Handling `GET` and `POST` requests
* Form validation
* Saving form data
* Using `commit=False`
* CSRF protection

### Database

* Working with SQLite
* Creating and modifying Django models
* Creating database migrations
* Applying migrations
* Retrieving objects using QuerySets
* Filtering QuerySets
* Ordering QuerySets

---

## 📝 Blog Post Ordering

Blog posts are displayed with the **newest published post first** using Django's `order_by()` method:

```python
.order_by('-published_date')
```

The `-` sign means **descending order**, so posts with the most recent `published_date` appear at the top.

---

## 🎯 Future Improvements

As I continue learning Django, I plan to improve this project by adding:

* 👤 User registration and login
* 💬 Comments
* 🔍 Search functionality
* 🏷️ Categories and tags
* 📄 Pagination
* 🖼️ Image uploads
* 👨‍💻 User profiles
* ❤️ Like functionality
* 🔌 Django REST Framework API
* 🎨 Improved UI/UX
* 🧪 More automated tests

---

## 🙏 Acknowledgement

This project was created while learning from the **[Django Girls Tutorial](https://tutorial.djangogirls.org/)**.

It is my first Django project and helped me build a strong foundation in **Python web development and Django**.

---

## 👨‍💻 Author

**Rabin Ghimire**

* GitHub: **[githubrabin1](https://github.com/githubrabin1)**
* Live Blog: **[rabinl.pythonanywhere.com](https://rabinl.pythonanywhere.com/)**

---

⭐ **If you found this project useful, feel free to give it a star!**

