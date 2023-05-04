Download Link: https://assignmentchef.com/product/solved-csc60-lab-4-on-file-handling-and-loops
<br>
<strong><u>PROBLEM</u></strong>:

Write a program to compute the perimeter and area of a polygon using an input data file and an output file.  A file <strong>lab4.c</strong> is provided with some of the print statements in it.

<ul>

 <li>It is your responsibility to read the Power Point files:</li>

</ul>

o C-3 Characters ControlStructures.pptx, #20-57 on the various Ifs and Switch o C-4 Loops.pptx, #1-24 o Ask any needed questions in class




To get the files you need, first move to your <strong>csc60</strong> directory:  <strong>cd csc60 </strong>

The following command will create a directory named <strong>lab4</strong> and put all the needed files into it below your csc60 directory.




Type:  <strong>cp -R</strong><strong>  </strong><strong>/gaia/home/faculty/bielr/files_csc60/lab4</strong> <strong><sub>.</sub></strong>

Spaces needed: (1) After the <strong>cp                                                                                  ↑ </strong>space &amp; dot

<ul>

 <li>After the <strong>-R</strong></li>

 <li>After the directory name at the end &amp; before the dot.</li>

</ul>




After the files are in your account and you are still in <strong>csc60</strong>, you need to type: <strong>chmod 755 lab4 </strong>This will give permissions to the directory.

Next move into lab4 directory [<strong>cd lab4</strong>], and type: <strong>chmod  644  lab4*.*</strong> This will give permissions to the files.

Your new lab4 directory should now contain: lab4.c, lab4.dat, lab4sample.dat




<strong><u>INPUT/OUTPUT DESCRIPTION</u></strong>:

<ul>

 <li>The<strong> test data </strong>will be a file called<strong>dat. </strong>Use it to verify the correctness of your program. It has 3 sets of data.</li>

 <li>The<strong> final data</strong> will be a file called <strong>dat</strong>. It has 6 sets of data.</li>

 <li>Each line or record of the file will consist of two numbers: the radius and the number of sides of the polygon.</li>

 <li>Print your name and assignment (use fprintf)</li>

 <li>Use an <em>fscanf</em> statement in a <em>while </em>loop to repeatedly get each set of values. It would be a good idea to make these variable type <em>double</em>.</li>

 <li><strong>The output</strong> will be a file, <strong>out. </strong>The output of the sample data will follow.</li>

</ul>




<strong><u>FORMULAS</u> </strong>

<ul>

 <li>Remember to translate the algebra of the two formulas into the C language.</li>

</ul>

<strong>Perimeter</strong> of the polygon  =  2n R sin <u>PI</u>

n

<strong>             Area</strong> of the polygon = ½ n R<sup>2</sup> sin <u>2 PI</u>

n

<strong><u>DATA FILES</u></strong>:

There are two data files:

<ul>

 <li>dat – Use it to verify the correctness of your program  lab4.dat</li>

</ul>

<strong><u>ALGORITHM DEVELOPMENT</u></strong>:

Open the data file <strong>lab4sample.dat </strong>or<strong> lab4.dat</strong>

Do the appropriate error checking




Open the output file <strong>lab4.out</strong>

Do the appropriate error checking




Print your name and assignment. Then print the column header lines needed. (use fprintf)




while ((fscanf(…, &amp;radius, &amp;nsides)) == 2)

|     Compute the perimeter and area of the polygon.

|_   fprintf the radius, nsides, perimeter, and area as in the Defined Output Appearance.




Close the two files







<strong><u>VIEWING OUTPUT</u> </strong>

When you run the program, the whole thing is going to <strong>lab4.out</strong>. Open that file to see your output. Use either “cat” or “vim”.




<strong><u>REMINDERS</u></strong>:

<ul>

 <li>Include your name and lab4 in your comment block, and in your output.</li>

 <li>All numeric variables are to be type <strong>double</strong>.</li>

 <li>Most of the print and fprintf statements are included in lab4.c for you. You need to write the fprintf in the loop.</li>

 <li>The input file name, which will be changed, ought to be in a #define statement. The file will come with two #define statements, for the test file and the final file. Just move the <strong>//</strong> from in front of one #define statement to the other #define statement.</li>

</ul>

<strong>      #define INFILE lab4sample.dat     </strong>

<strong>      // #define INFILE lab4.dat                                               </strong>

<ul>

 <li>FOR THE VALUE OF PI, use <strong>M_PI</strong> from math.h (which we already have included).</li>

 <li>To compile, you will need to add <strong>–lm </strong>so math.h can be found. Type: <strong>gcc  –lm  c</strong></li>

</ul>




<strong><u>DEFINED OUTPUT APPEARANCE (<em>using lab4sample.out</em>)</u></strong>:




Your Name.  Lab 4.




Number      Perimeter      Area Of

Radius    Of Sides    Of Polygon      Polygon

——–   ——–   ————   ———–

12.60      24.00        78.9422      493.0813

5.60       8.00        34.2884       88.6995

7.85      12.00        48.7615      184.8675




<strong> </strong>

<strong><u>PREPARE YOUR FILE FOR GRADING:</u> </strong>

Make sure your program has been corrected from:

using <strong>lab4sample.dat</strong> to using <strong>lab4.dat</strong>  and has been re-complied.




When all is well and correct,

at the prompt, type:  <strong>script StudentName_lab4.txt       </strong>[Script will keep a log of your session.]

<table width="518">

 <tbody>

  <tr>

   <td width="288">At the prompt, type:  <strong>gcc -lm lab4.c  </strong></td>

   <td width="230">to compile the code</td>

  </tr>

  <tr>

   <td width="288">At the prompt, type:  <strong>a.out</strong></td>

   <td width="230">to run the program</td>

  </tr>

  <tr>

   <td width="288">At the prompt, type:  <strong>cat lab4.out      </strong>After the program run is complete,</td>

   <td width="230">to show contents of the output file</td>

  </tr>

  <tr>

   <td width="288">                            type: <strong>exit</strong></td>

   <td width="230">to leave the script session</td>

  </tr>

 </tbody>

</table>




<strong><u>Turn in your completed session:</u></strong>

Go to Canvas and turn in two files:

<ol>

 <li>c</li>

 <li>txt</li>

</ol>











