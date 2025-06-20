# Amazon_Book_Review_and_Analysis
This project is a Python-SQL integrated application that allows users to explore, review, and analyze books available on Amazon. The system connects a MySQL database with a Python interface using mysql-connector, allowing dynamic interaction with book review data via SQL queries executed within Python.

## 🔧 Project Features
## 🔍 Book Recommendation & Review
* Search books by title or author
* Submit your rating (1–5) and review comments
* Register automatically if you're a new user

## 📊 Analytics & Reports
Get insights based on SQL queries directly from the database:
* Distribution of reviewer age and books by publish year
* Average ratings by book category
* Probability of authors receiving a review score > 4

## 🧩 Technical Highlights
* Python notebook (.ipynb) connected to MySQL via mysql-connector-python
* SQL queries embedded within Python functions (getDF() and editDF())
* Console-based interactive interface
* Entity-Relationship Diagram (ERD) with three main tables:
  * book_detail: Book metadata
  * book_rating: User reviews and scores
  * customer: Reviewer demographics

## 🗂️ Files Included
* Missing Data_python.ipynb: Jupyter Notebook containing all Python and SQL logic
* Missing Data_database.png: Database schema/ERD
* Missing Data_database.sql: SQL script for setting up the database and initial tables
* คู่มือการใช้งาน ระบบข้อมูลการรีวิวหนังสือเว็บ Amazon.pdf: Thai user manual explaining the system interface

🚀 How to Run
1. Install the database using Missing Data_database.sql in your MySQL server
2. Open and run Missing Data_python.ipynb in Jupyter Notebook
3. Update your database credentials inside the functions getDF() and editDF()
4. Run all cells
5. Enter your User ID or register as a new user
6. Navigate the menu:
  * Mode 1: Review books
  * Mode 2: Analytics reports
  * Mode 3: Exit

## 🧭 Menu Overview
✅ Mode 1: Review Books
In this mode, users can perform the following actions:

1.1 Search by Book Title
  * Input partial or full book title
  * Get list of matching books

1.2 Search by Author
  * Input partial or full author name
  * Get list of matching books by the author

1.3 Review a Book
  * After selecting a book, enter a rating (1–5)
  * Add an optional review comment

1.4 Back to Main Menu
  * Return to the main menu interface

## 🔹 SQL Code Used in Mode 1
(Insert SQL code screenshot or markdown block here — e.g., for searching and inserting review)

## 🖼️ Example Output
(Insert screenshots of user interface or sample output here)

## 📈 Mode 2: Analytics Reports
This mode provides access to 3 analytical views:

2.1 Distribution of Reviewer Age & Book Publish Year
  * Histogram or count of reviewer ages
  * Histogram or count of books grouped by publication year

2.2 Average Rating by Book Category
  * Aggregated average rating across genres/categories

2.3 Probability of Authors Receiving Ratings > 4
  * Calculates how often each author's books receive a rating higher than 4

2.4 Back to Main Menu
  * Return to the main menu interface

## 🔹 SQL Code Used in Mode 2
(Insert SQL code screenshots or markdown block here — separate by 2.1, 2.2, 2.3)

## 🖼️ Example Output
(Insert plots or tables of each analytic report here)

## ❌ Mode 3: Exit
Cleanly exits the application.

## 🛠️ Tech Stack
* Python 3
* MySQL
* Jupyter Notebook
* SQL Connector: mysql-connector-python
