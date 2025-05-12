# **Functional Requirements Document (FRD)**  
**Project Name:** Brushed by betty Makeup Art Training System  
**Prepared By:** [Juhar Yimer]  
**Date:** [05-12-2025]  
**Version:** 1.0  

---

## **1. Introduction**  
### **1.1 Purpose**  
This document outlines the functional requirements for the **Brushed By Betty Makeup Art Training System**, which will facilitate online makeup training through studio bookings, video courses, live classes, and assignments, leading to certification upon completion.  

### **1.2 Scope**  
The system will consist of:  
- **Mobile App (End Users):** Course registration, payment, learning, assignments, and certification.  
- **Web Admin Panel:** Course management, instructor management, user management, and analytics.  
- **Backend System:** Supports both mobile and web interfaces with APIs.  

### **1.3 Target Users**  
- **Students/Trainees** – Register, pay, attend courses, submit assignments, and get certified.  
- **Instructors** – Teach courses, manage sessions, and evaluate assignments.  
- **Administrators** – Manage courses, instructors, payments, and certifications.  

---

## **2. Functional Requirements**  

### **2.1 User Registration & Authentication**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR1.1 | User Registration | Users (students/instructors) can register via email/mobile. |  
| FR1.2 | Login/Logout | Secure login using credentials. |  
| FR1.3 | Role-Based Access | Different roles (Student, Instructor, Admin). |  

### **2.2 Course Management (Admin Web Panel)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR2.1 | Add/Edit/Delete Course | Admin can create courses with details (title, description, category, price). |  
| FR2.2 | Course Categories | Courses can be categorized (e.g., Basic, Advanced, Bridal). |  
| FR2.3 | Assign Instructors | Admin assigns instructors to courses. |  
| FR2.4 | Course Types | Define course types (Video, Live Class, Studio Booking). |  

### **2.3 Instructor Management (Admin Web Panel)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR3.1 | Add/Edit/Delete Instructor | Admin can manage instructor profiles. |  
| FR3.2 | Instructor Selection | Students can choose instructors during registration. |  

### **2.4 Payment & Enrollment (Mobile App)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR4.1 | Course Payment | Users must pay before accessing courses (Stripe/PayPal integration). |  
| FR4.2 | Enrollment Confirmation | Users receive confirmation upon successful payment. |  

### **2.5 Learning Management (Mobile App)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR5.1 | Access Course Content | Students can view videos, attend live classes, or book studio sessions. |  
| FR5.2 | Assignments Submission | Students submit assignments via the app. |  
| FR5.3 | Progress Tracking | Users see course progress and completion status. |  

### **2.6 Certification (Mobile & Admin Panel)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR6.1 | Automatic Certification | System issues certificates upon course completion. |  
| FR6.2 | Certificate Download | Users can download certificates from the app. |  

### **2.7 Admin Dashboard (Web Panel)**  
| **ID** | **Requirement** | **Description** |  
|--------|----------------|----------------|  
| FR7.1 | Analytics Dashboard | Admin views enrollments, revenue, and course performance. |  
| FR7.2 | User Management | Admin can manage (ban, edit) users. |  
| FR7.3 | Certification Approval | Admin verifies and approves certifications. |  

---

## **3. Non-Functional Requirements**  
- **Performance:** System should handle 1000+ concurrent users.  
- **Security:** Secure payment processing, data encryption.  
- **Platforms:** Mobile (Android/iOS), Web (Admin Panel).  
- **Scalability:** Ability to add more courses and users.  

---

## **4. Assumptions & Constraints**  
- Payment gateway integration (Stripe/PayPal) is required.  
- Students must complete assignments to get certified.  
- Instructors must be approved by the admin.  

---

## **5. Future Enhancements**  
- **Chat Support** – For student-instructor communication.  
- **Multi-language Support** – Expand to non-English users.  
- **Gamification** – Badges and rewards for course completion.  

---
