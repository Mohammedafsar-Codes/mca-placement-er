# MCA Placement Management System - ER Model

## 1. Entities and Attributes

### Student (Entity)
- student_id (Primary Key)
- name
- email
- phone
- cgpa
- department

### Company (Entity)
- company_id (Primary Key)
- company_name
- location
- hr_contact

### Placement_Drive (Entity)
- drive_id (Primary Key)
- company_id (Foreign Key)
- job_role
- salary_package
- min_cgpa

### Application (Entity)
- application_id (Primary Key)
- student_id (Foreign Key)
- drive_id (Foreign Key)
- status (Applied / Selected / Rejected)

---

## 2. Relationships (Cardinality)
- **Company to Placement_Drive**: One-to-Many (1 : N)
- **Student to Application**: One-to-Many (1 : N)
- **Placement_Drive to Application**: One-to-Many (1 : N)
