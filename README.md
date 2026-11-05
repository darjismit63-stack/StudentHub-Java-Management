# ACMS – Advanced College Management System (Java 17)

## Run
1. Extract the ZIP.
2. Open the `ACMS_Advanced_Student_Management` folder in IntelliJ IDEA as a Maven project.
3. Set Project SDK to Java 17 or newer.
4. Open `src/main/java/com/college/Main.java` and Run `Main.main()`.
5. Sign in using the demo credentials shown on the login screen (admin / admin123).

## Main modules
- Student Management: add, update, delete, undo delete, search, department filter, sorting, CSV export, print, topper and performance report.
- Attendance Management: select a student, choose a date, mark Present or Absent, view present/absent days, attendance percentage and date-wise history. Re-marking the same student/date updates that date's status.
- Fees & Payment Management: select a student, set their actual total fee, record one or more instalments with receipt/note, view paid amount, remaining balance, payment status and transaction history. No arbitrary fee is automatically assigned; the administrator must set the fee.
- Academic Operations: faculty, courses, library, timetable and Data Structure Lab.

## Data structures demonstrated
- ArrayList: student and registry collections
- HashMap: fast Student ID lookup and attendance/fee ledgers
- HashSet: unique roll-number validation
- Stack: undo delete
- Queue: admission processing
- Binary Search Tree: student index demonstration
- Trie: prefix search suggestions
- Graph + BFS: course prerequisite traversal
- Priority Queue / Min Heap: library due-date ordering
- Sorting: ID, name and marks ordering; JTable column sorting

## Data storage
Records are saved locally under `acms-data/` in the application's working directory. Keep this folder to retain records between runs. Back it up before moving the project to another computer.

## Important
Attendance and Fee windows use the same shared StudentManager and shared service instances as the main dashboard. Open them using the clearly visible **ATTENDANCE MANAGEMENT** and **FEES & PAYMENT MANAGEMENT** buttons under **COLLEGE MANAGEMENT MODULES**, or from the Modules menu. Add students first; then select a student in the relevant module to record attendance or fees.
