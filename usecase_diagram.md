```mermaid
usecaseDiagram
    actor User as "User (Student/Faculty)"
    actor Admin as "Admin"
    
    (Login) as UC1
    (Submit Code) as UC2
    (View Leaderboard) as UC3
    (Post in Forum) as UC4
    (Solve Challenges) as UC5
    (Reset Password) as UC6
    
    (Manage Users) as UC7
    (Create Challenges) as UC8
    (Review Submissions) as UC9
    (Moderate Forum) as UC10
    
    User --> UC1
    User --> UC2
    User --> UC3
    User --> UC4
    User --> UC5
    User --> UC6
    
    Admin --> UC1
    Admin --> UC7
    Admin --> UC8
    Admin --> UC9
    Admin --> UC10
```
