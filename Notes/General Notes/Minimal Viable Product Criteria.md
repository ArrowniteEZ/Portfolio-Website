MVP Features
1. Public Portfolio
-Home page
    -Display name
    -Display professional title
    -Short introduction
    -Navigation bar
    -Call-to-action button ("View Projects")
    -Footer with social links

-About page
    -Profile photo/avatar
    -Biography
    -Education
    -Technical skills
    -Resume download button

-Projects page
    -Display all projects as cards
    -Each card shows:
        -Title
        -Thumbnail/image
        -Short description
        -Technologies used
    -Clicking a card opens a detailed page with:
        -Full description
        -GitHub link
        -Live demo link (optional)
        -Additional screenshots
    -Allow sorting (Newest, Oldest)
    -Allow filtering by technology (optional MVP+)
    
-Contact page
    -Form fields:
        -Name
        -Email
        -Subject
        -Message
    -Client-side validation
    -Server-side validation
    -Success/error message
    -Save submission to database

2. Admin Panel
-Authentication
    -Login page
    -Username/password
    -Password hashing
    -Session or JWT authentication
    -Logout
    -Prevent unauthorized access
    -Prevent SQL Injection

-Dashboard
    -Number of projects
    -Number of contact messages
    -Recent messages
    -Navigation sidebar

-Project Management
    -View Projects
        -Table of all projects
        -Search by title
        -Sort by date
    
    -Create Project
        -Fields:
            -Title
            -Description
            -Technologies
            -GitHub URL
            -Demo URL
            -Thumbnail image URL
            -Featured (Yes/No)

    -Edit Project
        -Modify any project field
        -Save changes

    -Delete Project
        -Confirmation dialog
        -Delete from database


Contact Message Management
    -View Messages
        -Display:
            -Name
            -Email
            -Subject
            -Date
            -Read/Unread

    -Read Message
        -Full message
        -Mark as read
    
    -Delete Message
        -Delete selected message

Error Handling
    -404 page
    -Invalid form feedback
    -Unauthorized page
    -Database errors specifically handled 
    -Logging for server errors



How Layers Are Incorporated:
Presentation: 
    -HTML/CSS/JS (or React/Vue)
    -Forms
    -Displaying projects and messages

Application:
    -Routes/API endpoints
    -Authentication
    -Request validation
    -Coordinating services

Business Logic:	
    -Rules like "only admins can edit projects"
    -Filtering/sorting projects
    -Validating business rules

Data Access:
    -Repository/DAO classes that perform database queries

Database: 
    -Tables for: 
        -Users
        -Projects
        -ContactMessages