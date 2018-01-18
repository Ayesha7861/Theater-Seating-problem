# Theater-Seating-problem

***The program is written in Java***

**Program Description**

This program parses a theater layout and a list of ticket requests and produce a list of tickets or explanations in the same order as the requests.
 
few rules to follow 
1.	Fill as many orders as possible
2.	Put parties as close to the front as possible.
3.	If there are not enough seats available in the theater to handle a party, tell them "Sorry, we can't handle your party."
4.	Each party must sit in a single row in a single section.  If they won't fit, tell them "Call to split party".
 
The theater layout is made up of 1 or more rows.  Each row is made up of 1 or more sections separated by a space.

After the theater layout, there is one empty line, followed by 1 or more theater requests.  The theater request is made up of a name followed by a space and the number of requested tickets.

Your program must produce results to standard output in the same order as the requests, with the name of the person who requested the ticket and either the row and section of the ticket or the explanations "Sorry, we can't handle your party" or "Call to split party."

**Execution steps: 

Option 1:


1. Go to File -> Import. ...
2. Select Existing Projects into Workspace.
3. Click on the select root directory and browse the file from drive.
4.Find the archive file on your hard disk.
5. Run build-impl.xml file to generated class files,jar files and help-doc.html file to understand method description.
6.Run TheaterSeat.java file as main programe and give below input.

Option 2:

1. Open command line and iterate through ~/theaterSeat/
2. Type "javac theaterdata\*.java theaterseat\*.java theatersearch\*.java" to compile the program
3. Type "jar cfm theaterseat.jar manifest.txt theaterdata theaterseat theatersearchâ€� to make jar file
3. Type "java -jar theaterseat.jarâ€� to execute the program
4. The program will indicate the path of the output file .
5.Run TheaterSeat.java file as main programe and give below input.


** Sample input&output

Sample input: 
6 6
3 5 5 3
4 6 6 4
2 8 8 2
6 6

Smith 2
Jones 5
Davis 6
Wilson 100
Johnson 3
Williams 4
Brown 8
Miller 12

Sample output:

Smith Row 1 Section 1
Jones Row 1 Section 2
Davis Row 3 Section 2
Wilson Sorry, we can't handle your party
Johnson Row 1 Section 1
Williams Row 2 Section 2
Brown Row 4 Section 2
Miller Call to split party.

Sample Input:

1 2
3 4 5
7 8 1

Ayesha 8
Begum 1
Arsalan 1
Javeed 1
Mummy 3
XXX 100
Begum 1
end


Sample outPut:

Ayesha Row 3 Section 2
Begum Row 1 Section 1
Arsalan Row 1 Section 2
Javeed Row 1 Section 2
Mummy Row 2 Section 1
XXX Sorry, we can't handle your party
Begum Sorry Cannot process Same request


Sample Input:

1 2
3 4 5
7 8 1

Ayesha 1
Ayesha 1
XXXX -1
end

Sample Output:

Ayesha Row 1 Section 1
Ayesha Sorry Cannot process Same request
XXXX Sorry, we can't handle your party.

