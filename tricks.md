<strong>#Utiliser une union pour stocker couleur</strong>

```c
typedef struct				s_rgb
{
	unsigned char			b;
	unsigned char			g;
	unsigned char			r;
	unsigned char			a; //transparence
}							t_rgb;

typedef union				u_color
{
	unsigned int			all;
	char					tab[4];
	t_rgb					rgb;
}							t_color;
```
-> remplir l'un des trois champ va remplir les autres, car même espace mémoire.
-> unsigned : pas de crash si mauvaise valeur r, g, b.

<strong>#bzero</strong> 
- systematiquement sur structure avant de l'utiliser

<strong>#buffer sizes</strong>
- 4096 = common memory page -> common buffer size.

<strong>#No space left on device</strong> \
 rm -r ~/Library/Caches/* \
 https://github.com/alexandregv/42toolbox/blob/master/free_space.sh

<strong>#Debugger</strong> 
- Ne pas protéger la libc contre le segfault : permet de voir quand ça crash.
- Sinon : faire deux versions de chaque ft, une par défaut, secure, et une non secure avec la commande preprocesseur #ifndef DEBUG, suivi de #endif. Possible d'ajouter des commentaires donnant des infos sur le bug. Compiler avec -D DEBUG. 

<strong>#Memmove</strong> 
Permet de modifier une string sans devoir en malloc une autre. Si je copie les derniers char d'une string, y compris le '\0', et que je les deplace au debut de la string, alors j'ai une nouvelle string plus courte. Ce qui apres le nouvel emplacement du \0 n'est pas à free.

<strong>Bool</strong> 
```c
typedef enum		e_bool
{
	false,
	true
}			t_bool;
```
---> Voir lst_list_sort


<strong>Afficher leaks en sortie de programme</strong> 
```c
system("leaks minishell");
```

<strong>#Macros with arguments</strong>
They work like functions : https://www.9wy.net/onlinebook/CPrimerPlus5/ch16lev1sec3.html

<strong>#Utiliser vscode debugger with stdin</strong>
Dans vscode config, mettre external console à True. Puis press play et ecrire dans la console qui s'ouvre.

<strong>#Flagbit</strong>
->to be continued

<strong>#Bitfield</strong>
->to be continued
