# B2 - Pàgina Web Responsive
## Pràctica de Llenguatge de Marques

**Tasca:** Dissenyar i desenvolupar un lloc web *responsive* utilitzant HTML i CSS.

##  Característiques i funcionalitats principals de la pàgina web

### Tema:
Aquesta página web és una web de la vida del filòsof *Albert Camus*.

### Estructura i navegació de les pàgines:
La web compta amb resums de qui és (index.html), sa seva biografía (vida.html), el seu pensament (pensamiento.html) i les seves obres principals (obras.html).

Des de totes les págines es pot accedir a totes les pagines mitjatçant el menu de navegació.

Totes les págines tenen un *header*, dins el cual está el *nav*, després un *section* on hi ha informació diferent en cada pàgina i després un *footer*.

- header
    + nav
- section
- footer

A sa página de "vida.html" he afegit un *article* dins el section perque trobaba més comode de donar-li estils d'aquesta manera.

- header
    + nav
- section
    + article
- footer

### Etiquetes:
He tractat de no abusar de "classes" i de "ids" més de lo estrictament necessari.

He començat posant estils a la primera página, he utilitzat es mateix header i footer per totes i després he anat afegint classes i ids segons ho trobaba necessari.

No he trobat necessari fer servir pseudoelements, però si he fet servir vàries pseudoclasses i selectors semántics d'avegades combinats amb classes i ids. Com per exemple:
```
#contenido_p div:first-of-type {
    flex-basis: 100%;
}
```
o
```
.pensamientos h5:first-child {
    margin-right: 1rem;
}
```

### Disseny adaptatiu:
La pàgina web és *responsive*, he aconsseguit aixó principalment fent us de **flexbox** i de **media queries**.

He fet 3 ***breakpoints***. 

El primer és per **1100px**, després he fet un altre per pantalles més grans, amb un mínim de **1730px** i després he fet un altre pensant en dispositius més petits, amb un máxim de **570px**.

Els *media queries* estan al final de l'arxiu d'estils.

Ho he combinat amb flexbox perque ho trobava més práctic d'aquesta manera.

### Multimédia:

Totes ses imatges tenen un "alt" amb una petita i curta descripció.

Totes ses imatges han estat optimitzades per que no pesin tant amb un compresor d'imatges ([aquest](https://compressor.io/)).

Com la pàgina tenía que tenir un audio o un video, he utilitzat un audio d'aquesta [web](https://incompetech.com/music/royalty-free/music.html).

### Comentaris:
No he tobat necessari comentar el codi HTML perque consider que l'estructura és molt senzilla i autoexplicativa.

Els comentaris a la página d'estils son una petita guia per sabre que estils son de cada pàgina.

Primer he posat uns estils generals on, per exemple, he posat dins :root una serie de colors per poder tenir més a má la paleta de colors que s'esta utilitzant i de pas poder canviar-los més fàcilment en cas de que façi falta:
```
:root {
    --color-1:#44194a;
    --color-2: #ba5a9f;
    --color-3: #e1ff00;
    --color-4: #f0ff8d;
}
```
I després he anant afegint estils de cada part comentant-ho:
```
/*estilos especiales pagina "vida" (selector article reservado para esta pagina)*/
#vida {
    width: 50rem;
    margin: auto;
    display: none;
}
```
### Animacions:
He utilitzat algunes animacions per fer la pàgina més dinàmica. Sobretot he fet servir "@keyframes" i també ":hover".

![Animació header](/readme_medios/animacio_header.gif "Animació header")

A la página de vida he intentat fer un *timeline* i una opció per veure més contingut que d'entrada apareix oculta però en pitjar "saber más" es pot veure.

![timeline i saber mas](/readme_medios/timeline.gif "timeline i saber mas")


---

## Validació W3C
Totes les pàgines han estat aprobades per el [W3C](https://www.w3.org/).

Validació de l'HTML:
![validacio w3c](/readme_medios/w3c_validado.png "validacio w3c")

Validació del CSS:
![validacio w3c](/readme_medios/w3c_validado_2.png "validacio w3c")

## Estructura de carpetes i arxius que conformen la pàgina web
La pàgina web está estructurada de manera en la cual tenim un css anomenat "estilos.css" i 4 pàgines html. Hi ha un fitxer anomenat "medios" dins el qual hi ha algunes imatges, un audio i un altre fitxer anomenat "obras" on he possat imatges dels llibres de l'autor per tenir-les mes organitzades.

L'estructura sería:
+ medios
    - imatges de la web
    - audio
    - obras
        - imatges concretament de les obres
+ estilos.css
+ index.html
+ obras.html
+ pensamiento.html
+ vida.html

## Tecnologies utilitzades en el desenvolupament de la pàgina web.
- El codi l'he fet amb [Visual Studio Code](https://code.visualstudio.com/).
- La font l'he agafat de [Google Fonts](https://fonts.google.com/specimen/Nunito).
- He utilitzat un box-shadow d'un [CodePen](https://codepen.io/airen/pen/eYGKEdz).
- He generat els clip-path amb aquesta eina anomenada [Clippy](https://bennettfeely.com/clippy/).
- He agafat  informació d'[aquí](https://www.biografiasyvidas.com/biografia/c/camus.htm) i d'[aquí](https://en.wikipedia.org/wiki/Albert_Camus).
- He optimitzat les imatges amb aques [compressor](https://compressor.io/).
- He utilitzar un audio d'[aquesta pàgina](https://incompetech.com/music/royalty-free/music.html)


##  Captures de Pantalla:
### Pàgina vida
![captura de la web 1](/readme_medios/captura1.png "captura de la web 1")

### Pàgina obres
![captura de la web 2](/readme_medios/captura2.png "captura de la web 2")

### Página pensament
![captura de la web 3](/readme_medios/captura3.png "captura de la web 3")

### Pàgina inici 1
![captura de la web 4](/readme_medios/captura4.png "captura de la web 4")

### Pàgina inici 2
![captura de la web 5](/readme_medios/captura5.png "captura de la web 5")

### Pàgina inici mòvil
![captura de la web 6](/readme_medios/captura6.png "captura de la web 6")

### Pàgina vida mòvil
![captura de la web 7](/readme_medios/captura7.png "captura de la web 7")
