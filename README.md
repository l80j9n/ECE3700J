java c
ECE3700J Introduction to Computer Organization
Lab 2 Assembly Programming
Purpose
This lab is design for you to have a programming experience   with   RISC-V   assembly   instruction   set.
Tasks
Develop a RISC-V assembly program that operates on a   data   segment   consisting   of   an   array   of   32-   bit signed integers. In the text (program) segment   of   memory, write   a procedure   called main   that         implements the main()   function as well as procedures for other subroutines   described below.
Assemble, simulate, and carefully comment the file.   Screen print your   simulation results   and explain the results by annotating the screen prints. You should compose   an   array whose   size   is   determined by you in the main   function and is not less than 30   elements.
In this lab, you are allowed to use only RV32I BASE INTEGER   INSTRUCTIONS.   Any   Extension   Instruction   Sets or pseudo-instructions should be avoided.
main()   {
int size =   ...;      //determine   the   size   of   the   array here
int hotDay, coldDay,   comfortDay;
int tempArray[size] =   {36,   25,   -6,
... //compose   your   own   array   here
//test data will be provided   at demonstration
};
//hotDay is the number of   values   greater   than   or   equal   to   30   in   tempArray[]
hotDay =   countArray   (                  ,                      ,                           );
//coldDay is the number of   values   less   than   or   equal   to   5   in   tempArray[]
coldDay =   countArray   (                  ,                      ,                           );
//comfortDay is the number of   values   between   5   and   30   in   tempArray[]
comfortDay =   countArray   (                     ,                      ,                         );
}
int countArray   (int A[], int   numElements,   int   cntType)   {
/*************************************************************************
* countArray   (int A[], int   numElements,   int   cntType);                                                 代 写ECE3700J Introduction to Computer Organization Lab 2 Assembly ProgrammingSQL
代做程序编程语言            *
* Count specific elements   in   the   integer   array A[] whose   size   is                        *
* numElements and   return   the   following:                                                                                                    *
*                                                                                                                                                                                                                     *
* When cntType = 1,   count   the   elements   greater   than   or   equal   to   30;               *
* When cntType = -1,   count   the   elements   less   than   or   equal   to   5;                        *
* When cntType = 0,   count   the   elements   greater   than   5   and   less   than   30.   *
*************************************************************************/
int   i,   cnt   =   0;
...... //complete   the   code   here
//must call functions   hot(),   cold(),   and   comfort()
return   cnt;
}
int hot   (int   x)   {
if(x>=30) return   1;
else   return   0;
}
int   cold   (int x)   {
if   (x<=5)   return   1;
else   return   0;
}
int   comfort   (int x)   {
if   (x>5    x<30)   return   1;
else   return   0;
}
Deliverables
This is a   1-week lab. The full   score   for this   lab   is   200 points.
1)         Demonstrate your program and simulation results to the TAs before your lab session   ends.   Go through the program step by step and show corresponding   changes   in   the   registers   and   memory.
2)       Upload the   source   file(s)   on   Canvas by 22:00   pm,   June   1,   2024.This is an individual assignment. Your work must be submitted electronically   to   Canvas before   the      specified due date. Late submission will result   in 0 point   for the   corresponding   deliverables.   Source   code must be submitted before a grade for this lab   can be   assigned.
Grading Policy
Demonstration: 80%
Source code: 20%





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
