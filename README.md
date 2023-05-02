Download Link: https://assignmentchef.com/product/solved-comp273-assignment-2-an-8-bit-shift-register
<br>
<h1> An 8-bit Shift Register</h1>

Design an 8-bit shift register with output bits <em>A</em><sub>7</sub><em>A</em><sub>6</sub><em>A</em><sub>5</sub><em>A</em><sub>4</sub><em>A</em><sub>3</sub><em>A</em><sub>2</sub><em>A</em><sub>1</sub><em>A</em><sub>0</sub>. Each bit <em>A<sub>i </sub></em>is represented by the Q output of a <em>rising edge </em>triggered D Flip-flop, which is available in logisimevolution. The circuit has a clock and it also has the following two selector inputs: <em>S</em><sub>0</sub><em>,S</em><sub>1</sub>. The roles of the selector inputs are described in the table below. The timing is such that a hold, shift right, shift left or circular shift right, is controlled by the clock input.

<table width="0">

 <tbody>

  <tr>

   <td width="31"><em>S</em><sub>1</sub></td>

   <td width="31"><em>S</em><sub>0</sub></td>

   <td width="135">Function</td>

  </tr>

  <tr>

   <td width="31">0</td>

   <td width="31">0</td>

   <td width="135">No shift – hold</td>

  </tr>

  <tr>

   <td width="31">0</td>

   <td width="31">1</td>

   <td width="135">Shift right</td>

  </tr>

  <tr>

   <td width="31">1</td>

   <td width="31">0</td>

   <td width="135">Shift left</td>

  </tr>

  <tr>

   <td width="31">1</td>

   <td width="31">1</td>

   <td width="135">Circular shift right</td>

  </tr>

 </tbody>

</table>

The bit that is shifted out, i.e., when you do a shift right or a shift left, should be stored in an additional output called <em>B<sub>out</sub></em>. Correspondingly, an input bit, called <em>B<sub>in </sub></em>should be brought in to the space created by the open position, when you carry out a shift operation. A template file has been provided for you called <em>shift.circ</em>, which you can start with and then modify. Explain your design in words in a separate text file, which you will also upload, and then submit the circuit (<em>shift.circ</em>) implementation in logisim-evolution. Note that the TA’s will download and test your circuit design.

<h1>2           String Capitalization</h1>

You are to write a MIPS program that takes as input a string of text and then does the following.

<ul>

 <li>Prints the input string</li>

 <li>Capitalizes and prints the capitalized string.</li>

</ul>

You can assume that the string input is comprised of words consisting of keyboard alphabetic characters, with each word separated by a single “space” character, and with each word beginning with an alphabetical character. The program should be able to handle strings up to 127 characters in length. No characters other than lowercase letters should be modified. In other words, the input string may have some of its letters already capitalized. Use properties of the ASCII code, and in particular the manner in which characters are represented, to solve this problem!

As a working example, given the input string “this is A StrinG”, the printed capitalized output should be “THIS IS A STRING”. A template file <em>capitalize.asm </em>has been provided for you. In this file, you will note that there is an input string that is hard-coded and there is place for an output string. The TA’s might change the contents of the input string while testing your code. You should use the space allocated for the output string to write in the content of your capitalized output. Then, it should be a simple matter to print it.

<h1>3           Quadratic Congruence</h1>

One of the problems in the set of NP-Complete problems is that of quadratic congruences: given positive integers <em>a</em>, <em>b </em>and <em>c</em>, does there exist an integer <em>x </em>≤ <em>c </em>such that <em>x</em><sup>2 </sup>≡ <em>a </em>mod <em>b</em>? For small values of <em>a</em>, <em>b</em>, and <em>c</em>, we can decide by brute force if the congruence can be solved. Write a program in assembly to get values for <em>a</em>, <em>b </em>and <em>c </em>from the user and then outputs each value of <em>x</em>, for which congruence holds, or reports back that there is no solution. You can use a single main program for this question; i.e., you do not have to use subroutines. However, if you use subroutines make sure that they are commented and your code is well structured. Note that you can use the rem pseudo-instruction to get the modulus of two numbers. Please name your solution file quad.asm.

An example of four test cases is given below. We will test your program with these and some other (different) test cases. Note, you can print your solutions for <em>x </em>in any way you like – the table below just shows the full solution set for certain choices of <em>a,b,c</em>.

<table width="0">

 <tbody>

  <tr>

   <td width="24"><em>a</em></td>

   <td width="30"><em>b</em></td>

   <td width="23"><em>c</em></td>

   <td width="92">Solution (x)</td>

  </tr>

  <tr>

   <td width="24">4</td>

   <td width="30">7</td>

   <td width="23">5</td>

   <td width="92">Yes (2,5)</td>

  </tr>

  <tr>

   <td width="24">1</td>

   <td width="30">5</td>

   <td width="23">6</td>

   <td width="92">Yes (1,4,6)</td>

  </tr>

  <tr>

   <td width="24">3</td>

   <td width="30">10</td>

   <td width="23">4</td>

   <td width="92">No solution</td>

  </tr>

  <tr>

   <td width="24">5</td>

   <td width="30">12</td>

   <td width="23">7</td>

   <td width="92">No solution</td>

  </tr>

 </tbody>

</table>


