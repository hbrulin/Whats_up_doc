<strong>#Run lldb :</strong> \
lldb ./name web_root

<strong>#Commands :</strong>\
r (run the program) \
s (step in) \
n (step over) \
finish (step out) \
c (continue) \
q (quit the program)

<strong>#Setting a breakpoint in asm :</strong> \
b adresse
Then run : r

<strong>#Next instruction : </strong> \
next / n \
<strong>#Next breakpoint :</strong> \
continue/c

<strong>#See more of current stack frame:</strong> \
d

<strong>#Getting a back trace (call stack) :</strong> \
bt

<strong>#Going to upper stack frame :</strong> \
up \
<strong>#Back down to breakpoint-halted stack frame :</strong> \
down 

<strong>Dumping register values : </strong> \
register read \
<strong>#One register : </strong> \
register read rdi

<strong>#Show frame variables : </strong> \
fr v \
<strong>#Show content of one variable : </strong> \
p

<strong>#Find out which system calls are made :</strong> \
dtruss

<strong>#Disassemble</strong> \
compiler un .c avec un -g : Faire ensuite lldb nom du programme, set a breakpoint et r -> affichage du code en assembleur

<strong>#Ressources :</strong> 
- http://nickdesaulniers.github.io/blog/2016/01/20/debugging-x86-64-assembly-with-lldb-and-dtrace/ 
- lldb commands : https://lldb.llvm.org/use/map.html 
