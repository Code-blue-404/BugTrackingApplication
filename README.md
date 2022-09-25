# Bug Tracking Application


The final project submission is in the folder Bug Tracking Project Deliverables or the zip file with the same name committed on 25/10/2022. 

Team Members:

Aanchal Chaurasia

Ayushman Mookherjee

Medha Chaudhary

Sakshi Singh

Suruchi Balasaheb Bhujbal

Tushar Ojha

Vidha Pandey

Yashvardhan Sharma

----------------------------------------------------------

Given are the functionalities of various modules implemented :-

(A) Bean classes

1. User - User class, parent of ProjectManager, Tester and Developer which contains details about all users.
2. Bug - Bug class that stores information about various bugs.
3. Project - Project class containing details about the project.
4. Developer - Developer class, child of User, to store data about the developers.
5. Project Manager - Project Manager class, child class for User, to store details about the project managers.
6. Tester - Tester class, child of User, for details about the tester.


(B) Dao layer classes and Interfaces

1. BugTrackDao - Interface for database layer (Dao layer) having function definitions of the layer.
2. BugTrackDaoImpl - This class contains the implementation of the functions defined in the BugTrackDao Interface.
3. DBUtil - provides singleton factory pattern for jdbc.
4. RegisterDao - Interface for registration.
5. RegisterDaoImpl - Implementation of registration.
6. UserDao - Interface for database layer (dao layer).
7. UserDaoImpl - Establish connection with derby db & run queries to fetch/add/modify data.

(C) Exceptions classes

1. BugNotFoundException - Exception for handling when a bug is not found.
2. ErrorInExecutionException - Exception for handling error in execution of code.
3. InvalidUserException - Exception when user is invalid.
4. UserNotFoundException - Exception when the user is not found.

(D) Service layer classes and Interfaces

1. BugTrackService - Interface for business logic layer.
2. BugTrackServiceImpl - Provide business logic to the bug tracking service.
3. RegisterService - Interface for business logic for registration.
4. RegisterServiceImpl - Provides business logic for registration.
5. UserService - Interface for service layer.
6. UserServiceImpl - class for service layer.

(E) Servlets

1. ImportUsersServlet - For importing users to the database.
2. MyLoginServlet - servlet for login (session created).
3. LogoutServlet - To logout of the system (session invalidated).
4. RegisterServlet - For registering a user.
5. AddProject - Adding of new project by manager.
6. PMCreateProject - For creating a new project and transferring to CreateProject.jsp for getting info about the project.
7. DisplayPMBugsServlet - To display bug list for the project chosen by the project manager.
8. DisplayPMProjectsServlet - To display the projects created by the project manager.
9. PMAssign - For assigning the developer to a bug.
10. PMCloseBug - For closing the bugs marked by the developers.
11. AddRemarks - Servlet to add remarks when developer marks a bug for closing.
12. AssignDevServlet - To get the list of developers for assigning them to a bug.
13. DisplayDeveloperBugsServlet - Servlet to display bugs from a specific project.
14. DisplayDeveloperProjectsServlet - To display projects assigned to the developer.
15. DisplayTesterBugsServlet - To display bugs of the project chosen by the tester.
16. DisplayTesterProjectsServlet - To display projects assigned to the tester.
17. GetBugInfoServlet - Used to get info about the new bug from addbug.jsp form.
18. TempBugServlet - For redirecting the page to AddNewBug.jsp and autofilling some details.