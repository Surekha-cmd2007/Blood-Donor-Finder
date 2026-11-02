# Blood Donor Finder

A web-based platform that helps connect people who need blood with registered blood donors. Users can search for donors using blood group and location, submit blood requests, receive responses, and track request progress.

> **Project stage:** Initial repository setup. This repository contains the planned structure and project documentation. Application features are not implemented yet.

---

## 1. Problem Statement

Finding a suitable blood donor quickly can be difficult, especially during emergencies. People may have to contact multiple individuals or groups to locate someone with the required blood group nearby.

Blood Donor Finder aims to make this process more organized by providing one platform where donors can register and people in need can submit blood requests.

## 2. Project Objectives

- Make it easier to find registered blood donors.
- Support searching by blood group and location.
- Allow users to submit and manage blood donation requests.
- Notify potentially eligible registered donors about matching requests.
- Allow requesters to track request status.
- Provide an admin dashboard to monitor users and requests.
- Protect donors' personal information and avoid exposing contact details publicly.

## 3. Intended Users

### Donor
- Create an account and register donor details.
- Provide blood group and general location.
- Update donation availability.
- Receive relevant blood request notifications.
- Choose whether to respond to a request.

### Requester
- Register or log in.
- Search for donors by blood group and location.
- Submit a blood request with the required details.
- View donor responses and track request status.

### Administrator
- Manage donor and requester accounts.
- Review and monitor blood requests.
- Handle reported or suspicious activity.
- View basic platform statistics.

## 4. Planned Features

| Feature | Description |
|---|---|
| Donor registration | Allows willing donors to create a profile. |
| Authentication | Provides secure registration and login. |
| Donor search | Filters registered donors by blood group and location. |
| Blood request | Allows a requester to submit a blood requirement. |
| Donor notifications | Notifies matching donors about relevant requests. |
| Request tracking | Shows whether a request is pending, accepted, fulfilled, or closed. |
| Admin dashboard | Helps administrators monitor users and requests. |
| Privacy controls | Restricts access to personal and contact information. |

## 5. Proposed Technology Stack

The following stack is proposed for the initial implementation and may be adjusted during development.

| Layer | Proposed technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python with Flask |
| Database | MySQL |
| Version control | Git and GitHub |
| Notifications | Email or SMS service (to be evaluated) |

## 6. High-Level Workflow

1. A donor registers and provides their blood group, location, and availability.
2. A requester submits a blood request with the required blood group and location.
3. The system searches for matching registered donors.
4. Eligible matching donors are notified without making their private contact details public.
5. Donors can choose to respond to the request.
6. The requester can view responses and track the request status.

**Important:** The platform is intended to help people discover and contact potential donors. Final donor eligibility, blood-group compatibility, and transfusion decisions must always be confirmed by qualified medical professionals or an authorized blood bank.

## 7. Privacy and Security

Donor privacy is a core project requirement.

- Do not display donor phone numbers, email addresses, or other private contact details publicly.
- Collect only information needed for the platform's purpose.
- Use authentication and role-based access control.
- Restrict personal information to authorized users and legitimate request workflows.
- Obtain donor consent before sharing contact information.
- Protect stored data and avoid committing passwords, API keys, or secrets to GitHub.

## 8. Planned Project Structure

```text
Blood-Donor-Finder/
├── frontend/
│   ├── index.html
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── assets/
├── backend/
│   ├── app.py
│   ├── routes/
│   ├── models/
│   └── requirements.txt
├── database/
│   └── schema.sql
├── docs/
│   └── project-overview.md
├── .gitignore
└── README.md
```

## 9. Project Status and Next Steps

**Current status:** Initial project structure and documentation.

Planned development steps:
1. Finalize requirements and user roles.
2. Design the database tables and relationships.
3. Build the frontend pages.
4. Develop backend APIs and authentication.
5. Implement donor search and blood request workflows.
6. Add notifications and request tracking.
7. Build the admin dashboard.
8. Test privacy, security, and application workflows.

## 10. Disclaimer

Blood Donor Finder is a coordination platform, not a substitute for a hospital, licensed blood bank, or medical professional. Donor eligibility and transfusion compatibility must be verified by qualified professionals.

---

**Repository:** Blood-Donor-Finder  
**Project type:** Web application  
**Status:** Initial setup
