# Operating-System

Operating System simulation based projects. Problem:
# 1
There are 3 student processes and 1 teacher process. Students are supposed to do their assignments and they need 3 things for that pen, paper and question paper. The teacher has an infinite supply of all the three things. One students has pen,an other has paper and another has question paper. The teacher places two things on a shared table and the student having the third complementary thing makes the assignment and tells the teacher on completion. The teacher then places another two things out of the three and again the student having the third thing makes the assignment and tells the teacher on completion. This cycle continues. WAP to synchronize the teacher and the students.


Explanation: 
1.	In the given solution I have taken all the student processes and resources in 2D array and initialized then to 0. 
2.	I have made 3 student processes in three different functions which will be executed by single s_thread and one t_thread for execution of teacher process. 
3.	User will get a menu to select any two out of three resources that are to be placed on shared table. 
4.	If one process is completed there will be a message printed on the screen saying process is completed.
5.	When one process is executing no other student or teacher process will execute and for achieving this I have used Mutex lock. 
6.	When a process starts to execute it acquires the lock and when it completes the execution releases the lock. 
7.	After completion of all the three processes the program will end.

# 2
Two types of people can enter into a library- students and teachers. After entering the library, the visitor searches for the required books and gets them. In order to get them issued, he goes to the single CPU which is there to process the issuing of books. Two types of queues are there at the counter-one for students and one for teachers. A student goes and stands at the tail of the queue for students and similarly the teacher goes and stands at the tail of the queue for teachers (FIFO). If a student is being serviced and a teacher arrives at the counter, he would be the next person to get service (PRIORITY-non preemptive). If two teachers arrive at the same time, they will stand in their queue to get service (FIFO). WAP to ensure that the system works in a non-chaotic manner. 

 If a teacher is being served and during the period when he is being served, another teacher comes, then that teacher would get the service next. This process might continue leading to increase in waiting time of students. Ensure in your program that the waiting time of students is minimized.
