Download Link: https://assignmentchef.com/product/solved-csc349-project-2-part-2-matrix-multiplication-algorithms
<br>
<strong>Goals of the assignment: </strong>

<ol>

 <li>Implement divide-and-conquer algorithms.</li>

 <li>Implement two classic algorithms for matrix multiplication.</li>

 <li>Handle intricate details of recursive matrix manipulation – identifying and working with segments of two-dimensional arrays, constructing two-dimensional arrays from smaller ones.</li>

</ol>

<ol>

 <li><strong> Design and implement a class named <em>MatrixProduct.</em></strong></li>

</ol>

The only content of <em>MartixProduct</em> class should be the implementation of the following 2 classic algorithms for matrix multiplication: the <strong>“<em>simple” divide-and-conquer</em> algorithm</strong> and the <strong><em>Strassen’s</em> algorithm</strong> (<em>see the lecture handout/slides for these algorithms</em>). Both algorithms take two square matrices A(<em>n</em>×<em>n</em>) and B(<em>n</em>×<em>n</em>) and return a product-matrix C(<em>n</em>×<em>n</em>); <em>n</em> is required to be a power of 2 (you need it to be divisible by 2 without remainder at each level of recursion).

Both algorithms are recursive so <strong>for </strong><strong><em>each </em>algorithm</strong> you need to have the following members:

<ul>

 <li>a <em>public</em> method that will get two <strong><em>square</em></strong> matrices A and B (both of the <strong><em>same size</em></strong>) and will <strong>initiate</strong> the recursion. It will return the final product-matrix (of the same size as A and B). <em>The </em><strong><em>signature</em></strong><em> of this method for each algorithm (i.e. the name, the number and type of parameters, and the return-value type) is specified on the top of the next page*. </em></li>

</ul>




<strong><u>Important</u></strong>: The first thing to do in this method is the <strong><u>validity check</u></strong>, namely:

<ol>

 <li>Check if A and B are <u>square</u> matrices of the <u>same size.</u></li>

 <li>Check if the matrix size (i.e. the n-value) is a <u>power of 2</u>.</li>

</ol>

<strong>        </strong><strong>IF </strong>at least one requirement is <strong>not satisfied</strong>, throw <strong><em>IllegalArgumentException</em></strong> exception.




<ul>

 <li>a <em>private</em> method that carries the recursion (<em>see the lecture handout/slides</em>)</li>

</ul>




<ul>

 <li>as many <em>private</em> supporting methods as you need to do the work.</li>

</ul>




<strong><u>Note</u></strong>: the signature of <em>private</em> methods (name, type and number of parameters, return value’s type) is not mandated, but to stay on track and to avoid confusion, follow the path of the lecture handout/slides. Do <strong>NOT</strong> seek help on the internet – all you need is in the handout.

1 Dr. Hasmik Gharibyan

CSC/CPE349 *<strong> The above-mentioned two </strong><strong><em><u>public</u></em> methods should have the following headers: </strong>

<strong> </strong>

<strong> </strong>

<em>public static  int[][]  matrixProduct_DAC(int[][] A,  int[][] B)</em>

//Compute and return the product of A, B matrices using “<strong>simple” DAC algorithm </strong>presented in class.







<em>public static  int[][]  matrixProduct_Strassen(int[][] A,  int[][] B)</em>

//Compute and return the product of A, B matrixes using <strong>Strassen’s algorithm </strong>presented in class.

<strong> </strong>

<strong><u>Note</u>: </strong>both algorithms are working with integer values.










<ol>

 <li><strong>Design and implement application class(es) to test your two algorithms. </strong></li>

</ol>

<strong> </strong>

You can make a single application class to test both algorithms, or you can create two separate classes – one for each algorithm. An application class will contain a <em>main</em> method very similar to the <em>main</em> method in your <em>Project2_part1 </em>assignment.




<strong><u>Reminder</u></strong>: when testing the functionality of your algorithms, make sure the input matrices are square and of the same size, and that their size is a power of 2 (the two mentioned algorithms can only multiply matrices that satisfy these conditions).