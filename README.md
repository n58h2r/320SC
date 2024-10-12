java cComputer Science 320SC – (2024)
Programming Assignment 5
Due: Oct 13 2024 (11:59pm)
Academic Integrity
Before attempting to solve the assignment, please read the message below very carefully.
As described on https://academicintegrity.cs.auckland.ac.nz/, you must NOT
 Use all or part of another student’s solution to the assignment. Changing variable names or
substituting words in a sentence does not make it your solution.
 Allow someone else to complete all or part of the assignment for you.
 Solicit answers for the assignment on contract-cheating websites such as Chegg.com and
Bartleby.com.
 Use code from Internet sources such as StackOverffow or generative-AI tools such as ChatGPT.
 You are encouraged to learn from Internet sources and tools, but you need to come up
with your own implementation of the code to show your learning.
 Allow another student to copy all or part of your solution to the assignment.
 Do all or part of an assignment for someone else.
 Share code that can lead to the solution of an assignment.
 Post the assignment anywhere online or share it with anyone else. The assignment material
is copyrighted and sharing or posting them online violates our copyright.
 Post your solution online on public websites. Your online solutions will encourage other
students to copy your solution. Private GitHub repositories and other private online storage
 drives are acceptable, and you can also share your solution privately with prospective
employers.
 Reuse your own work unless discussed otherwise with the lecturer.
 Leave your computers, devices, and belongings unattended — you must secure these at all
times to prevent anyone having access to your assessments or solutions.
Last year, out of 218 students, there were 11 misconducted cases found on A5 - Task 1. We kept the
submissions from the last few years to run MOSS at https://theory.stanford.edu/~aiken/moss/.
I hope that there will be no cases this year!
1Requirements
This 5th assignment lets you get familiar with dynamic programming design and development. It is
worth 5% of your total course marks. We would like you to implement efffcient dynamic programming
algorithms for two tasks: Task 1: Finding partner and Task 2: Killing enemies.
An excessive number of submissions (over 10) for a particular problem will accrue a 20% penalty per that
problem if you eventually solve it. Therefore, please write a bruteforce algorithm and test your
dynamic programming version with your own generated inputs at scale before submitting
to the automated marker.
We only accept Python programs that use built-in packages (i.e. packages that do not require pip
install).
1 Task 1: Meet your partner at skyscraper
1.1 Problem description
You are standing at the ground ffoor and your partner is waiting at the top ffoor of a skyscraper. You
will have to use an algorithmically designed lift L to reach your partner. The lift L is designed in the
manner that if you use the lift at the ffoor i, you are able to reach any ffoor from i + 1 to i + L[i] where
L[i] is a positive integer that presents the capacity of the lift at the i-th ffoor. Each time you use the
lift costs $1.
Assume that the skyscraper has n ffoors and you are at the ffoor 0. Your partner is at the ffoor n − 1
and waiting for you to see the sky view. The lift information L[i] for 0 ≤ i < n is available at the
ground ffoor. Write a function to return the minimum cost, i.e. the number of time using the lift, to
reach yo代 写320SC、Python
代做程序编程语言ur partner.
O(n) solutions are preferred since we have set the running time limit on the automarker.
1.2 Test case description
Your input will be a sequence of n integers, each value per line corresponding to the lift information
L[i] (e.g. the capacity of the lift) on the i-th ffoor. The ffrst line is for the 0-th ffoor. The last line is
for the (n − 1)-th ffoor, which is a redundant information :-). Your output will be an integer.
There are 4 test cases.
1. A trial test case of n = 10 has no mark.
2. A test case of n = 100, 000 and has 1 mark.
3. A test case of n = 1000, 000 and has 2 marks.
2Sample Input 1:
Sample Output 1:
1
You only need to use the lift once since L[0] = 8 is sufffcient to get you to the 4th ffoor.
Sample Input 2:
Sample Output 2:
2
You only need to use the lift twice. The ffrst one with L[0] = 2 to the 1st ffoor, and L[1] = 5 is sufffcient
to get you to the 4th ffoor.
32 Task 2: Arrange tanks to eliminate enemies
2.1 Problem description
You have a queue of n tanks hidden in a forest. Due to the UAV of enemies, only 1 tank is used per
day, and the used tank can only be taken from the front or rear of the queue for some security reasons.
Each tank has a number indicating the number of potential units the tank can eliminate. Since tanks
are hurrily queued up during the night, you cannot organize the tank in the good order to use. Instead,
you have a queue of n values, each reffects the number of potential eliminated units for each tank in
the queue.
Since the war is more and more severe, the number of potential eliminated units dramatically increases
day-by-day. Let the labels of the number of eliminated units from n tanks in the queue be t1,t2, . . . ,tn.
In the i-th day, the used tank k will eliminate i ∗ tk units.
As a commander, for each day, your task is to give an order 1 or 0 corresponding to whether the front
or the rear tank in the queue is used. Write a program to compute the best order of using n tanks for
n days to eliminate maximum number of enemies’ units.
Since there might be several orderings that output the same number of eliminated units, you would
need to output the maximum number of eliminated units only.
You might see that the best solution runs in O(n
2
) time asymptotically. However, a program with low
memory usage (e.g. O(n)) is preferred since the automarker has limited resources, and we have set the
running time limit on the automarker.
2.2 Test case description
Your input will be a sequence of n integers, each value per line i corresponding to the amount of eliminated
 units of the tank ti
. The ffrst and last lines correspond to the front and rear tanks, respectively.
Your output is an integer in range [0..2
31
] corresponding to the maximum number of eliminated units.
There are 2 test cases.
1. A trial test case of n = 10 has no mark.
2. A test case of n = 10, 000 has 2 marks.
4Sample Input 1:
Sample Output 1:
128
The order is {1, 0, 0, 1, 1}, and the maximum number of detroyed units is 4 * 1 + 10 * 2 + 4 * 3 + 8 *
4 + 12 * 5 = 128. Note that for the last tank (#3), any order of 1 or 0 does not matter.
Sample Input 2:
Sample Output 2:
261
The maximum number of detroyed units is 261 and the order is {1, 1, 1, 0, 0, 0, 0, 1}. Note that for the
last tank (#4), any order of 1 or 0 does not matter.
Submission Procedure
Submit your program solutions to https://www.automarker.cs.auckland.ac.nz.
5

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
