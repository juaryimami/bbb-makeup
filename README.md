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
- Payment gateway integration (Stripe/PayPal/Telebirr) is required.  
- Students must complete assignments to get certified.  
- Instructors must be approved by the admin.  

---

## **5. Future Enhancements**  
- **Chat Support** – For student-instructor communication.  
- **Multi-language Support** – Expand to non-Amharic users.  
- **Gamification** – Badges and rewards for course completion.  

---

# **Brushed By  Betty Makeup Artistry Online Learning App Development Plan (4-Month Timeline)**  


## **Phase 1: Planning & Requirement Analysis (2 Weeks)**
### **Tasks:**
1. **Define Project Scope & Features**  
   - Mobile App (Student & Instructor Views)  
   - Web Admin Dashboard (Admin & Instructor Access)  
   - Microservices Breakdown (Auth, Courses, Messaging, Certifications, Notifications, Assignments)  
   - User Roles & Permissions  

2. **Wireframing & UI/UX Design**  
   - Mobile App Screens (Login, Courses, Assignments, Messaging, Certifications)  
   - Admin Dashboard Screens (User Management, Course Management, Notifications)  

3. **Tech Stack Selection**  
   - **Frontend:** React Native (Mobile), React.js (Admin Dashboard)  
   - **Backend:** Node.js (Express/NestJS)  
   - **Database:** PostgreSQL/MongoDB (Per Microservice)  
   - **Authentication:** JWT/OAuth  
   - **Cloud:** AWS/Azure (For Deployment)  
   - **CI/CD:** GitHub Actions/Docker  

4. **Project Documentation**  
   - Functional & Technical Requirements  
   - API Contracts (Swagger/Postman)  

### **Time Allocation:**  
- Week 1: Scope Definition & Wireframing  
- Week 2: Tech Stack Finalization & Documentation  

---

## **Phase 2: Backend Development (6 Weeks)**
### **Microservices Breakdown:**  
1. **Authentication & User Management (1 Week)**  
   - User Registration/Login (Students, Instructors, Admins)  
   - Role-Based Access Control (RBAC)  

2. **Course Management (1.5 Weeks)**  
   - Course Creation/Updation  
   - Instructor Assignment  
   - Enrollment System  

3. **Messaging Service (1 Week)**  
   - Real-time Chat (Student-Instructor)  
   - Notifications  

4. **Assignments & Submissions (1 Week)**  
   - Assignment Creation  
   - Submission & Grading  

5. **Certification Service (1 Week)**  
   - Course Completion Certificates  
   - Verification System  

6. **Notification Service (0.5 Week)**  
   - Email/Push Notifications  

### **Time Allocation:**  
- Week 3-4: Auth, Course Management  
- Week 5: Messaging & Assignments  
- Week 6: Certification & Notifications  
- Week 7: API Integration Testing  

---

## **Phase 3: Frontend Development (5 Weeks)**
### **Mobile App (React Native) – 3 Weeks**  
- **Authentication Flow** (Login/Signup)  
- **Course Browsing & Enrollment**  
- **Assignment Submission**  
- **Messaging & Notifications**  
- **Certificate Download**  

### **Admin Dashboard (React.js) – 2 Weeks**  
- **User & Course Management**  
- **Instructor Assignment**  
- **Notification & Announcement System**  
- **Analytics & Reports**  

### **Time Allocation:**  
- Week 8-10: Mobile App Development  
- Week 11-12: Admin Dashboard Development  

---

## **Phase 4: Testing & Deployment (3 Weeks)**
### **Tasks:**  
1. **Integration Testing (1 Week)**  
   - API & Microservice Testing (Postman/Jest)  
   - Mobile App Testing (Manual & Automated)  

2. **User Acceptance Testing (UAT) (1 Week)**  
   - Beta Testing with Selected Users  
   - Bug Fixes  

3. **Deployment (1 Week)**  
   - Backend (AWS ECS/Kubernetes)  
   - Mobile App (App Store/Play Store)  
   - Admin Dashboard (Hosting on AWS/Azure)  

### **Time Allocation:**  
- Week 13: Integration Testing  
- Week 14: UAT & Bug Fixes  
- Week 15: Deployment & Final Review  

---

## **Final Deliverables (Week 16)**
✅ **Fully Functional Mobile App** (iOS & Android)  
✅ **Admin Dashboard** (Course, User, Assignment Management)  
✅ **Microservices Backend** (Scalable & Secure)  
✅ **Documentation & Handover**  

---

### **Risk Management & Buffer Time**
- **Potential Delays:**  
  - Third-party API integrations (Payment, Notifications)  
  - App Store/Play Store Approval  
- **Buffer Time:** 1 Week (Adjustments in Testing Phase)  

---

### **Summary Timeline**
| **Phase** | **Duration** | **Key Tasks** |
|-----------|------------|--------------|
| **Planning & Design** | 2 Weeks | Scope, Wireframes, Tech Stack |
| **Backend (Microservices)** | 6 Weeks | Auth, Courses, Messaging, Certifications |
| **Frontend (Mobile + Dashboard)** | 5 Weeks | React Native App, React.js Admin |
| **Testing & Deployment** | 3 Weeks | QA, UAT, Cloud Deployment |
| **Final Review** | 1 Week | Bug Fixes, Documentation |

