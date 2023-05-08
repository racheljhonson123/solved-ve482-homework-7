Download Link: https://assignmentchef.com/product/solved-ve482-homework-7
<br>
<strong>Ex. 1 — </strong><em>Page replacement algorithm</em>

In this exercise we consider the WSClock page replacement algorithm with a <em>τ </em>value of two ticks. The system state is given as follows.

<table width="354">

 <tbody>

  <tr>

   <td width="55">Page</td>

   <td width="91">Time stamp</td>

   <td width="63">Present</td>

   <td width="84">Referenced</td>

   <td width="62">Modified</td>

  </tr>

  <tr>

   <td width="55">0</td>

   <td width="91">6</td>

   <td width="63">1</td>

   <td width="84">0</td>

   <td width="62">1</td>

  </tr>

  <tr>

   <td width="55">1</td>

   <td width="91">9</td>

   <td width="63">1</td>

   <td width="84">1</td>

   <td width="62">0</td>

  </tr>

  <tr>

   <td width="55">2</td>

   <td width="91">9</td>

   <td width="63">1</td>

   <td width="84">1</td>

   <td width="62">1</td>

  </tr>

  <tr>

   <td width="55">3</td>

   <td width="91">7</td>

   <td width="63">1</td>

   <td width="84">0</td>

   <td width="62">0</td>

  </tr>

  <tr>

   <td width="55">4</td>

   <td width="91">4</td>

   <td width="63">0</td>

   <td width="84">0</td>

   <td width="62">0</td>

  </tr>

 </tbody>

</table>

<ol>

 <li>Explain the content of the new table entries if a clock interrupt occurs at tick 10.</li>

 <li>Due to a read request to page 4 a page fault occurs at tick 10. Describe the new table entry.</li>

</ol>

<strong>Ex. 2 — </strong><em>Minix 3</em>

The goal of this exercise is to understand and implement system calls.

<ol>

 <li>In which files are:

  <ol>

   <li>the constants with number and name for the system calls?</li>

   <li>the names of the system call routines?</li>

   <li>the prototypes of the system call routines?</li>

   <li>the system calls of type “signal” coded?</li>

  </ol></li>

 <li>What problems arise when trying to implement a system call int getchpids(int n, pid_t *childpid) which “writes” the pids of up to <em>n </em>children of the current process into *childpid?</li>

 <li>Write a “sub-system call” int getnchpid(int n, pid_t childpid) which retrieves the <em>n</em>-th child process.</li>

 <li>Using the previous sub-system call, implement the original getchpids system call. The returned int value corresponds to the number of pids in *childpid, or -1 on an error.</li>

 <li>Write a short program that demonstrate the previous system calls.</li>

 <li>The above strategy solves the initial problem through the introduction of a sub-system call.

  <ol>

   <li>What are the drawbacks and benefits of this solution?</li>

   <li>Can you think of any alternative approach? If yes, provide basic details, without any implementation.</li>

  </ol></li>

</ol>

<strong>Ex. 3 — </strong><em>Research</em>

Write about a page on the topic of the ext2 filesystem. Do not forget to reference your sources.

<strong>Ex. 4 — </strong><em>Simple questions</em>

<ol>

 <li>If a page is shared between two processes, is it possible that the page is read-only for one process and read-write for the other? Why or why not?</li>

 <li>A computer provides each process with 65,536 bytes of address space divided into pages of 4096 bytes. A particular program has a text size of 32,768 bytes, a data size of 16,386 bytes, and a stack size of 15,870 bytes. Will this program fit in the address space? If the page size were 512 bytes, would it fit?</li>

 <li>When both paging and segmentation are being used, first the segment descriptor is found and then the page descriptor. Does the TLB also need a two-levels lookup?</li>

</ol>