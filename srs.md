# **Software Requirements Specification (SRS)**

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to define the functional and non-functional requirements for the development of a centralized repository website for **previous year question papers and remedial materials**. The website will provide users with the ability to search, download, and optionally upload academic resources.

### 1.2 Scope
This project focuses on developing a user-friendly website that serves as a centralized repository for students to access and download exam papers and remedial materials. Additional features such as a community forum and upload functionality can be implemented in future iterations.

### 1.3 Audience
- **Primary users**: Students looking for exam preparation materials.
- **Secondary users**: Educators and contributors who wish to add or access resources.
- **Developers**: Responsible for maintaining and expanding the platform.

### 1.4 Definitions and Acronyms
- **SRS**: Software Requirements Specification
- **User**: Any registered or unregistered individual accessing the website.
- **Repository**: Collection of exam papers and remedial materials.

---

## 2. System Overview

The website will function as a centralized platform for students to easily search and download past exam papers and remedial materials. It will feature an intuitive user interface with essential functionalities, and will be scalable for future additions like forums or user-uploaded content.

---

## 3. Functional Requirements

### 3.1 Search Functionality
- **Description**: Users can search for materials by filtering based on subject, course level, and year.
- **Input**: Search terms such as "subject", "course level", "year".
- **Process**: The system filters available documents based on the search criteria.
- **Output**: A list of matching materials for download.

### 3.2 Download Functionality
- **Description**: Users can download the selected documents in PDF or Word format.
- **Input**: Selection of a document to download.
- **Process**: The system allows the user to download the chosen document.
- **Output**: A downloadable file in the user's preferred format.

### 3.3 User Registration & Login
- **Description**: Users can register and log in to access additional features.
- **Input**: User details such as name, email, password.
- **Process**: The system verifies user credentials and grants access upon successful login.
- **Output**: User access to upload functionality and other privileged features.

### 3.4 Upload Functionality (Future plan)
- **Description**: Registered users can upload exam papers and remedial materials.
- **Input**: Document file, metadata (e.g., subject, year).
- **Process**: Uploaded content is reviewed for copyright compliance before being made publicly available.
- **Output**: The file is added to the repository for other users to access.

### 3.5 Community Forum (Future plan)
- **Description**: Users can engage in discussions, share tips, and ask questions.
- **Input**: Posts, replies, comments.
- **Process**: Real-time updates allow for interactive conversations.
- **Output**: Threads of discussions accessible to all users.

---

## 4. Non-Functional Requirements

### 4.1 Usability
- The website will feature a clean, easy-to-navigate interface.
- Users should be able to access resources with minimal effort and training.

### 4.2 Performance
- The system should handle multiple concurrent searches and downloads.
- Search results should appear in under 2 seconds.

### 4.3 Scalability
- The website must support future growth, including user-uploaded content and additional features such as a community forum.

### 4.4 Security
- User data (e.g., passwords, emails) must be encrypted.
- Uploaded content should undergo copyright compliance checks before approval.

### 4.5 Availability
- The system should maintain a minimum of **99% uptime**, ensuring access during critical periods like exams.

---

## 5. System Design Constraints

### 5.1 Technology Stack
- **Frontend**: Angular 18
- **Backend**: Spring Boot handling all user requests and interactions with the database.
- **Database**: MySQL (or MongoDB) for storing exam papers, user data, and forum discussions.
- **Hosting**: The system will be hosted on a cloud provider like AWS  for scalability and high availability.

---

## 6. Risks and Assumptions

### 6.1 Risks
- **Data Integrity**: Ensuring all uploaded materials are free from errors and are legitimate.
- **Copyright Issues**: Handling uploaded content in compliance with copyright laws.

### 6.2 Assumptions
- Students will use the platform primarily for educational purposes.
- Contributors will be willing to share content while respecting copyright laws.
- The initial scope will focus on search and download functionalities, with the possibility of future expansions.

---

## 7. Appendices

### 7.1 Future Enhancements
- **Integration with Learning Management Systems (LMS)** for a more comprehensive academic tool.
- **Mobile Application** to make the platform accessible from mobile devices.
- **Gamification** to encourage student participation and content contribution.
