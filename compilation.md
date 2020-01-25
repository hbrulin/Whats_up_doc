<strong>#gcc</strong>
- '-c' : create object file
- '-o' name

<strong>#faire une librairie asm</strong>
ar rcs

<strong>#debugger</strong>
- '-g' - pour vscode, lldb, fsanitize
- -fsanitize=address

<strong>#optimisation</strong>
- '-j' :opti compil
- '-O3', '-lfto' :opti running program

<strong>#fichier .d dependance header</strong>
- '-MMD'
- définir 'DPD = $(OBJ:.o=.d)'
- '-include $(DPD)' en fin de makefile

<strong>#compil nasm</strong>
- 'nasm -f macho64 test.s -o test.o'
- '-g' valable


A ajouter : 
- makefile tricks, compile with librairies, include headers
