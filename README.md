# Campus Bites - Campus Cafeteria Information Website

A collaborative web project developed for the **DevOps Fundamentals** course at the **University of Central Punjab**.

---

## Project Overview
**Campus Bites** is a responsive informational website designed to help students and staff easily discover cafeteria menus, daily specials, ordering guidelines, and contact details. 
The primary goal of this project is to practice hands-on collaborative software development using Git and GitHub workflows, including feature branching, pull requests, branch protection rules, interactive rebasing, and release management.

---

## Repository Structure
```text
campus-cafeteria/
│
├── .gitignore
├── README.md
├── src/
│   ├── index.html       # Home Page (Team Lead)
│   ├── menu.html        # Menu Page (Member 1)
│   ├── deals.html       # Daily Specials & Deals (Member 2)
│   ├── order.html       # How to Order Guide (Member 3)
│   └── feedback.html    # Feedback & Contact Form (Member 4)
└── styles/
    └── style.css        # Shared responsive stylesheet
```

---

## Team Details & Page Assignments

| Sr # | Student Name | University Email | GitHub Username | Role | Branch Worked On | Assigned Page |
| :---: | :--- | :--- | :--- | :---: | :--- | :--- |
| **1** | *[Team Lead Name]* | *[email@ucp.edu.pk]* | *[username]* | Team Lead | `main`, `develop`, `release/v1.0` | `index.html` (Home) |
| **2** | *Raveeha Fatima* | *[L1f23bsse0045@ucp.edu.pk]* | *raveehafatima* | Member 1 | `feature/menu-page` | `menu.html` (Menu) |
| **3** | *[Member 2 Name]* | *[email@ucp.edu.pk]* | *[username]* | Member 2 | `feature/deals-page` | `deals.html` (Deals) |
| **4** | *[Member 3 Name]* | *[email@ucp.edu.pk]* | *[username]* | Member 3 | `feature/order-page` | `order.html` (Order Guide) |
| **5** | *[Member 4 Name]* | *[email@ucp.edu.pk]* | *[username]* | Member 4 | `feature/feedback-page` | `feedback.html` (Feedback) |

---

## Tech Stack & Rules
* **Frontend:** Plain HTML5 & CSS3 (using CSS Media Queries for responsiveness)
* **Design Rule:** All HTML files link to the shared stylesheet via `../styles/style.css`.
* **Version Control:** Git & GitHub

---

## Git Branching Strategy & Workflow
1. **`main`**: Production-ready code (Protected: Requires 3 PR approvals before merge).
2. **`develop`**: Active development and integration branch (Protected: Requires 2 PR approvals before merge).
3. **`feature/<page-name>`**: Individual feature branches created from `develop` by team members.
4. **`release/v1.0`**: QA and final testing branch created from `develop` prior to production release.

### Daily Member Workflow:
```bash
# 1. Fetch latest updates from develop
git fetch origin
git checkout develop
git pull origin develop

# 2. Rebase feature branch before opening Pull Request
git checkout feature/<your-page>
git rebase origin/develop

# 3. Resolve conflicts locally (if any) and push updates
git push origin feature/<your-page>
```

---

## How to Run Locally
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd campus-cafeteria
   ```
2. Open `src/index.html` in your web browser.
