# 022 - Instrumentation

## Calcul de l'inclinaison

On doit normalement calculer cette inclinaison à partir d'une vitesse vraie (TAS) et non d'une vitesse indiquée (IAS).
On peut utiliser la formule approchée :

```
ΦSTD = 15/100 x Vp
```

Ou la formule exacte mais en unités système international (SI) : 

```
tan Φ = (Vp x ω)/g
```

## Logiciels embarqués

### Classement

Niveau A : Logiciel dont la panne cause ou contribue à une panne catastrophique de l’avion.
Niveau B : Logiciel dont la panne cause ou contribue à une situation sérieuse / dangereuse.
Niveau C : Logiciel dont la panne cause ou contribue à une panne majeure.
Niveau D : Logiciel dont la panne cause ou contribue à une panne mineure.
Niveau E : Logiciel dont la panne n’a pas d’effet sur l’avion ou sur la charge de travail du pilote.


## Centrale Inertielle

Principe de l’inertie :
On mesure l'accélération horizontale "gamma"
On intègre une première fois, on obtient : Vs
On intègre une deuxième fois, on obtient : la position.


## Conséquence d'une fuite sur le tube Pitot

Une fuite de pression totale provoque une diminution de la pression totale qui arrive à l’anémomètre.
Si l’avion est en croisière à vitesse constante :
- Pt diminue du fait de la fuite.
- Ps reste constante.
- Pd = Pt - Ps diminue et donc la vitesse indiquée (IAS) diminue.


## Facteur de charge et virage

En mécanique du vol, on montre que : tan Φ = Vp²/(g x r) avec Φ : inclinaison, Vp la vitesse propre, g = 9,81 m/s² : l’accélération de la pesanteur et r le rayon de virage.
On voit sur le dessin ci-dessus que, par rapport au nord, les vitesses de rotation autour du centre du virage et autour de l’axe de lacet de l’avion sont les mêmes.
Autour du centre du virage, on peut écrire que : Vp = r x ω avec r le rayon de virage et ω (en rad/s) la vitesse de rotation de l’avion autour du centre du virage et de son axe de lacet.
Si dans tan Φ = Vp²/(g x r), on remplace r par Vp/ω on obtient : tan Φ = (Vp x ω)/g
D’où : ω = (g x tan Φ)/Vp
Ainsi, si on considère g constante, le taux de virage ou vitesse de changement de cap de l’avion ne dépend que de sa vitesse propre et de son inclinaison.
En pratique, on vire souvent au taux de virage standard (ou taux 1) qui est de 180°/minute. Pour calculer l’inclinaison à adopter pour virer au taux standard, on utilise la formule approchée suivante : ΦSTD = 15/100 x Vp