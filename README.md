# SDC310 Week 5 Performance Assessment: Cookie & Session Management

**Student Name:** Todd Upshaw  
**Course:** SDC310 - PHP Web Application Development  
**Date:** October 1, 2026  
**Repository:** [Upshaw_wk5pa](https://github.com/toddupshawdevops-design/Upshaw_wk5pa)

---

## Project Overview

This PHP web application demonstrates state management techniques across multi-page web applications using **Cookies** and **Sessions**. The application consists of a two-page workflow where user identity (Name) is persisted across browsing sessions via browser cookies, and sensitive or temporary session data (Date of Birth) is maintained securely using PHP server-side sessions.

---

## Technical Features

* **Cookie Persistence:** Captures the user's name via an HTTP POST request and stores it in a browser cookie (`user_name`) with a 30-day expiration window.
* **Session State Management:** Initializes a PHP session (`session_start()`) to temporarily store the user's Date of Birth (`$_SESSION['user_dob']`) on the server.
* **Form Pre-population:** Auto-fills form inputs on the data entry page using active cookie and session variables.
* **Data Retrieval & Rendering:** Sanitizes user inputs using `htmlspecialchars()` and dynamically renders stored values on a secondary display page.
* **Navigation & UI:** Built with clean, responsive CSS card containers and inter-page navigation links.

---

## File Structure

```text
Upshaw_wk5pa/
├── data_entry.php    # Form page to input and persist Name (Cookie) and DOB (Session)
├── data_display.php  # Output page retrieving and displaying stored Cookie and Session values
└── README.md         # Project documentation
