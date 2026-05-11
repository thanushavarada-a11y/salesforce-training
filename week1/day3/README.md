# 1. Difference Between App, Object, Record, and Field

| Term | Description |
|---|---|
| App | A collection of related objects, tabs, and tools designed for a specific business purpose. |
| Object | A database table used to store specific types of business data. |
| Record | A single entry or row inside an object. |
| Field | A column inside an object used to store a specific piece of information. |

### Example

- App → College Management System
- Object → Student
- Record → Details of one student
- Field → Student Name, Roll Number, Phone Number

# 2. Standard vs Custom Objects

| Standard Objects | Custom Objects |
|---|---|
| Pre-built by Salesforce | Created by users/developers |
| Used for common CRM processes | Used for specific business needs |
| Examples: Account, Contact, Opportunity | Examples: Student, Faculty, Course |

# 3. College Data Model

## Objects

- Student
- Faculty
- Course
- Department
- Attendance
- Exams

## Relationships

- One Department can have many Students
- One Department can have many Faculty members
- One Faculty member can teach many Courses
- One Student can enroll in many Courses
- One Student can have many Attendance records
- One Student can have many Exam records

# 4. Formula Fields

## 1. Attendance Percentage

### Formula Field
Automatically calculates student attendance percentage.

### Why?
This reduces manual calculations and helps students and faculty quickly view attendance status.

## 2. Remaining Seats

### Formula Field
Calculates remaining seats in a course.

### Why?
It automatically updates available seats whenever new students enroll.

## 3. Total Marks Percentage

### Formula Field
Calculates percentage based on obtained marks and total marks.

### Why?
It saves time and avoids human calculation errors.

# 5. Validation Rules

## 1. Student Age Cannot Be Negative

### Validation Rule
Prevents users from entering invalid age values.

### Why?
Negative age values are logically incorrect and create bad data.

---

## 2. Email Cannot Be Empty

### Validation Rule
Ensures every student record contains an email address.

### Why?
Email is important for communication and notifications.

## 3. Course Seats Cannot Exceed Limit

### Validation Rule
Prevents course capacity from exceeding the maximum allowed seats.

### Why?
It maintains accurate course enrollment data.

# 6. Reflection - Why Structured Enterprise Data Matters

Structured enterprise data helps companies organize information properly instead of storing random and inconsistent data in spreadsheets. It improves data accuracy, reporting, automation, security, and decision-making. Relationships between objects help businesses connect data efficiently and reduce duplication. Salesforce uses structured data to help organizations manage large-scale operations smoothly and efficiently.
