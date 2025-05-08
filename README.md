Student Course Management API

This repository contains a REST API built with FastAPI for managing students, courses, and enrollments. It includes a ZIP file (StudentCourseAPI.zip) with all source code and a requirements.txt file for dependencies. The API is powered by SQLAlchemy and supports SQLite (default) or PostgreSQL.

#video


Running the API

To start the API, use:


https://github.com/user-attachments/assets/d12d6e54-3261-4812-a61f-278ca9d28a8b


uvicorn main:app --reload

Access it at http://127.0.0.1:8000 or explore endpoints via http://127.0.0.1:8000/docs.

Features





Student Management:





Register students with name and email (POST /students/).



Retrieve student details, including enrolled courses (GET /students/{id}).



List all students with pagination (GET /students/).



Course Management:





Register courses with title and description (POST /courses/).



Retrieve course details, including enrolled students (GET /courses/{id}).



List all courses with pagination (GET /courses/).



Enrollment:





Enroll students in courses (POST /enroll/).



Bonus Features:





Email validation for student registration using Pydantic and regex.



Pagination for student and course lists using fastapi-pagination.



Unit tests (test_main.py) for core functionality using pytest.

Repository Contents





StudentCourseAPI.zip: Contains:





main.py: FastAPI application with endpoint logic.



utili.py: Database and Pydantic models.



test_main.py: Unit tests.



README.md: Setup and usage instructions.



requirements.txt: Dependencies.



Individual files are also available in the repository.
