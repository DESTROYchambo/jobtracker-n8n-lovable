# 🚀 JobTracker n8n+lovable

A modern minimalist dashboard designed for tracking job applications, interviews, and offers. Created to optimize the job search process with a focus on UX (user experience) and reliable data storage.

Application link: https://jobtrackern8n.lovable.app

## 🛠 Technical Stack

* **Frontend:** React (powered by Lovable.dev), Tailwind CSS, TanStack Query.
* **Backend:** n8n.
* **Database:** PostgreSQL.
* **Архітектура:** Client-server model using REST API via webhooks.

## ✨ Key Features

* **Dashboard view**: Kanban board or application grid with color-coded statuses (Applied, Interview, Offer, Rejected).
* **Real-time CRUD**: Instant creation, viewing, updating, and deletion of job records.
* **Smart date handling**: Display of relative time (e.g., "Applied 2 days ago") with reliable error handling for empty or invalid dates.
* **Optimistic UI**: The interface updates instantly after user actions (deletion/editing) without waiting for a server response, providing an immediate application reaction.
* **State persistence**: User authorization and data remain consistent after page reloads (localStorage + Postgres synchronization).

## Usage Instructions

* Open the web application.
  
* Enter the admin login and password (admin admin).
  
  <img width="408" height="455" alt="image" src="https://github.com/user-attachments/assets/ce4a63c3-5e98-4f19-885e-6c659e2a9161" />

* The admin panel will open, displaying all added job records. To add a new record, click the Add Application button on the right side of the application.
  
  <img width="1330" height="465" alt="Знімок екрана 2026-02-10 193123" src="https://github.com/user-attachments/assets/2dc4e268-4f7e-405d-b8d7-f584452776ed" />

* Fill in the data and add the record.

   <img width="549" height="649" alt="image" src="https://github.com/user-attachments/assets/8007aa85-c6b9-47d5-b165-fd066fa4b78e" />

   <img width="879" height="220" alt="image" src="https://github.com/user-attachments/assets/0185fa8f-a2cc-4c03-b5cb-ce9400742228" />

* To modify data, hover over the three dots in the top right corner of the record. Select Edit, and change the desired data.

   <img width="453" height="211" alt="Знімок екрана 2026-02-10 193717" src="https://github.com/user-attachments/assets/164686be-5b77-489b-8a5c-26fc3865ebbf" />

   <img width="429" height="195" alt="image" src="https://github.com/user-attachments/assets/1acc4883-b1b5-483a-826b-77b52c43b9ca" />

  <img width="436" height="199" alt="image" src="https://github.com/user-attachments/assets/fdc11091-5a14-4fa4-affb-aadf7366c688" />
  
* To delete a record, hover over the three dots in the top right corner of the record and click Delete. The record will then be deleted.

   <img width="590" height="281" alt="image" src="https://github.com/user-attachments/assets/779be886-d5c7-40ca-a209-4a736d12798d" />
   
* The application includes a feature to search records by company or position, as well as filter records by status.

   <img width="1132" height="262" alt="image" src="https://github.com/user-attachments/assets/0be90546-9daf-4bf0-af38-1388dbf739e8" />

   <img width="1143" height="290" alt="image" src="https://github.com/user-attachments/assets/f91b8f46-1feb-4975-8810-e1ce75f01c60" />

   <img width="1132" height="279" alt="image" src="https://github.com/user-attachments/assets/ba25427e-8c56-4e28-9b18-b91980b43dd8" />

* Records in the database

  <img width="811" height="183" alt="image" src="https://github.com/user-attachments/assets/7c97e763-698c-4322-8db4-2ea0da3bc619" />

---

## 🔮 Future Plans (Upgrade to ATS platform)

I am planning on scaling this project into a fully functional dual-role Applicant Tracking System (ATS).

**Planned features:**

* **Role-Based Access Control (RBAC):** Separation of rights and responsibilities between `Admin` (Recruiter) and `Candidate`.
* **Candidate Portal:**
    * Registration and login system.
    * "Available Vacancies" section, where users can apply for open positions in one click.
    * Personal dashboard to track the status of their own applications.
* **Administrator Workflow:**
    * Publishing new "Open" vacancies.
    * Viewing incoming applications from registered users.
    * Moving candidates through the pipeline (Applied -> Interview -> Offer).
* **Database expansion:** Adding a `Users` table and setting up relationships between Users and Vacancies.
