Download Link: https://assignmentchef.com/product/solved-csc1251-advanced-programming-assignment-3-c
<br>
<h1>Aim</h1>

The objectives of this assignment includes:

<ul>

 <li>Learning about generic programming templates, operator overloading, ST L (containers &amp; algorithms) and writing io manipulators</li>

 <li>Apply the concepts learnt by developing a data processing program</li>

</ul>

<h1>Backqround</h1>

In this assignment, you are required to develop a program that reads in and process some messy’ records from a file that contains data meant for different kinds of classes. These data are jumbled up and unsorted, and to make it worse, for any particular row of record, there may be multiple duplicates scattered over the entire file!

You program should be called ‘csci251_a3.exe’, and should posses the following capabilities:

<ol>

 <li>read in the records from a user-specified filename</li>

 <li>remove all duplicate rows of data</li>

 <li>filter and display the data according to user-specified sorting criteria</li>

 <li>store the records displayed in c), in a user-specified filename</li>

</ol>

The next section provides information about the requirements for developing this program.

<h1>Task Requirements</h1>

<ol>

 <li>Appendix A provides a sample input data from a file called ‘messy.txt’. It contains information meant to be stored in 4 classes: ‘Point2D’, ‘Point 3D’, ‘Line2D’ and ‘Line3D’. Please refer to the table in Appendix A for a description of the format in which the input data for each of the classes is stored.</li>

 <li>Notel: You are to research and determine which kind of <u>ST L containers</u> (e.g. Map, Vector, Set, Lists etc) you should use, to store all the various objects from the 4 classes. For this assignment you are not allowed to use array [ ] to store any of your data!</li>

 <li>Appendix B provides a description of the 4 classes: ‘Point2D’, ‘Point 3D’, ‘Line2D’ and ‘Line3D’, and the relationships between them. You are to study the diagrams and implement them accordingly.</li>

</ol>

I

<ol>

 <li>Appendix C provides the <u>sample output format</u> and a description of the <u>format requirements</u>, for each of the 4 classes. These format are to be applied whether the data from these classes are output to a file or terminal.</li>

 <li>Note2: To output data, you are required to <u>create vour own output manipulator(s)</u> to display/store data in the format described in Appendix C. You are further required to overload the insertion operator ‘&lt;&lt;‘, for each of the 4 classes, to support the process of inserting data to the terminal, or the relevant file stream. (Hint : Research on the concept of writing output manipulators. E.g. <u>https://en.cppreference.com/w/cpp/io/manip/left</u> )</li>

 <li>Note3: All output data must not contain any duplicates! There are many approaches to solving this problem. Firstly, you could check for, and remove duplicate records at the point of reading in the input. Alternatively, you could temporarily store the data in a ST L container, research and make use of any <u>ST L alqorithm</u> to search for, and remove the duplicates. Another (inefficient) way is to store everything in ST L container, but your program needs to ensure that when user wishes to see / store the records in a file, no duplicate records are shown.</li>

 <li>Appendix D provides a description of a few generic template functions that you are supposed to develop. These ‘utility’ functions plays a supporting role, and they should be developed in a separate header file called ‘My Templates.h’</li>

 <li>Your program should allow user specify the filtering criteria so that user can specify which set of records he wishes to view / store. Your program should allow the following options:</li>

</ol>

Point2D records     &lt;= default selected option

Point3D records

Line2D records iv)           Line3D records

<ol>

 <li>l) Your program should allow user to specify the sorting criteria so that user can specify which attributes (of a set of records) to order the data by. The sorting criteria is based on the current filtering criteria.</li>

</ol>

For example, if the current filtering criteria is ‘Only Point2D records’, your program should restrict user to the options of sorting the data by ‘x’, ‘y’ &amp; scalar value ‘distFrOrigin’ only!

Please refer to Appendix E for a detailed description of the combinations of filtering criteria, and the respective (allowable) sorting criteria.

<ol>

 <li>Hint: It is not necessary to develop your own sorting algorithm, or make use of any of the classical algorithms like ‘Quick-Sod, ‘Bubble-Sod to fulfill the sorting requirements.</li>

</ol>

There is a function defined in ST L algorithm (i.e. #include &lt;algorithm&gt;) called ‘sort’. You should research on its usage, code the necessary <u>comparator functions</u> (for each of the 4 classes + sorting criteria). Once you mastered its usage, you will easily achieve the desired sorting effect using less than 3 lines of code!

<ol>

 <li>To assist you in visualizing the desired program interactions, please refer to Appendix F which provides a sample menu displaying the output data / messages in response to user input.</li>

 <li>Once the program is completed and tested to be vorking successfully, you are highly encouraged to add on “new features” to the program that you feel are relevant to the problem. Additional marks may be awarded subject to the relevancy and correctness of the new functionalities.</li>

 <li>You are to use only C++ language to develop your program. There is no restriction on the IDE as long as your source files can be compiled by g++ compiler (that comes packaged in Ubuntu linux) and executed in the Ubuntu terminal shell environment.</li>

</ol>

<h1>Deliverables</h1>

The deliverables include the following:

<ol>

 <li>The actual working C++ program (soft copy), <u>with comments on each file </u><u>function or block of code</u> to help the tutor understand its purpose.</li>

 <li>A softcopy word document that elaborates on:

  <ul>

   <li>(Interpreted) requirements of the program</li>

   <li>Diagram / Illustrations of program design</li>

   <li>Summary of implementation of each module in your program</li>

   <li>Reflections on program development (e.g. assumptions made, difficulties faced, what could have been done better, possible enhancements in future, what have you learnt, etc)</li>

  </ul></li>

 <li>A program demo/software testing during lab session. You must be prepared to perform certain tasks / answer any questions posed by the tutor.</li>

</ol>

<ul>

 <li>IMPT: Please follow closely, to the submission instructions in Appendix G, which contains details about what to submit, file naming conventions, when to submit, where to submit, etc.</li>

 <li>The software demo / testing will be held during lab session where you are supposed to submit your assignment. Some time will be allocated for you to present / demonstrate your program’s capabilities during the session.</li>

</ul>

<h1>Gradinq</h1>

Student’s deliverable will be graded according to the following criteria:

Program fulfills all the basic requirements stipulated by the assignment

Successful demonstration of a working program, clarity of explanation / presentation and satisfactory answers provided during Q &amp; A session.

(iii)      Additional effort (e.g. enhancing the program with <u>relevant</u> features over and above task requirements, impressive, ‘killer’ presentation)

After the submission of deliverables, students will be required undergo a software testing process (to determine the correctness and fulfillment of software requirements.) Further instructions will be given by the Tutor during the subsequent respective labs. Please pay attention as failure to adhere to instructions Will result in deduction of marks.

Tutor’s note:

In the real working world, satisfactory completion of your tasks is no longer enough. The capability, efficiency and robustness of your system to operate under different testing conditions, and the ability to <u>add value</u> <u>communicate</u> and/or <u>demonstrate</u> your ideas with clarity is just as important as correct functioning of your program. The grading criteria is set to imitate such requirements on a ‘smaller scale’.

<h1>APPENDIX A</h1>

(Sample ‘messy’ data from an input file)

<table width="646">

 <tbody>

  <tr>

   <td width="646">Point2D, [3, 21Line3D, [7, 12, 31, [-9, 13, 681 Point3D, [1, 3, 81Line2D, [5, 71, [3, 81 Point2D, [3, 21Line3D, [7, -12, 31, [9, 13, 681Point3D, [6, 9 51Point2D, [3, 21Line3D, [70, -120, -31, [-29, 1, 2681Line3D, [25, -69, -331, [-2, -41, 581Point3D, [6, 9, -501</td>

  </tr>

 </tbody>

</table>

Note:

<ul>

 <li>Some data, (e.g. ‘Point2D, [3, 2] can be repeated multiple times (i.e. they are duplicated data), this applies to all other kinds of data as well.</li>

 <li>In each line, the <u>1 <sup>st </sup>field</u> WII contain the class’s name (e.g. ‘point2D’, ‘Point3D’,</li>

</ul>

‘Line2D’ and ‘Line3D’)

<ul>

 <li>The delimiter separating the <u>1 <sup>st </sup>field</u> from the rest of the data, is a comma, followed by a space char (i.e.</li>

 <li>The delimiter separating each number in the 2D/3D coordinate, is also a comma, followed by a space char (i.e. ‘)</li>

 <li>Each 2D/3D point’s data, is enclosed by the square brackets ‘[‘ and ‘]’</li>

 <li>Each Line2D / Line3D’s data consists of buo points, each enclosed by square brackets, and the delimiter separating each point is also a comma, followed by a space char (i.e.</li>

 <li>You may assume that the <u>ranqe of each number</u> in the x, y or z coordinate can be anything from -999 to 999</li>

</ul>




B

(The 4 classes, and their relationships)

<table width="657">

 <tbody>

  <tr>

   <td width="221">Point2D</td>

   <td colspan="3" rowspan="2" width="173"></td>

   <td width="263">Line2D</td>

   <td width="0"></td>

  </tr>

  <tr>

   <td rowspan="2" width="221"># x: int# y: int# distFrOrigin: double</td>

   <td rowspan="2" width="263">–                     ptl: Point2D–                     pt2: Point2D # length: double</td>

   <td width="0"></td>

  </tr>

  <tr>

   <td colspan="3" rowspan="2" width="173"></td>

  </tr>

  <tr>

   <td width="221"># setDistFrOrigin ()+ Point2D (x: int, y: int)+ getX () : int+ getY () : int+ getScaIarVaIue () : double+ setX (x: int)+ setY (y: int)</td>

   <td width="263"># setLength ()+ Line2D (ptl : Point2D, pt2: Point2D)+ getPt1 : Point2D+ getPt2 : Point2D+ getScaIarVaIue () : double+ setPt1 (ptl: Point2D)+ setPt2 (pt2: Point2D)</td>

   <td width="0"></td>

  </tr>

  <tr>

   <td colspan="2" rowspan="2" width="291">


    <table width="221">

     <tbody>

      <tr>

       <td width="110"></td>

       <td width="110"></td>

       <td width="0"></td>

      </tr>

      <tr>

       <td colspan="2" width="221">Point3D</td>

       <td width="0"></td>

      </tr>

      <tr>

       <td colspan="2" rowspan="2" width="221"># z: int</td>

       <td width="0"></td>

      </tr>

      <tr>

       <td colspan="2" width="221"># setDistFrOrigin ()+ Point3D (x: int, y: int, z: int)+ getZ () : int+ setZ (z: int)</td>

       <td width="0"></td>

      </tr>

     </tbody>

    </table></td>

   <td rowspan="2" width="101"></td>

   <td colspan="2" width="265"></td>

   <td width="0"></td>

  </tr>

  <tr>

   <td colspan="2" width="265">


    <table width="262">

     <tbody>

      <tr>

       <td width="262">Line3D</td>

      </tr>

      <tr>

       <td width="262">– PM: Point3D– pt2: Point3D</td>

      </tr>

      <tr>

       <td width="262"># setLength ()+ Line3D (pti: Point3D, pt2: Point3D)+ getPt1 : Point3D+ getPt2 : Point3D+ setPt1 (pti: Point3D)+ setPt2 (pt2: Point3D)</td>

      </tr>

     </tbody>

    </table></td>

   <td width="0"></td>

  </tr>

  <tr>

   <td width="206"></td>

   <td width="15"></td>

   <td width="99"></td>

   <td width="4"></td>

   <td width="716"></td>

   <td width="0"></td>

  </tr>

 </tbody>

</table>

<h1>APPENDIX B (con’t)</h1>

Note:

<ol>

 <li>I) The above diagrams depict the <u>bare minimum requirements</u> for the 4 classes whose attributes and methods you MUST implement</li>

</ol>

<ul>

 <li>In Point2D class, setDistFrOrigin ( ) method computes the <u>distance</u> of the point to the origin (O, O), and initializes the attribute distFrOrigin with this <u>distance value</u>. The formula to compute is as follows:</li>

</ul>

distFrOrigin = (x — O) <sup>2 </sup>+ (y — O) <sup>2 </sup>OR distFrOrigin = <sup>A</sup>l x<sup>2 </sup>+ Y<sup>2</sup>

Note : means square root

<ul>

 <li>In Point2D class, getScaIarVaIue ( ) method is merely an accessor method that returns the value of attribute distFrOrigin.</li>

 <li>In Line2D class, setLength ( ) method computes the <u>distance</u> between its own Point2D attributes ptl and pt2, and initializes the attribute Length with this <u>distance value</u>. The formula to compute is as follows:</li>

</ul>

length = <sup>A</sup>l (ptl,x — pt2.x) <sup>2 </sup>+ (ptl,y —

<ul>

 <li>In Line2D class, getScaIarVaIue ( ) method is merely an accessor method that returns the value of attribute length.</li>

 <li>In Line3D class, set Length ( ) method computes the <u>distance</u> betoeen its own Point 3D attributes ptl and pt2, and initializes the attribute Length with this <u>distance value</u>. The formula to compute is as follows:</li>

</ul>

length                                   (ptl . x pt2.x) <sup>2 </sup>+ (ptl . y pt2.y) <sup>2 </sup>+ (ptl.z                              pt2.z) 2

<ul>

 <li>For all the 4 classes, you are free to declare and implement any additional attributes and methods like:

  <ul>

   <li>Overloading io-stream, arithmetic, comparison or any other operators ‘&lt;&lt;‘,</li>

   <li>Writing static comparator functions to use in STL algorithms and containers,</li>

   <li>Writing io manipulators specific to a particular class</li>

   <li>Writing any other supporting helper functions necessary to fulfill the requirements of this assignment.</li>

  </ul></li>

</ul>

C

(General Output Format for Point2D &amp; Point 3D data)

<table width="398">

 <tbody>

  <tr>

   <td width="78"></td>

   <td width="58"></td>

   <td width="262">Point2D</td>

  </tr>

  <tr>

   <td width="78">x[—999,3,23,123,</td>

   <td width="58">Y-9]-99]-999]3]23]123]</td>

   <td width="262">Dist. Fr Origin12 . 728140 . 0071412 . 79932 . 527173 . 948</td>

  </tr>

  <tr>

   <td width="78"></td>

   <td width="58"></td>

   <td width="262">Point3D</td>

  </tr>

  <tr>

   <td width="78">x[-999,3,23,123,</td>

   <td width="58">Y-9,-99,-999,3,23,123,</td>

   <td width="262">       z                Dist. Fr Origin-9]     15 . 589-99]       171 .473-999]      1730 .3203]     5 . 19623]     39 . 837123]       213 . 042</td>

  </tr>

 </tbody>

</table>

Note:

The allocated width to store each x, y and/or z ordinate value is 4 ‘spaces’, inclusive of mnus Sign

<ul>

 <li>All x, y, z values are strictly whole numbers (i.e. integers) and all Dist. Fr Origin values are strictly decimal (i.e. double), with precision set at up to 3 decimal places</li>

 <li>The 1 &lt; 2 lines (representing the ‘header’) is compulsory. The alignment of the ‘X’, ‘Y’ or ‘Z’ column names in the header is vertically aligned to its respective last digit’s position!</li>

 <li>The should be 3 ‘spaces’ between the end of each point’s data values, and its corresponding Dist. Fr Origin values</li>

</ul>




<h1>APPENDIX C (con’t)</h1>

(General Output Format for Line2D &amp; Line3D data)

<table width="611">

 <tbody>

  <tr>

   <td width="78"></td>

   <td width="58"></td>

   <td colspan="2" width="86"></td>

   <td width="57"></td>

   <td colspan="3" width="331">Line2D</td>

  </tr>

  <tr>

   <td width="78">PI-X[—999,3,999,[-999,</td>

   <td width="58">PI-Y-9]-99]-999]3]999]-999]</td>

   <td colspan="2" width="86">P2-X[-999,999 ,[-999,3,</td>

   <td width="57">P2-Y-99]-999]-9]999]-999]3]</td>

   <td colspan="3" width="331">Length127 . 2791272 . 79214 00 . 07114 08 . 5572825 . 5991417 . 042</td>

  </tr>

  <tr>

   <td width="78"></td>

   <td colspan="2" width="115"></td>

   <td colspan="4" width="221">Line3D</td>

   <td width="196"></td>

  </tr>

  <tr>

   <td width="78">Pl-x[-999,3,999,-999,</td>

   <td colspan="2" width="115">PI-Y Pl-z-9,     -9]-99,     -99]-999, -999]3,       3]999,      999]-999, -999]</td>

   <td colspan="3" width="145">P2-x P2-Y-99,    -99,[-999, -999,—9,        —9,999,    999,[-999, -999,3,       3,</td>

   <td width="76">P2-z-99]-999]_9]999]-999]3]</td>

   <td width="196">Length155 . 8851558 . 8461714 . 7301275 . 1233460 . 6381735 .515</td>

  </tr>

  <tr>

   <td width="78"></td>

   <td width="58"></td>

   <td width="58"></td>

   <td width="29"></td>

   <td width="57"></td>

   <td width="59"></td>

   <td width="76"></td>

   <td width="196"></td>

  </tr>

 </tbody>

</table>

Note:

<ul>

 <li>In Line2D, the formatting for data under ‘PI-X’, ‘PI—Y’, ‘p 2-X’ and ‘P2—Y’ headings is similar to that for Point2D. The corresponding formatting applies for the case of Line3D which is similar to that specified for Point3D.</li>

 <li>The 1 <sup>st </sup>2 lines (representing the ‘header’) is compulsory. The alignment of the ‘PI-X’, ‘PI-Y’, ‘PI-Z’, ‘P2-x’, ‘P2-Y’ and ‘P2—Z’ column names in the header is vertically aligned to its respective last digit’s position!</li>

 <li>The should be 3 ‘spaces’ between the end of each point’s data values, and its corresponding Length values</li>

</ul>

<h2>IO</h2>

D

(Description of Generic Function Template)

<table width="707">

 <tbody>

  <tr>

   <td width="95">Template function</td>

   <td width="195">Parameter description</td>

   <td width="140">If param(s) is of the followingClass / Type</td>

   <td colspan="3" width="278">“Meaning” of the template function when applied to (param’s) Class /Type</td>

  </tr>

  <tr>

   <td rowspan="4" width="95">Name : scalar differenceReturn Type :double</td>

   <td rowspan="4" width="195">No. of parameters : 2Type of          parameter :Type of 2<sup>nd </sup>parameter :</td>

   <td width="140">Point2D</td>

   <td rowspan="4" width="118">The absolute scalar values and 2.(Hint: make use getScaIarVaIue() Appendix B!)</td>

   <td colspan="2" rowspan="4" width="159">value difference in the betw. parameters Iof the method mentioned in</td>

  </tr>

  <tr>

   <td width="140">Point3D</td>

  </tr>

  <tr>

   <td width="140">Line2D</td>

  </tr>

  <tr>

   <td width="140">Line3D</td>

  </tr>

  <tr>

   <td width="95"></td>

   <td width="195"></td>

   <td width="140"></td>

   <td width="118"></td>

   <td colspan="2" width="159"></td>

  </tr>

  <tr>

   <td rowspan="5" width="95">equalsReturn Type :‘bool’</td>

   <td rowspan="5" width="195">No. of parameters : 2Type of 1st parameter :Type of 2nd parameter :</td>

   <td width="140">Numeric primitives (int, double, etc)</td>

   <td width="118">parameter I</td>

   <td colspan="2" width="159">parameter 2</td>

  </tr>

  <tr>

   <td width="140">Point2D</td>

   <td width="118">param I ‘s x param I ‘s y</td>

   <td width="105">param 2′ s x param 2’s y</td>

   <td width="54">AND</td>

  </tr>

  <tr>

   <td width="140">Point3D</td>

   <td width="118">param I ‘s x param I ‘s y param I’s z -z</td>

   <td width="105">param 2’s x param 2’s y param 2’s z</td>

   <td width="54">ANDAND</td>

  </tr>

  <tr>

   <td width="140">Line2D</td>

   <td colspan="3" rowspan="2" width="278">param I ‘s ptl           param 2’s ptl AND param I ‘s pt2 -z param 2’s pt2</td>

  </tr>

  <tr>

   <td width="140">Line3D</td>

  </tr>

  <tr>

   <td width="95"></td>

   <td width="195"></td>

   <td width="140"></td>

   <td colspan="3" width="278"></td>

  </tr>

 </tbody>

</table>

Note:

<ul>

 <li>Based on the information provided in the table, you will need to overload the relevant operators in the affected classes, in order to implement the ‘meaning’ correctly, when the generic function’s algo is applied on the 4 classes</li>

 <li>The above generic function templates should be implemented in a header file called ‘My Templates . h’.</li>

</ul>

<u>E</u>

(Combinations of filtering + sorting criteria)

<table width="696">

 <tbody>

  <tr>

   <td width="155">Filtering Criteria</td>

   <td width="79"></td>

   <td colspan="3" width="462">Sorting Criteria (allow sorting by … )</td>

  </tr>

  <tr>

   <td width="155">Point2D records</td>

   <td width="79">iii)</td>

   <td width="170">X  ordinate valueY  ordinate valueDist. Fr Origin value</td>

   <td width="96">(default)</td>

   <td width="196"></td>

  </tr>

  <tr>

   <td width="155">Point3D records</td>

   <td width="79">iii) iv)</td>

   <td width="170">X  ordinate valueY  ordinate valueZ  ordinate valueDist. Fr Origin value</td>

   <td width="96">(default)</td>

   <td width="196"></td>

  </tr>

  <tr>

   <td width="155">Line2D records</td>

   <td rowspan="2" width="79"></td>

   <td colspan="2" rowspan="2" width="266">X and Y coordinate values of Pt. 1X and Y coordinate values of Pt. 2Length value</td>

   <td rowspan="2" width="196">(default)</td>

  </tr>

  <tr>

   <td width="155">Line3D records</td>

  </tr>

 </tbody>

</table>

Note:

<ol>

 <li>l) Sorting by X and Y coordinates is done, by first ordering all rows according to x-ordinate value, this will have a ‘sorting and bunching’ effect that groups rows with the same xordinate values together, if it exists.</li>

</ol>

Within each ‘group’ with similar x-ordinate values, the sorting order (assuming it is ascending), is then applied to the y-ordinate, such that rovvs with the same X, but smaller Y value will be ‘above’ those with same X, but bigger Y values.

<ul>

 <li>For all sorting criteria, you should allow sorting in both ASCENDING and DESCENDING order! (Assume default is ‘ASC’).</li>

 <li>If you are using ST L containers / algorithms to handle the storage of your objects and sorting, you need to implement the relevant function comparators for each of the 4 classes. These function comparators should ideally be implemented as static boolean functions under each of the 4 classes.</li>

</ul>

<u>F</u>

(Sample Menu Interactions)

<table width="375">

 <tbody>

  <tr>

   <td rowspan="3" width="375">Student ID      : 1234567Student Name : Tan Ah Meng ElvisWelcome to Assn3 program!1)                  Read in data2)                  Specify filtering criteria (current : Point2D)3)                  Specify sorting crieria (current : x-otdinate)4)                  Specify sorting order (current : ASC)5)                  View data6)                  Store dataPlease enter your choice : IPlease enter filename : messy.txt13 records read in successMIy!Going back to main menu .</td>

   <td width="0"></td>

  </tr>

 </tbody>

</table>

The figure on the left describes a sample interaction for specifying input filename to <u>read in data</u>.

The program should acknowledge by indicating the no. of records read in successfully!

<table width="377">

 <tbody>

  <tr>

   <td width="377">Student ID    : 1234567Student Nane : Tan Ah Meng ElvisWelcome to Assn3 program!1)                  Read in data2)                  Specify filtering criteria (curren : PoiN2D)3)                  Specify sorting crteria (curren : x-ordinate)4)                  Specify sorting order (cument : ASC)5)                  View data6)                  Store dataPlease enter your choice : 2[ Specifying fiftering ctiteria (currenta)                    Point2D recordsb)                   Point3D recordsc)                    Line2D recordsd)                   Line3D recordsAease enter your crtetia (a — d) : dFifer crieria successfully set to ‘Line3D’!1)                  Read in data2)                  Specify filtering criteria (current : Line3D)3)                  Specify sotting crieria (curren : Pt. 1)4)                  Specify sotting order (cument : ASC)5)</td>

  </tr>

 </tbody>

</table>

The figure on the right describes a sample interaction for specifying <u>filterinq criteria</u> to indicate which type of records user wish to see.

Notel: Observe that the current filtering criteria has changed in option 2) of the man menu, once it has been

Note2: Observe that the current sorting criteria is automatically changed to the <u>default</u> for Line3D records, which is sorting by Pt I’s (x, y) coordinates (refer to Appendix E for details)




<u>APPENDIX F (con’t)</u>

(Sample Menu Interactions)

<table width="375">

 <tbody>

  <tr>

   <td width="375">1)                  Read in data2)                  Specify filtering criteria (current : Line3D)3)                  Specify sorting crieria (current : Pt. 1)4)                  Specify sorting order (current : ASC)5)                  View data6)                  Store dataPlease enter your choice : 3[ Specffying sating crieria (current : Pt. 1)]a)                  R. I’s (x, y) valuesb)                  R. 2’s (x, y) valuesc)                  Length valuePlease enter your crietia (a — c) : cSorting criteria successfully set to ‘Length’!1)                  Read in data2)                  Specify filtering criteria (curren : Line3D)3)                  Specify sorting crteria (curren : Length)4)                  Specify sorting order (current : ASC) 5)</td>

  </tr>

 </tbody>

</table>

The figure on the right describes a sample interaction for specifying <u>sortinq criteria</u> to indicate which attribute, of the selected type of records user wish to see.

Note3: Observe that the sub-menu display options which are relevant to currently selected filter, which is ‘Line3D’! (refer to Appendix E for details)

Note4: Observe that the current sorting criteria has changed in option 3) of the main menu, once it has been successfully set to ‘Length’.

<table width="375">

 <tbody>

  <tr>

   <td width="375">1)                   Read in data2)                   Specify fitering criteria (curren : Line3D)3)                   Specify sating crieria (cument : Pt. I)4)                   Specify sating order (current : ASC)5)                   View data6)                   Store dataPlease enter your choice : 4[ Specifying sating order (current : ASC) Ja)                  ASC (Ascending order)b)                  DSC (Descending order)Please enter yourcrteria (a — b) : bSating order successfully set to ‘DSC’!1)                  Read in data2)                  Specffy fitering criteria (curren : Line3D)3)                  Specfy sating crteria (cument : Len$h)4)                  Specfy sating order (current : DSC) 5)</td>

  </tr>

 </tbody>

</table>

The figure on the right describes a sample interaction for specifying <u>sortinq order</u> to indicate whether records are to be displayed / output in Ascending or Descending order.

Note5: Observe that the current sorting order has changed in option 4) of the main menu, once it has been successfully set to ‘DSC’

<u>APPENDIX F (con ‘t)</u>

(Sample Menu Interactions)

The figure on the right describes a sample interaction to <u>displav data</u>.

Note6: Observe that all the latest criteria specified in main menu options 2) — 4) are re-iterated before the rows of Line3D records are displayed.

<table width="469">

 <tbody>

  <tr>

   <td colspan="3" width="469">1)                  Read in data2)                  Specify filtering criteria (current : Line3D)3)                  Specify sorting crieria (current : Len$h)4)                  Specify sorting order (current : DSC)5)                  View data6)                  Store dataPlease enter your choice : 5[ View data J fifering crieria : Line3D sorting criteria : Length sorting order : DSCPI -x PI-Y                                                P2-x P2-Y P2-z                    Length999,     999,     999]          [-999, -999, _ 999]         3460. 638999 -999, _999]                 3,         3,         3]      1735 . 5159 99 _999] —9, 1714. 730 [ -99, _ 99, -99] [-999, -999, _ 999] 155B.3, 3,         3]        [ 999,  999,    999]    1275 .123      [ -99,        155 . 885Press any key to go back to main menu .</td>

  </tr>

  <tr>

   <td width="320"></td>

   <td colspan="2" width="148"></td>

  </tr>

  <tr>

   <td colspan="2" width="355">1)                   Read in data2)                   Specify filtering crfteria (curren : Line3D)3)                   Specify sorting crteria (current : Len#)4)                   Specify sorting order (current : DSC)5)                   View data6)                   Store dataPlease emeryour choice : 6Please enerfilename : Line3D.txt13 records output successfully!Going back to main menu</td>

   <td width="114">The figure on interaction toNote7: The the data in should be user choose refer to output</td>

  </tr>

  <tr>

   <td width="320"></td>

   <td width="35"></td>

   <td width="114"></td>

  </tr>

 </tbody>

</table>

the right describes a sample <u>write data to an output file</u>.

contents and its formatting of the output file ‘Line3D txt’ similar to that displayed when main menu option 5! (please of the figure above)

<h1>APPENDIX G</h1>

Submission Instructions (V. IMP T!!)

<ul>

 <li>Deliverables

  <ol>

   <li>All submissions should be in softcopy, unless otherwise instructed</li>

   <li>For the actual files to be submitted, you typically need to include the followng:

    <ul>

     <li>word document report (e.g. *.doc), save as <u>MS Word 97-2003</u> format the source file(s), (e.g. *.h, *.0, or *.cpp files)</li>

     <li>the executable file, (using Ubuntu g++ compiler), compile into an executable filename with *.exe (e.g. csci251_a3.exe)</li>

    </ul></li>

  </ol></li>

</ul>

<ul>

 <li>How to package</li>

</ul>

Compress all your assignment files into a <u>sinqle zip file</u>. Please use the following naming format

&lt;FT/PT&gt;_&lt;Your Grp&gt;_Assn3_&lt;Stud. No.&gt;_&lt;Name&gt;.zip

Example .

&lt;FTIPT&gt; Use “F T” for Full-Time student, “P T” if you are Part-Time student

&lt;Your Grp&gt; refers to your SIM tutorial group (e.g. TutGrp1 / TutGrp2 / TutGrp / etc.)

Assn3 if you are submitting assignment 3, Assnl if submitting assignment 1 etc.

&lt;Stud. No.&gt; refers to your LJOW student number (e.g. 1234567)

&lt;Name&gt; refers to your IJOW registered name (e.g. JohnDoeAnderson)

<ul>

 <li>Where to submit</li>

</ul>

Please submit your assignment via Moodle el-earning site.

IMPORTANT NOTE :

<ul>

 <li>To minimize the chances of encountering UNFORSEEN SITUATIONS (mentioned below), please do an <u>EARLY SUBMISSION</u> via Moodle.</li>

 <li>Prior to the relevant assignment deadline, you can upload (and replace) your assignment submissions in Moodle as many times as you like</li>

 <li>It is <u>vour responsibilitv</u> to confirm that you have submitted the final (and correct version) of your deliverables to Moodle <u>before deadline</u></li>

 <li>Any submission uploaded to Moodle after deadline will be considered late</li>

</ul>

In the event of UNFORSEEN SITUATIONS :

( E.g. 3 hrs prior to deadline, there is proof of unforseen events like Moodle site down, unable to upload assignment, undersea internet cable damaged by sea urchins, etc )

Please email your single zip file to your tutor at

<u><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="abc8d8c8c2999e9aebd2cac3c4c485c8c4c6">[email protected]</a></u> for FULL TIME students <u><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="0e6d7d6d673c3b3f4e786f666161206d6163">[email protected]</a></u> for PART TIME students

In your email subject line, type in the following information

&lt;FTIPT&gt; &lt;Your Grp&gt; &lt;assignment inf0&gt; &lt;student number&gt; and Fname&gt;




Example:

To                              tutor’,s email (s+e above)

<table width="632">

 <tbody>

  <tr>

   <td width="95">SubjectNote 1 :Note 2 :</td>

   <td width="537">           FT TutGrp3 Assn3 1234567 JohnDoeAndersonThe timestamp shown on tutor’s email Inbox will be used to determine if the assignment is late or not.After email submission, your mailbox’s s<u>ent f</u>older would have a copy (record) of your sent email, please <u>do not delete</u> that copy It could be used to prove your timely submission, in case the Tutor did not receive your email!</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>When to submit</li>

</ul>

<ol>

 <li>a) Depending on the time-table, a <u>software demo / testinq / presentation</u> for your assignment will be scheduled during the:

  <ul>

   <li>3<sup>rd </sup>– 5<sup>th </sup>lab session for the semester (i.e. lab 3 – 5), for Full Time (F T) students</li>

   <li>2<sup>nd </sup>– 4<sup>t1 </sup>lab session for the semester (i.e. lab 2 – 4), for Part Time (PT) students</li>

  </ul></li>

</ol>

Please consult your tutor for further details. Some time will be allocated for students to demo / present / explain your system design or run test cases during the session.

<ol>

 <li>Please refer to the following table on the different deliverables, submission events &amp; deadlines</li>

</ol>

<table width="654">

 <tbody>

  <tr>

   <td rowspan="2" width="94">Assignment</td>

   <td colspan="2" width="198">Submission Deadline (check Moodle forEXACT date-time )</td>

   <td rowspan="2" width="162">Software Demo / Testing (Tasks), during …</td>

   <td rowspan="2" width="200">Email Demo I Software Testing result files by :</td>

  </tr>

  <tr>

   <td width="102"></td>

   <td width="96"></td>

  </tr>

  <tr>

   <td width="94">1</td>

   <td width="102">Lab 2</td>

   <td width="96">Lab 3</td>

   <td width="162">Lab 2(PT), Lab 3(FT)</td>

   <td width="200">End of Lab 2(PT), Lab 3(FT)</td>

  </tr>

  <tr>

   <td width="94">2</td>

   <td width="102">Lab 3</td>

   <td width="96"></td>

   <td width="162">Lab 3(PT), Lab 4(FT)</td>

   <td width="200">End of Lab 3(PT), Lab 4(FT)</td>

  </tr>

  <tr>

   <td width="94">3</td>

   <td width="102"></td>

   <td width="96">Lab 5</td>

   <td width="162">Lab 4(PT), Lab 5(FT)</td>

   <td width="200">End of Lab 4(PT), Lab 5(FT)</td>

  </tr>

 </tbody>

</table>

<ol>

 <li>IMPORTANT NOTE : Non-submission of any of the above mentioned deliverables will result in ZERO marks! Please check with your Tutor personally if you are unsure!</li>

</ol>

<ul>

 <li>Please help by paying attention to the following …</li>

</ul>

! VERY IMPORTANT !

PLEASE FOLLOW ALL THE GUIDELINES / REQUIREMENTS IN ALL ASSIGNMENT APPENDICES

PLEASE FOLLOW ALL THE SUBMISSION INSTRUCTIONS FROM 1 TO 4 Il

IF YOU ARE NOT SURE,

PLEASE CHECK WITH YOUR TUTOR DURING LABS / LECTURES !

OR

PLEASE EMAIL YOUR ENQUIRIES TO YOUR TUTOR !

MARKS <u>WILL BE DEDUCTED</u> IF YOU FAIL TO FOLLOW INSTRUCTIONS

Examples of marks deduction

<ul>

 <li>Your deliverables / zip file does not follow naming convention</li>

 <li>You have no email subject/ or do not following naming convention</li>

 <li>Your email address / content does not include your name/identity (i.e. tutor cannot easily identify sender)</li>

 <li>Wrong naming or misleading information given</li>

</ul>

(e.g. putting “Assn2” in email subject, when you are submitting “Assnl “)

(e.g. naming “Assnl ” in your zip file, but inside contains Assn2 files )

<ul>

 <li>You email to the WRONG tutor</li>

 <li>Your submission cannot be downloaded and unzipped</li>

 <li>Your program cannot be re-compiled and/or executable file cannot run</li>

 <li>Your report / testing files cannot be opened by Microsoft Word / Excel 2003</li>

 <li>You did not submit / incomplete submission of software demo / testing files etc</li>

</ul>

6) Re-submission administration

After the deadline, (on case-by-case basis), some students / grp may be granted an opportunity for an un-official resubmission by the tutor. If this is so, please adhere to the following instructions carefully:

&lt;Step 1&gt;    Prepare 2 zip files as follows

Zip up for re-submission, <u>proqram files</u> according to the following format

Resubm it &lt;FT/PT&gt;&gt;_&lt;Your Grp&gt;_Assn3_&lt;Stud. No.&gt; _&lt;Name&gt;.zip

Example : Resubmit FT_TutGrp3_ Assn3=1234567_JohnDoeAnderson. zip

Zip up for re-submission, <u>test case results</u> files according to the following format

Resubm it &lt;FT/PT&gt;_&lt;Your Grp&gt;_Assn3_TCResults_&lt;Stud. No.&gt; _&lt;Name&gt;.zip

Example : Resubmit_FT_TutGrp3_Assn3_TCResults_1234567_JohnDoeAnderson. zip

<ul>

 <li>&lt;FTIPT&gt; Use “FT” for Full-Time student, “PT” if you are Part-Time student</li>

 <li>&lt;Your Grp&gt; refers to your SIM tutorial group (e.g. TutGrp1 / TutGrp2 / TutGrp / etc.)</li>

 <li>Assn3 if you are submitting assignment 3, Assn2 if submitting assignment 2 etc.</li>

 <li>&lt;Stud. No.&gt; refers to your I-JOW student number (e.g. 1234567)</li>

</ul>

&lt;Name&gt; refers to your I-JOW registered name (e.g. JohnDoeAnderson)

<ol>

 <li>IMPT To prevent Tutor’s Inbox from blowing up in his face, each student is <u>only allowed to re-submit ONCE</u>, for each assignment only!</li>

</ol>

&lt;Step 2&gt;

Please email your 2 zip files to your tutor’s email (refer to section 3) – Where to submit)

In your email subject line, type in the following information

Resubm it &lt;FTIPT&gt; &lt;Your Grp&gt; &lt;assignment inf0&gt; &lt;student number&gt; and &lt;name&gt;

Example:

To                            tutor’s &amp;Qail befer to s&amp;tion 3) – UKere to sugrnit)

Subject              Resubmit FT TutGrp3 Assn3 1234567 JohnDoeAnderson

IMPORTANT NOTE

Non-submission of any of the above mentioned files, or failure to adhere to submission instructions will result in ZERO marks!

Please check with your Tutor personally if you are unsure!