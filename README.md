# ⚽ Football Match & Team Management System

This is a modern web application designed to manage football teams, players, and matches. The platform allows users to view teams, schedule matches, and track player performance. It also features advanced analytics tools for administrators, such as top players, most active teams, and most played matches. The application is built with a cutting-edge tech stack and a robust relational database.

---

## 🚀 Features

### ⚙️ User Features

#### 📅 Match Scheduling
- Users can schedule matches by selecting teams, date, time, and location.
- Matches can be categorized (e.g., Friendly, Tournament, League).

#### 🧑‍🤝‍🧑 Team & Player Management
- View teams and their associated players.
- View player profiles with stats (goals, assists, appearances).

#### 📆 View Matches
- Users can see all upcoming and past matches with detailed information (teams, date, location, result).

---

### 🔑 Admin Features

#### 📊 Advanced Analytics
- **Top 3 Players**: Players with the most goals/assists.
- **Top 3 Teams**: Teams with the most matches played.
- **Top 3 Matches**: Most attended matches.
- **Top 3 Days**: Days with the highest number of scheduled matches.

#### 🛠️ Team Management
- Add, update, and delete teams and assign players to teams.

#### 🧍‍♂️ Player Management
- Manage player profiles, including stats and personal information.

---

## 🌐 Dynamic Navigation
Responsive navbar with links to **Home**, **Teams**, **Matches**, **Players**, and **Contact** pages.

---

## 🔒 User Authentication
- **Signup/Login**: Secure user registration and login with bcrypt-based password hashing.
- **Role Management**: Distinction between normal users and admin users for privileged operations.

---

## 🗄️ Database Structure

The application is powered by a **MySQL relational database** with the following tables:

| Table        | Description                                  |
|--------------|----------------------------------------------|
| **Users**    | Stores user information and hashed passwords.|
| **Teams**    | Stores football teams and their info.        |
| **Players**  | Player profiles linked to teams.             |
| **Matches**  | Scheduled matches linked to teams.           |
| **Categories** | Types of matches (Friendly, League, etc.). |

### Key Relationships:
- **Matches** link to **Teams** (home & away).
- **Players** link to **Teams**.
- **Matches** link to **Categories** for match type.

---

## 💻 Technologies Used

### Frontend
- **React.js**: Modular, component-based user interface.
- **CSS**: Customized responsive styles for modern UI/UX.
- **Responsive Design**: Fully mobile-friendly.

### Backend
- **Node.js & Express.js**: RESTful APIs for database interaction.
- **MySQL**: Relational database for structured data and complex queries.

---

## 🔌 Endpoints Overview

### 🔍 Simple Queries (JOINs)
- Retrieve all matches for a specific team.
- List all players along with their team.
- Show most active teams based on match count.
- Display top players and their stats.
- Highlight most played matches.
- Summarize team performance statistics.

### 🔑 Complex Queries (Subqueries)
- Find top players with the most goals/assists.
- Identify top 3 teams based on matches played.
- List top 3 matches based on attendance or importance.
- Highlight top 3 days with the most scheduled matches.


