# Blog de Moo Labs.

¿Cómo se escribe una entrada? El motor utilizado es Jekyll. El formato recomendado es usar [Markdown](https://www.markdownguide.org/basic-syntax/) pero Jekyll soporta Textile.

Un ejemplo de post en Markdown:

``` liquid
---
layout: post
author: Eder A. Trujillo
about: Un buen muchacho al que le gustan los perritos
twitter: "@ederywonton"
github: Narinas
email: eatrujillo@protonmail.com
website: https://www.narinas.xyz
---

$$
\int_0^{u} a |J(u)|d\alpha =  \pi
$$

$$
A = \begin{bmatrix}
1 & 2 & 4 \\
2 & 5 & 10
\end{bmatrix}
$$
{% highlight python %}
import numpy as np

def temkiu(u: str): -> str

    return f'temkiu {u}'

{% endhighlight %}
# Es ora neque obortis Amyclis nemus

## Flumina Ianthe

Lorem markdownum ingens remeat. Quid aureus stravit cetera? Iam ducunt sopita
sibi quoque cardine liceat toto, [superasse aequor](http://www.ad-accipit.io/) e
mallet contingere copia.

Nubibus in venit mihi iam aer scinditur bis trahebant poenam o **ad huc** est.
Refugitque sinus asper cubitoque ignes erubuisse, iacuit violave utiliter est
anili venias. Aede ego mulcebunt ante vestra cum adacto spatium paelicis; quid
ad cadit nec putant vidit breve.
```

Como se puede observar, el blog soporta expresiones de Latex para símbolos matemáticos. Jekyll por default utiliza {% highlight %} para bloques de código.

En la parte de arriba se definen las variables de usuario. Respetar ```layout: post```

En la carpeta ```_drafts``` se pueden hacer los borradores, ahí hay otra guía de cómo publicar.

## Instalación local.

- Clonar rama main del repo.
- Instalar Ruby y Gems, hacer disponibles en el PATH.
- Ejecutar ```gem install jekyll bundler```.
- ```cd <ruta-a-repo>```
- ```bundle install```
- ```jekyll serve```

## Actualización.

- Hay una GitHub action que actualiza el blog con cada que se hace push a ```main```.
- Asegurarse de hacer ```git pull origin main``` cada que se vaya a actualizar.
- Ignorar rama ```gh-pages```que ahí es donde se genera el sitio.

## Archivos estáticos.

Hay folders ```css/```, ```images/```, ```js/```, etc. donde se pueden modificar y añadir recursos para el blog. Si se va a hacer referencia a algún archivo en estos folders se especifica así: ```{{ 'folder/recurso.ext' | relative_url }}```. Dentro de los posts, se hace la referencia directamente: 
``` markdown
![My helpful screenshot](/assets/screenshot.jpg)
```

## Pendientes:

[] Hay un sistema de etiquetas, hay que decidir cómo usarlo.
[] Acerca de.
[] Hay una pestañita de proyectos, aún no sé bien qué podríamos poner ahí.