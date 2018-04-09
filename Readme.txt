Repository:
Download solution from following path and extract the zip file. Solution project Zip file is available in GIT Zip file.
https://github.com/udayakumary/MazePath

Environment:
Developed this project using Visual Studio 2017 and .net framework 4.6.1. 
Technologies used for this project are c#, Web API, MVC, HTML, JQuery, CSS

What This Solution Contains?
Solution contains Web API (REST) service and client application (web page) to test rest service. 
Service has one end point “SolveMaze” which accepts maze as input and returns solved maze and number of steps required to move from point A to point B.
Client application has two text box controls one to accept maze input and second to display solved maze. And it also displays number of steps required to move from “A” point to “B”.

How to Run This Application?
Open code in visual studio and Build it. Restore required packages through NuGet(If required) and run the application. 
Service will be self-hosted and client application page (Home page) will be displayed. Enter maze in “Input Maze” textbox and click on “Solve button”. Number of steps and output will be displayed.

To clear fields click on clear button.

Logic Files: 
Rest Service:
MazePath.Business/MazeLogic.cs
MazePath/Controller/MapController.cs

Test Page: 
MazePath/Views/Home/Index.cshtml

Service Endpoint point:
http://localhost:8080/api/Map/SolveMaze

Assumptions:
1.Maze as two dimensional (All lines should be equal length) and surrounded by “#”
2.Line break as new row
3.Contains only “#”, “.”, “A” and “B” characters
4.Only one start and end point
5.Contains at least one valid path
6.Always copy maze from notepad (To aviod extra characters).

Note:
Copy output to notepad to verify solved maze
All validations are not implemented (Few are implemented).
Output "Solution" returned as string. Other option, it can be returned as array of strings (Each row as one array element).
Client page is developed to test the service and logic, not focused on style sheets (As per phone conversation, only solution for problem was requested)
