Download Link: https://assignmentchef.com/product/solved-comp2130-assignment-client-server-spreadsheet-main
<br>
Write a program that provides a simple multi-user networked spreadsheet. The system will be a client server based application using TCP socket connections. The clients should only communicate with the server.

The server should be responsible for executing all the functionalities of the spreadsheet on behalf of the clients.

The program should allow the users to enter numeric values, text, or formulas into any cell at any time. As new data is entered, the spreadsheet should be updated and re-displayed to all clients/users. The program should run until the first user quits. The server should keep track of a count of the number of clients. This  information should also be communicated to all the clients/users upon each re-display.

The maximum size of the spreadsheet should be 9 x 9 cells. Rows should be labeled with numbers, starting from 1, and columns should be labeled with letters, starting from A. Cells should be referenced by a letter number pair, with no space or symbol between; for example, E9. Lowercase and uppercase letters to reference cells are allowed and must be recognized.

The client program cannot prompt what type of entry is being made into a cell. It should prompt only for an input. If the user types data consisting only of numeric values, for example 4.53, then the program must recognize that input as a number. All numbers should be considered real numbers. If the user types input describing a formula (discussed below), then the program must recognize that input as a formula. Everything else defaults to text.

The display of the spreadsheet should be aligned in an easy-to-read 9 x 9 grid. If text entries or other displayed content go beyond the given display size, the display should be truncated.

Formulas are of the form =AVERAGE(A2,A5). This formula would return the average value from the four cells A2, A3, A4, and A5. Three formulas are required: AVERAGE, SUM, and RANGE. RANGE should return the difference between the largest and smallest value in the input. SUM should return the cumulative total. The input must be a horizontal or vertical 1D range of cells, described by the end points. The formula should compute a result using only values within the given range of cells; it should ignore empty cells and those containing text or another formula. If there are no values within the given range of cells, the result should default to zero.

Additionally, you should implement a function in the server to do the following:

(a) Save the current spreadsheet from memory to a location on  the file system running the      server. You can save it in any format. Only the first client should be able to perform this      function.   (function name: <em>saveWorksheet </em>)

Make sure you use appropriate ports. You should ensure that you close your connections cleanly.

<em>Each assignment should clearly contain the ID number and name of each student in the group. </em>

<em>You should work in groups of three (3). </em>

<strong>TIPS</strong>

Make sure you use functions appropriately.

Your code should be properly commented.

Break down the problems into small workable units and create associated functions. Use appropriate collaboration tools eg. GitHub.

Bonus marks will be given for additional useful features.