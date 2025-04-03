# 📸 Instagram Clone Web App

A full-stack Instagram-style web application, that supports core social media functionality including user registration, photo uploads, likes, comments, and follower interactions — all built from scratch using modern web technologies.

## 🧱 Features

- 🔐 **User Authentication**  
  Sign up, log in, and log out securely with session management

- 🖼️ **Post Feed**  
  Displays posts from followed users in reverse chronological order

- 💬 **Comments and Likes**  
  Users can like photos and leave comments on posts

- 📷 **Image Uploads**  
  Upload, store, and view user-submitted photos

- 👤 **Profile Pages**  
  View user details, post count, follower/following lists

- 🔄 **Dynamic Updates**  
  Supports JSON APIs and AJAX updates for seamless UX

## ⚙️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript (vanilla + AJAX)
- **Backend:** Python (Flask)
- **Database:** SQLite
- **Templating:** Jinja2
- **Testing:** Unit tests with `pytest`
- **Deployment:** Locally and on AWS EC2 (via `make deploy`)

## 🏗️ Architecture Overview

- RESTful endpoints with `/`, `/explore/`, and `/users/<username>/` routes
- Clean separation of views, static content, and templates
- Implements the MVC (Model-View-Controller) pattern
- Includes support for JSON API endpoints for asynchronous content rendering

## 📸 Sample Routes

| Route | Description |
|-------|-------------|
| `/` | Home feed (requires login) |
| `/explore/` | Browse all users |
| `/users/<username>/` | View a user's profile and posts |
| `/posts/<postid>/` | View a single post |
| `/accounts/login/`, `/logout/`, `/create/` | Auth routes |
| `/api/v1/` | JSON API endpoints for dynamic interaction |

## 🧪 Development Workflow

```bash
# Set up virtual environment
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Run the development server
flask run

# Run unit tests
pytest
