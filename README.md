# TaskTrack Android Mobile Application Project Outline
### Prepared by Devon Moore
### Course: Mobile Application Development COM-437-OL01
### Instructor: Dr. Marwan Omar
### Date: August 31, 2026

## Purpose: This outline describes the Android application I plan to design and develop during the term. The project is called TaskTrack, a mobile assignment and deadline tracker intended to help students keep schoolwork organized in one place. The outline explains the problem the app addresses, the planned platform and technology, expected functions, and the initial screen design.

## I. Project Description
•	Application name: TaskTrack
•	Application type: Student productivity and assignment-tracking application
•	Primary users: College and high-school students who need a simple way to organize coursework and deadlines.
•	Main idea: TaskTrack will let a student enter classes and assignments, assign due dates and priorities, mark work as complete, and view upcoming deadlines from a simple dashboard.
•	Project goal: The goal is to create a useful Android app that demonstrates mobile interface design, user input, local data storage, navigation, validation, and device notifications.

## II. Problem Being Addressed
Students often receive deadlines from several places, including course websites, email, syllabi, and classroom announcements. When assignments are spread across different systems, it is easy to forget a due date or lose track of what should be completed first. A general calendar can help, but it does not always provide a clear school-focused view of courses, assignments, priorities, and completion status.
TaskTrack addresses this problem by giving the user one organized location for school assignments. Instead of trying to remember every deadline, the user can enter the assignment once and check the app for upcoming work. The app will also make it easier to identify overdue items and assignments that are due soon.

## III. Platform
•	Operating system: Android
•	Development environment: Android Studio
•	Programming language: Kotlin
•	User interface: XML-based Android layouts and standard Material-style controls
•	Target device: Android smartphone; the final version will be demonstrated on a real mobile device
•	Version control: Git and GitHub will be used to store source code and project documentation

## IV. Front-End and Back-End Support
### A. Front End
The front end will be the part of TaskTrack that the user sees and interacts with. It will be built in Android Studio using Kotlin and XML layouts. The interface will focus on a clean layout with clear buttons, readable text, and simple navigation. The main screens will include a dashboard, assignment list, add/edit assignment form, course list, and assignment details.

### B. Back End
The first version of TaskTrack will use a local Room database, which provides an Android-friendly way to store structured data on the device. The database will hold course and assignment information such as title, course, due date, priority, notes, and completion status. A local database is a good fit for this project because the basic app can work without requiring the user to create an online account.
Android notification support will be used for assignment reminders. If time allows later in the term, a cloud backup or sign-in feature could be explored as an enhancement, but it is not required for the first working version.

## V. Planned Functionality
•	Add, edit, and delete courses.
•	Add, edit, and delete assignments.
•	Enter an assignment title, course, due date, priority level, and optional notes.
•	View assignments in a list and sort or group them by due date.
•	Display upcoming assignments on a dashboard.
•	Clearly identify overdue assignments.
•	Mark an assignment as completed and separate completed work from active work.
•	Validate required fields so an assignment cannot be saved without basic information.
•	Use local storage so information remains available after the app is closed.
•	Provide reminder notifications for upcoming assignments.

## VI. Design and Wireframes
The interface is intended to be simple enough to use quickly between classes. The wireframes below show the basic organization of the most important screens. These are early designs and may change slightly as the application is developed and tested.

## Wireframe 1 - Dashboard
### TASKTRACK
### Today | Upcoming | Completed
### Next Due: Database Quiz - Sep. 3
### Web Design Project - Sep. 5
### Android Outline - Sep. 7
### [ + ADD ASSIGNMENT ]
### Home     Courses     Assignments


## Wireframe 2 - Add Assignment
### ADD ASSIGNMENT
### Assignment Title: __________________
### Course: [ Select Course ▼ ]
### Due Date: [ MM / DD / YYYY ]
### Priority: [ Low ] [ Medium ] [ High ]
### Notes: _____________________________
### [ SAVE ASSIGNMENT ]
### [ CANCEL ]


## Wireframe 3 - Assignment List
### ASSIGNMENTS
### [ Search assignments... ]
### ☐ Android Project      Sep. 7   HIGH
### ☐ Database Quiz        Sep. 3   MED
### ☑ Chapter Questions    Aug. 30  DONE
### [ Filter ▼ ]   [ Sort by Due Date ▼ ]
### [ + ADD ]
### Home     Courses     Assignments


## Wireframe 4 - Assignment Details
### ASSIGNMENT DETAILS
### Android Project Outline
### Course: Mobile App Development
### Due: Sep. 7
### Priority: High
### Notes: Finish outline and GitHub README.
### [ MARK COMPLETE ]
### [ EDIT ]      [ DELETE ]


## VII. Basic Data Design
TaskTrack will use two main data groups: Course and Assignment. A course can have many assignments, while each assignment will belong to one course. Keeping the data separated this way will make it easier to update a course without repeating the same information for every assignment.
Entity	Sample Fields	Purpose
Course	courseId, courseName, instructor, colorLabel	Stores the classes the student is taking.
Assignment	assignmentId, courseId, title, dueDate, priority, notes, completed	Stores individual tasks and links each one to a course.
## VIII. Development and Testing Goals
1.	Create the basic project and navigation structure in Android Studio.
2.	Build the main screens shown in the wireframes.
3.	Create the Room database and connect the forms to stored data.
4.	Add assignment completion, sorting, and reminder features.
5.	Test required-field validation and common user actions.
6.	Test the final application on an actual Android mobile device.
7.	Correct usability or layout problems found during testing.

GitHub Repository/README Link: 

GitHub Wiki Link: 
