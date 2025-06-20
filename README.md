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

1.3 Review a Book (Triggered from 1.1 or 1.2)
  * After selecting a book, enter a rating (1–5)
  * Add an optional review comment

1.4 Back to Main Menu (Triggered from 1.1 or 1.2)
  * Return to the main menu interface

## 🔹 Python and SQL Code Used in Mode 1
Mode 1<br>
![image](https://github.com/user-attachments/assets/91b07dbc-8938-4f89-a879-8cd95a02e509)

1.1 Search by Book Title<br>
![image](https://github.com/user-attachments/assets/abe77575-19ec-4014-91fa-07107bebebdb)

1.2 Search by Author<br>
![image](https://github.com/user-attachments/assets/9b63d534-988c-4a95-ba78-603f3c57b0da)

1.3 Review a Book (Triggered from 1.1 or 1.2)<br>
![image](https://github.com/user-attachments/assets/42728d95-5a4c-41cf-bea2-22c69983033e)

## 🖼️ Example Output
Mode 1<br>
![12 reviewmode](https://github.com/user-attachments/assets/675082c1-fc8b-4c72-9b0b-9823be9a6ed0)

1.1 Search by Book Title<br>
![12 reviewmode](https://github.com/user-attachments/assets/9fbf94ca-733b-4d13-88ff-c842d167e0c5)
![14 หลัง search หนังสือ](https://github.com/user-attachments/assets/035f9260-0bd1-4367-975c-8d18be092ad1)


1.2 Search by Author<br>
![18 search by auther](https://github.com/user-attachments/assets/09ba611d-a7ff-410b-8291-2da597b75b15)
![19 search by authors 1](https://github.com/user-attachments/assets/060247ba-e310-4d13-9a8a-49042334b612)
![20 result search by author](https://github.com/user-attachments/assets/c4e10c90-7fd9-4608-8d6f-7fa34af4b555)



1.3 Review a Book (Triggered from 1.1 or 1.2)<br>
![15 REVIEW SCORE](https://github.com/user-attachments/assets/88b567f0-7d4e-4eb1-bbd2-c16e52de2723)
![16 comment](https://github.com/user-attachments/assets/9ab8eb74-c1a6-4a89-af66-023dff3752f3)



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
