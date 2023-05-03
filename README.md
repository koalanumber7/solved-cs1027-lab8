Download Link: https://assignmentchef.com/product/solved-cs1027-lab8
<br>
<h1>Learning Outcomes</h1>

<ul>

 <li>Differentiate between static and non-static variables and methods and their usages</li>

 <li>Compare the effects of changing primitive variables and objects/arrays within instance methods.</li>

 <li>Analyze the approaches to checking for equality between String objects  Apply String formatting to create a clean alignment in print lines</li>

</ul>

<h1>Pre-Lab</h1>




<ul>

 <li>Create a new Java project called Lab8</li>

 <li>Download the files: <a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/VariableTest.java">java</a><a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/VariableTest.java">,</a> <a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/MemoryDemo.java">MemoryDemo.java</a><a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/MemoryDemo.java">,</a> <a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/StringCompare.java">StringCompare.java</a><a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/StringCompare.java">,</a> and <a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/Product.java">Product.java</a></li>

 <li>Save these downloaded files into the Lab8 src folder</li>

</ul>




<h1>Exercise 1 – Accessing static vs. non-static variables</h1>




<ol>

 <li>Open VariableTest.java in Eclipse and examine the code. Notice the difference between sNum and iNum.</li>

 <li>Add a test harness main (String[] args) method at the bottom of this class. Within it, add two consecutive print lines: one printing out iNum and one printing out sNum.</li>

 <li>What does the IDE / compiler say about these lines? Why is one of them valid but the other invalid? Comment out the offending line.</li>

 <li>Create an object and print out the iNum value of that object.</li>

</ol>




<h1>Exercise 2 – Method parameters</h1>




<em>When a primitive variable is declared, it is allocated a memory location. When that primitive variable is initialized (for example, with the value of 5) the value at its memory location takes on the value of 5. In contrast, when a reference variable is declared and initialized, the value at its memory location takes on the value of another memory location. Given this information, can you explain why the following demo works the way that it does? If you are confused, try drawing the memory locations and their values on paper. </em>




<ol>

 <li>Open MemoryDemo.java and examine the code but do <strong>not</strong> run it.</li>

 <li>As you examine the code visually, write down the results you expect it to print out.</li>

 <li>Once you have written the expected results, run the program to see the actual results. Were you correct? If not, review the paragraph at the start of this exercise to try to understand the reason for these results.</li>

</ol>




<h1>Exercise 3 – String equality</h1>




<em>A string created without the use of the new operator is called a string literal (i.e. String s = “hi”). String literals are objects, but the Java compiler will not create two copies of the same string literal. The string literals are saved into a special memory pool and duplicates point to the same literal to reduce the amount of memory that a Java program uses. </em>




<ol>

 <li>Open StringCompare.java but do <strong>not</strong> run it.</li>

 <li>Carefully read through the 6 different test cases written in the test harness. Notice that the first 3 cases use == and the last 3 call the equals() method. Notice also that in each of these sets of 3 cases, the Strings are initialized slightly differently.</li>

 <li>As you examine these 6 different String comparison cases, write down the results you expect from each of the cases (true or false).</li>

 <li>Once you have written expected results, run the program to see the actual results. Were you correct? For any cases in which your expected result was incorrect, review the code to understand why this occurred. Review the paragraph on string literals at the start of this exercise if you are confused by these results.</li>

</ol>




<h1>Exercise 4 – Create a receipt program</h1>




<ol>

 <li>Open Product.java in Eclipse and examine the code.</li>

 <li>Create a new class called Receipt.</li>

 <li>The only instance method you need to implement in Receipt.java is a constructor with the following signature: public Receipt (Product[] cart) { }</li>

 <li>In the constructor, loop through each of the products in the cart array and display each one on its own line with clean formatting. Each line must include the product’s name, code, cost, and the after-tax cost. Use the following hints and guidelines:

  <ul>

   <li>Align the print lines in a table-like structure so that each row (line) is a single product and each column is each of the attributes (name, code, etc.)</li>

   <li>Use format() or System.out.printf() with “%” to help with the alignment. Refer to the zyBook section 9.2 for a refresher.</li>

   <li>If you call prod.getTax() (assuming prod is the Product variable), it will be underlined in yellow to indicate a warning. This means it will technically still compile and run with this line, but it is not recommended. How is this method different from the other getters in Product.java? How should this type of method be called? Call it the proper way so there are no warnings.</li>

  </ul></li>

 <li>Add a print line before the loop to display header labels for each of the columns (product name, code, cost, and after-tax cost) with the same table-like alignment.</li>

 <li>Add a line after the loop that displays the grand total and keep it aligned with the column of the individual product’s after-tax costs.</li>

 <li>Add a test harness main (String[] args) method at the bottom of this class. Within it, initialize at least 3 different Product objects and create a Product array containing these items. Then initialize a new Receipt object with the Product array parameter.</li>

 <li>View an <a href="https://www.csd.uwo.ca/courses/CS1027a/labs/lab08/receipt-output.jpg">example of the expected output</a> (note that you can use any product names, codes, and costs so your output may not be identical to this one).</li>

</ol>


