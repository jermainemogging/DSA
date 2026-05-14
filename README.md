SMART STUDY PLANNER SYSTEM
Created By: Jermaine Encinares, CS-1203
Final Project for the Course CC 102 | Advanced Computer Programming

📖 Project Overview
The Smart Study Planner System is a C++ console-based application designed to help students organize and manage their academic tasks efficiently. The system allows users to create, search, update, delete, and prioritize study tasks while keeping records saved using file handling.
The application uses C++ structures (struct) and dynamic arrays (vector) to organize task information and provide efficient task management operations. It also implements sorting and searching algorithms to improve task organization and accessibility.
The system was developed using procedural programming concepts and standard C++ libraries without relying on external frameworks or databases.

🔄 How the System Works
The application provides several core operations that simulate a real-world study planner workflow:
Add Task
Users can create new study tasks by entering a title, description, deadline, and priority level.
View Tasks
Displays all saved tasks together with their priority, completion status, and deadlines.
Search Task
Allows users to search tasks using keyword matching based on task titles.
Mark Completed
Updates a selected task’s status from “Pending” to “Completed.”
Delete Task
Removes unnecessary or completed tasks from the system.
Save and Load Tasks
Uses file handling to permanently store tasks in a text file and automatically reload them when the program starts.
Task Statistics
Displays total tasks, completed tasks, pending tasks, and overall completion percentage.

✨ Features
Dynamic task management using vector<Task> 
Task prioritization using Bubble Sort 
Keyword-based task searching 
File handling for persistent storage 
Completion tracking system 
Task statistics and completion percentage 
Automatic task sorting by priority 
Input validation for task selection 
Console-based menu navigation 
Organized modular functions for easier maintenance 

🧠 Technical Deep Dive: Why Structs and Vectors?
The system uses a Task struct to group all related task information into a single custom data structure. Each task stores the title, description, deadline, priority, and completion status.
Instead of fixed-size arrays, the program uses std::vector<Task> to dynamically manage multiple tasks. Vectors automatically resize depending on the number of tasks entered by the user, making the system more flexible and memory efficient.
Bubble Sort is used to arrange tasks according to priority levels (High, Medium, Low), while Linear Search is used for keyword-based task searching.

🛠️ Technical Details
Component	Description
Language	C++
Programming Style	Procedural Programming
Data Structure	struct and std::vector
Sorting Algorithm	Bubble Sort
Searching Algorithm	Linear Search
File Handling	ifstream and ofstream
Libraries Used	<iostream>, <vector>, <fstream>, <string>, <cstdlib>

🧩 Core Data Structure
struct Task {
    string title;
    string description;
    string deadline;
    string priority;
    string status;
};

📄 Sample Output
===== SMART STUDY PLANNER =====

1. Add Task
2. View Tasks
3. Search Task
4. Mark Completed
5. Delete Task
6. Show Statistics
7. Save Tasks
0. Exit

Enter Choice: 2

===== TASK LIST =====

1. Mathematics Assignment | High | Pending | Deadline: 2026-05-20
2. Physics Reviewer | Medium | Completed | Deadline: 2026-05-25

🚀 How to Compile and Run
Compile the program
g++ smart_study_planner.cpp -o StudyPlanner
Run the executable
StudyPlanner.exe
Using specific C++ standard
g++ -std=c++17 smart_study_planner.cpp -o StudyPlanner

📂 File Handling
The system stores task records inside:
tasks.txt
Each task is separated using delimiters (|) for easier reading and parsing during loading operations.
Example stored format:
Math Assignment|Chapter 5 Exercises|2026-05-20|High|Pending

🎮 Controls
Key	Function
[1]	Add Task
[2]	View Tasks
[3]	Search Task
[4]	Mark Completed
[5]	Delete Task
[6]	Show Statistics
[7]	Save Tasks
[0]	Exit Program

🧪 Algorithms Used
Bubble Sort
Used to automatically organize tasks based on priority level.
Linear Search
Used to search task titles using keyword matching.

🎯 Objectives of the System
To help students organize academic tasks efficiently 
To implement data structures and algorithms in a practical application 
To apply file handling for persistent data storage 
To improve task monitoring through prioritization and completion tracking 
To demonstrate procedural programming concepts in C++
