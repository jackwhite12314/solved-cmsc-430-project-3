Download Link: https://assignmentchef.com/product/solved-cmsc-430-project-3
<br>
The third project involves modifying the attached interpreter so that it interprets programs for the complete language.

You may convert all values to double values, although you can maintain their individual types if you wish.

When the program is run on the command line, the parameters to the function should be supplied as command line arguments. For example, for the following function header of a program in the file <sub>text.txt</sub>: function main a: integer, b: integer returns integer; One would execute the program as follows:

$ ./compile &lt; test.txt 2 4

In this case, the parameter <sub>a</sub> would be initialized to <sub>2</sub> and the parameter <sub>b</sub> to <sub>4</sub>.

An example of a program execution is shown below:

$ ./compile &lt; test.txt 2 4




<ul>

 <li>function main a: integer, b: integer returns integer;</li>

 <li>c: integer is</li>

 <li>if a &gt; b then</li>

 <li>a rem b;</li>

 <li>else</li>

 <li>a ** 2;</li>

 <li>endif;</li>

 <li>begin</li>

 <li>case a is</li>

 <li>when 1 =&gt; c;</li>

 <li>when 2 =&gt; (a + b / 2 – 4) * 3;</li>

 <li>others =&gt; 4;</li>

 <li>endcase;</li>

 <li>end;</li>

</ul>




Compiled Successfully




Result = 0

After the compilation listing is output, the value of the expression which comprises the body of the function should be displayed as shown above.

The existing code evaluates some of the arithmetic, relational and logical operators together with the reduction statement and integer literals only. You are to add the necessary code to include all of the following:

<ul>

 <li>Real and Boolean literals</li>

 <li>All additional arithmetic operators</li>

 <li>All additional relational and logical operators</li>

 <li>Both <sub>if</sub> and <sub>case</sub> statements</li>

 <li>Functions with multiple variables</li>

 <li>Functions with parameters</li>

</ul>

This project requires modification to the bison input file, so that it defines the additional the necessary computations for the above added features. You will need to add functions to the library of evaluation functions already provided in <sub>values.cc</sub>. You must also make some modifications to the functions already provided.

You are to submit two files.

<ol>

 <li>The first is a <sub>.zip</sub> file that contains all the source code for the project. The <sub>.zip</sub> file should contain the flex input file, which should be a <sub>.l</sub> file, the bison file, which should be a <sub>.y</sub> file, all <sub>.cc</sub> and <sub>.h</sub> files and a <sub>makefile</sub> that builds the project.</li>

 <li>The second is a Word document (PDF or RTF is also acceptable) that contains the documentation for the project, which should include the following:

  <ol>

   <li>A discussion of how you approached the project</li>

   <li>A test plan that includes test cases that you have created indicating what aspects of the program each one is testing and a screen shot of your compiler run on that test case</li>

   <li>A discussion of lessons learned from the project and any improvements that could be made</li>

  </ol></li>

</ol>