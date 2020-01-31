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


<strong>#Flagbit</strong>
->to be continued

<strong>#Bitfield</strong>
->to be continued
