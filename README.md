Download Link: https://assignmentchef.com/product/solved-comp1410-lab-9-dynamic-data-structures
<br>
In this Lab you will practice implementing and using dynamically allocated data structures.

<u>Background</u>:.

The problem of not having enough space to store data, or wasting space by having too much of it using a static data structure (such as an array), can be overcome easily by using dynamic data structures that can grow or shrink in size at run time.




A linked-list is a simple dynamic data structure that is based on self-referential C structures. In this lab you will use such a self-referential structure Student, as defined below, to implement and manipulate a simple linked-list called SLIST.

struct student { int ID; char name[40]; struct student *next; }; typedef struct student Student;

<strong> </strong>

<strong>Work to do: </strong>

You are going to define the following functions (at a minimum – you may design and define additional functions if you find it useful):




<h1>1.  Student *addToList(Student *SLIST);</h1>

– “addToList” will ask for the ID and name of a new student from the user, dynamically create a new Student structure, assign the values for the members, add the new student structure at the END of the student list “SLIST” and return the modified list.




<h1>2.  void printList(Student *SLIST);</h1>

– “printList” will traverse through the list from the beginning to the end and will print info for each student in the format “ID Name
”.




<h1>3.  void printListRR(Student *SLIST);</h1>

– “printListRR” will print the list, RECURSIVELY, starting from the END of the list, in the format “ID Name
”.




<h1>4.  void searchList(Student *SLIST);</h1>

– “searchList” will ask the user to enter a student’s ID, search the list for the student having that ID and will print the data in the format “ID Name
”. If failed, it will print “ID “ID” not found”.




For your convenience, a partial program (Lab9_W2017.c) with the function prototypes and the main() function with a menu option is given. Document the whole program and define the other functions required, as stated above.




It should be noted that this exercise illustrates simple aspects of a more general problem called Resource Management.  For a single computer running under a single operating system, the programming required to manage dynamic allocation and recovery of memory resources is a challenging problem.  Scaling the problem upwards to distributed resource sets under shared ownership and control (e.g. grid, cloud computing) introduces huge and challenging problems for research and businesses alike.




<strong>Summary of the lab requirements:  </strong>You must write one program for this lab, namely Lab9.c. The program must contain definitions of the four functions specified above (as a minimum – you may have more functions).  Be prepared to demonstrate the program with appropriate test input examples.