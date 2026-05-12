# 🚀 Salesforce Summer Program – Day 3  
# 📘 Data Modeling in Salesforce

---

# 📌 Difference Between App, Object, Record, and Field

| Component | Meaning | Simple Understanding | Example |
|---|---|---|---|
| App | Complete system of related features | Full application | College Management App |
| Object | Table that stores similar data | Like a database table | Student Object |
| Record | Single entry in an object | One row in a table | One student details |
| Field | Single attribute inside record | Column in table | Student Name |

👉 In simple terms:  
App → System  
Object → Table  
Record → Row  
Field → Column  

---

# 📌 Standard vs Custom Objects

## 🔹 Standard Objects
These are pre-built by Salesforce and used in most business systems.

### Examples:
- Account (Companies/Customers)
- Contact (People)
- Lead (Potential customers)
- Opportunity (Deals)

👉 Used mainly for CRM (Customer Relationship Management)

---

## 🔹 Custom Objects
These are created by developers/admins based on business needs.

### Examples in College System:
- Student
- Faculty
- Course
- Department

👉 Used when standard objects are not enough for business logic.

---

# 📌 College Management System Data Model

## 🏫 App Name
College Management App

---

# 📌 Objects Used

- Student
- Faculty
- Course
- Department

👉 These objects represent real-world entities in a college system.

---

# 📌 Relationships Between Objects

| Parent Object | Child Object | Type |
|---|---|---|
| Department | Faculty | Lookup |
| Department | Course | Lookup |
| Course | Student | Lookup |
| Faculty | Course | Lookup |

---

# 📌 Relationship Explanation

## 🏢 Department → Faculty
- One department can have multiple faculty members  
- Example: CSE department → 10 professors  

👉 Why?  
Because faculty belongs to a department but can exist independently.

---

## 🏢 Department → Course
- One department offers multiple courses  
- Example: CSE → Java, DBMS, AI  

👉 Why?  
Courses are grouped under departments for organization.

---

## 📘 Course → Student
- One course can have many students  
- Example: Java course → 120 students  

👉 Why?  
Students enroll in multiple courses.

---

## 👨‍🏫 Faculty → Course
- One faculty can teach multiple courses  
- Example: Professor → Java + DBMS  

👉 Why?  
Teachers are flexible across subjects.

---

# 📌 College Management System Diagram

```text
Department
   │
   ├── Faculty
   │
   └── Course
         │
         └── Student
```

👉 This shows how data flows and connects in a structured system.

---

# 📌 Formula Fields (Business Automation)

## 1️⃣ Full Name
```text
First Name + Last Name
```
## 2️⃣ Remaining Seats
```text
Total Seats - Enrolled Students
```
## 3️⃣ Percentage
```text
(Obtained Marks / Total Marks) * 100

```

# 📌 Validation Rules (Data Protection)

## 1️⃣ Email Cannot Be Empty
👉 Ensures every student has valid contact information  
✔ Prevents incomplete records

---

## 2️⃣ Student Age Cannot Be Negative
👉 Age must always be logical  
✔ Prevents invalid data entry like -5 years

---

## 3️⃣ Course Seats Cannot Exceed Limit
👉 Enrolled students must not exceed capacity  
✔ Prevents over-admission issues

---

# 📌 Why Structured Enterprise Data Matters

In real companies, data is very large and complex.

Without structure:
- Data becomes messy
- Duplicate entries increase
- Reports become wrong
- Automation fails

With structure (Salesforce model):
- Data is organized in objects
- Relationships connect data properly
- Validation rules ensure correctness
- Formula fields automate calculations

👉 Result: Clean, scalable, reliable system

---

# ✅ Final Summary

Salesforce Data Modeling is about:
- Structuring data properly
- Connecting objects using relationships
- Automating calculations using formulas
- Protecting data using validation rules

👉 This is the foundation of all enterprise Salesforce applications.
```
