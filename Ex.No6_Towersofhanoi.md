# Ex.No: 6  Towers of Hanoi problem
### DATE:  02/04/2025                                                                       
### REGISTER NUMBER : 212222040049
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:

move(1,X,Y,_) :-
 write('Move top disk from '),
 write(X),
 write(' to '),
 write(Y),
 nl.
move(N,X,Y,Z) :-
 N>1,
 M is N-1,
 move(M,X,Z,Y),
 move(1,X,Y,_),
 move(M,Z,Y,X).

### Output:

![image](https://github.com/user-attachments/assets/c4f2f911-87f0-4d7c-a4ab-489a7d825533)


### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
