```mermaid
%%{init: {'themeVariables': {'actorBorder': 'black', 'actorBkg': 'white', 'actorTextColor': 'black'}}}%%
usecaseDiagram
    actor User as "👩💻 User (Student/Faculty)"
    actor Admin as "👨💼 Admin"
    
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
    
    UC2 .> (Handle Compile Errors) : extends
    UC4 .> (Report Post) : extends
    UC1 <.. (Two-Factor Auth) : includes
    
    note for UC2 "Validates code against test cases\nand checks for plagiarism"
    note for UC8 "Sets time/memory constraints\nand difficulty levels"
```
