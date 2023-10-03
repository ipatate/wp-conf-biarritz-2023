---
theme: apple-basic
class: text-center
highlighter: 'prism'
lineNumbers: false
info: |
  ## WordPress Full Site Editing en 2023
drawings:
  persist: false
transition: slide-left
title: Full site editing en 2023
mdc: true

fonts:
  # basically the text
  sans: 'Sora'
  # for code blocks, inline code, etc.
  mono: 'Fira Code'
layout: intro
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

<div class="absolute top-16">
  <h1 class="text-[#5c6fc7]">Arrêtez d’écrire du PHP*, passez au Full Site Editing</h1>
</div>

<h3 class="mt-32">Adieu The Loop ! <noto-confetti-ball class="w-10 h-10" /></h3>

```php
<?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>
...
<?php endwhile; else : ?>
 <p><?php esc_html_e( 'Sorry, no posts matched your criteria.' ); ?></p>
<?php endif; ?>
```

<div class="absolute bottom-20 right-10">
  <span class="text-sm">
    *dans vos templates
  </span>
</div>


---
---
<div class="flex items-center gap-10 h-full">
<div class="flex-1">
<h1 class="text-[#5c6fc7]">Faramaz Patrick</h1>

<br />
<br />
Développeur depuis plus de 15 ans
Indépendant depuis 2016 (FR, CH)
<br />
<br />
<br />
<br />

**ReactJS - VueJS - Next.js - Nuxt.js - WordPress - Craft CMS**
</div>
<div class="flex-1">
<img src="/assets/media/1646725690644.jpeg" class="" />
</div>
</div>
---
---
<div class="flex items-center gap-10 h-full">
<div class="flex-1">
<h1 class="text-[#5c6fc7]">Co-présentateur du podcast Double Slash</h1>

Podcast bimensuel sur le développement web moderne

https://double-slash.dev/

</div>
<div class="flex-1">
<img src="/assets/media/ArtworkPodcastMain_w6nuaf.png" class="" />
</div>
</div>

---
layout: section
---

# But de la présentation

Expliquer les bases du Full Site Editing pour vous donner envie de tester et d'approfondir le sujet.

Et pourquoi pas sortir un premier site dans quelques mois en mode FSE <twemoji-rocket />


---
layout: section
transition: slide-up
level: 2
---

# Rapide Historique


---
transition: fade
level: 2
layout: section
---

## Avant l'arrivée de Gutenberg, WordPress ne proposait que TinyMCE en tant qu’éditeur de contenu.

<img src="/assets/media/styleselect.png" class="w-100 mx-auto mt-10 shadow" />

<small>&#160;</small>

---
transition: slide-up
level: 2
layout: section
---

## Avant l'arrivée de Gutenberg, WordPress ne proposait que TinyMCE en tant qu’éditeur de contenu.

<img src="/assets/media/styleselect.png" class="w-100 mx-auto mt-10 shadow" />

<small>En 2005, l'éditeur TinyMCE a été intégré à Wordpress 2.0 et continue d'être utilisé dans l'éditeur WordPress Classic.</small>

---
transition: slide-up
level: 2
layout: section
---

## Trop limité pour les développeurs.euses et les utilisateurs.trices

C'est donc à cause de cette faiblesse que l'on a vu l'apparition de différentes alternatives :

- shortcodes (mauvaise UX)
- ACF avec les flexibles contents (mauvaise UX)
- Les pages builders tels que Divi, Elementor, etc. (...)

Ces derniers ont pris une grosse part de marché en attendant que WordPress sorte enfin une vraie solution.


---
transition: slide-up
level: 2
layout: section
---

## L’idée du changement

### 2016
L'idée d'un nouvel éditeur visuel plus avancé a été initiée par Matt Mullenweg (créateur de WordPress) lors du WordCamp US **2016**.

### 2017
Le projet Gutenberg a donc commencé en 2017, ce qui a conduit à la création d'une équipe de développement dédiée à ce projet. Cette équipe a travaillé sur Gutenberg jusqu'à sa sortie en **2018**

### 2018
Gutenberg est donc un éditeur de contenu pour WordPress. Il a été intégré pour la première fois dans la version 5.0 du CMS en décembre **2018**. Soit <strong class="text-[#5c6fc7]">5 ans</strong> déjà !!!

---
transition: slide-up
level: 2
layout: section
---

## Une sortie un peu chaotique !
<div class="mt-10"></div>

### Pas prêt et pas un builder !

À sa sortie, Gutenberg n'était qu'un éditeur de contenu et son interface n'était pas du tout la même qu'aujourd'hui, et encore moins un équivalent d'un constructeur de pages tel qu'Elementor.

<div class="mt-10"></div>

Dans un premier temps, il y a eu une forte opposition à ce changement. Une grande partie de la communauté était contre l'arrivée de Gutenberg. <openmoji-stop-sign class="w-8 h-8" />

Nous avons vu la sortie d'un fork de WordPress sans Gutenberg : "ClassicPress". <game-icons-pirate-grave class="w-8 h-8" />

L'un des plugins les plus populaires encore aujourd'hui est "Disable Gutenberg"<br /> avec plus de **700 000** installations. <twemoji-exploding-head class="w-8 h-8" />


---
transition: slide-left
level: 2
layout: section
---

# L’arrivé du Full site editing


Le FSE, ou "éditeur de site", permet aux utilisateurs.rices de personnaliser le site entier, y compris les en-têtes, les pieds de page, la navigation et les modèles de page, etc.. directement depuis l'éditeur de site.

### WordPress 5.8 - juillet 2021

Il a été introduit pour la première fois dans WordPress 5.8 en juillet 2021 et fait partie de la phase 2 de la feuille de route.


---
layout: section
transition: slide-up
level: 2
---

# Pourquoi utiliser Gutenberg et le FSE ?


---
layout: section
transition: slide-up
level: 2
---

## 1 - Parce que c’est natif et dans le core de WordPress
<div class="mt-10"></div>

Pour utiliser Gutenberg, vous n’avez pas besoin d’installer un plugin ou de payer une licence. C’est disponible directement dans une nouvelle installation de WordPress.

Le développement de l’éditeur Gutenberg peut-être testé et suivi via le plugin. Le plugin embarque les évolutions de l’éditeur avant d’être mergé dans le core de Wordpress à chaque sortie d’une nouvelle version.

Comme pour le CMS, Gutenberg est totalement open-source.


---
layout: section
transition: slide-up
level: 2
---

## 2 - Une interface simple (presque) et rapide

<div class="mt-10"></div>
L’interface est totalement intégrée à l’administration WordPress et les fonctionnalités restent en majorité intuitives.

Depuis les premières versions, l’éditeur Gutenberg a été largement optimisé et il fonctionne assez rapidement. Quand on veut éditer un contenu, l’éditeur se charge sans latence.

Votre admin reste rapide et c’est très important pour une personne qui passe beaucoup de temps dans l’admin.

---
layout: section
transition: slide-up
level: 2
---

## 3 - Le code HTML qui en sort est assez concis

<div class="mt-10"></div>
Le HTML généré par Gutenberg est plutôt propre et la majorité du style des éléments est basée sur des variables CSS.

De base, un site réalisé avec Gutenberg/FSE est déjà performant même sans optimisation (cache, etc..)

---
layout: section
transition: slide-up
level: 2
---

Exemple de code HTML sur un simple titre avec Elementor :

```html
<div
  class="elementor-element elementor-element-3629291 elementor-widget elementor-widget-heading"
  data-id="3629291"
  data-element_type="widget"
  data-widget_type="heading.default"
>
  <div class="elementor-widget-container">
    <h2 class="elementor-heading-title elementor-size-default">
      Mon titre
    </h2>
  </div>
</div>
```

---
layout: section
transition: slide-up
level: 2
---

Code HTML pour le même titre avec Gutenberg :

```html
<h2 class="wp-block-heading">Mon titre</h2>
```

---
layout: section
transition: slide-up
level: 2
---

## 4 - Réglages de l’interface pour guider l’utilisateur.rice

<div class="mt-10"></div>
On peut régler assez finement certains réglages de l’interface :

- Les couleurs disponibles
- Les polices disponibles
- Les tailles des containers
- ….

Cela permet de garder une bonne cohérence entre les pages. L’éditeur de contenu est guidé et ne se retrouve pas perdu.


---
layout: section
transition: slide-up
level: 2
---

## 5 - Des éléments prêts à l’emploi dans l'interface

<div class="mt-10"></div>
Avec les blocs et les patterns, l’éditeur de contenu dispose d’éléments disponibles et mis en forme.

Il suffit donc d’ajouter les éléments dans le contenu et juste d’éditer le contenu de cet élément. Simple et rapide.

Un gain de temps considérable et les utilisateurs se retrouvent plus confiant.


---
layout: section
transition: slide-up
level: 2
---

## 6 - Le thème peut être contenu dans des fichiers et pas uniquement en base

<div class="mt-10"></div>
En tant que développeur, je peux créer un thème FSE basé sur des fichiers et déployer mon thème en production sans la base-de-donnée.

Vous pouvez conserver les fichiers sources sur un gestionnaire de versions et travailler d’une façon plus professionnelle.


---
layout: section
transition: slide-up
level: 2
---

## 7 - Réutilisation des éléments d’un site à l’autre

<div class="mt-10"></div>
On peut se créer plusieurs blocs, patterns et templates afin d’optimiser la production de site.

On retrouve souvent les mêmes éléments d’un site à l’autre.

Exemple : FAQ. Je peux réutiliser tout mon système de FAQ sur différents sites.

---
layout: section
transition: slide-left
level: 2
---

## 8 - Parce que ...

- C'est présent dans WordPress et ça ne risque pas de changer
- Permet de livrer des sites professionnels
- Permet une grande autonomie des utilisateurs.rices/editeurs.rices
- WooCommerce passe de plus en plus sur les blocs.


---
layout: section
transition: slide-up
level: 2
---

# Lexique du FSE


---
transition: slide-up
level: 2
---

### theme.json

Le fichier de config pour les réglages du Gutenberg et du FSE + les styles par défaut des blocs.
<br />Sans le savoir nous utilisons déjà le fichier theme.json de WordPress.

### Styles

Dérivés du theme.json pour proposer des styles différents pour un même theme.

### Les templates (modèle de contenu)

Comme le nom l’indique, il s’agit de template de page. Dans la création d’une page, nous avons soit le template par défaut, soit un template que l’on choisit dans le sélecteur.
<br />Les templates sont 100% HTML.

### Les templates parts (éléments de modèles)

Les parts représentent des éléments de template. Comme le header, le footer ou même des petits éléments comme le post-meta.html que l'on retrouve dans le thème twenty-twenty-three.
<br />Les parts sont 100% HTML

---
transition: slide-up
level: 2
---

### Les patterns (compositions)

Ce sont des sortes de composant HTML réutilisables. Des blocs HTML avec du style déjà assemblés disponibles directement dans l’éditeur Gutenberg.<br />
Les patterns sont sous forme de fichier PHP mais nous verrons un peu plus tard que le rendu reste en mode HTML.

### Les synced patterns (compositions synchronisées)

Ce sont des patterns réutilisables dans plusieurs contenus/pages et l’on peut modifier le pattern une seule fois pour toutes les pages. Uniquement disponible en passant par l'administration.

### Block

Ce sont les éléments principaux de l’éditeur Gutenberg. Dynamique ou statique, ils sont disponibles dans le sélecteur de bloc Gutenberg.<br />

Ils disposent de paramètres (ou pas) sur la colonne de droite dans l’éditeur.
Connaissez-vous la différence entre un bloc statique et un bloc dynamique ?

---
transition: slide-up
layout: section
level: 2
---

# Un nouveau modèle mental

---
transition: slide-up
level: 2
class: top-32
---

Les templates sont en HTML, logiquement, ils ne sont pas dynamiques. Cela oblige donc à réfléchir sous forme de bloc/pattern.

Dans une page, dans un template, dans un part, tout est bloc. Tout doit être pensé sous forme de bloc.

Pour les personnes qui font des Web Apps avec React/Vue, etc.. c’est déjà une habitude de penser comme cela.
Pour les autres, il faut se forcer à penser sous forme de bloc.

---
transition: slide-up
level: 2
layout: section
---

## Il est possible de couvrir 80% des besoins avec les blocs de base présent dans WordPress

- block group, row, column
- block heading, paragraph, list, image, etc..
- block navigation, site logo, etc..
- query loop, post title, post content, etc..

<div class="mt-10"></div>

### Plus avancé

- Block variations pour étendre les blocs de base (query loop, etc..)
- Plugin pour l'interface Gutenberg (sidebar, post status, etc..)

---
transition: slide-up
level: 2
layout: section
---

# Avec le FSE, on ne pense plus sous forme de page mais sous forme de blocs

## Stop les maquettes de pages


---
transition: slide-up
level: 2
layout: section
---

# Atomic design

On peut aussi prendre l’atomic design comme modèle qui représente parfaitement le mode de pensée du FSE.

L’atomic design comprend des éléments sous forme d’atomes, de molécules, d’organismes, de template et de page. Vous voyez où je veux en venir ?

---
transition: slide-left
level: 2
layout: section
---

<img src="/assets/media/1_U-jFHRJxePDHHBWtd19M8g.webp" />


---
transition: slide-up
layout: section
level: 2
---

# Getting started


---
transition: slide-up
level: 2
layout: section
---

<div class="mt-10"></div>

## Créer un Block Theme

Il suffit d'ajouter un fichier index.html dans un repertoire templates.

<img src="/assets/media/getting-started.png" class="w-134 mx-auto mt-10 shadow" />

<div class="absolute bottom-5">Demo <bi-terminal /></div>

---
transition: slide-up
level: 2
layout: section
---

# Ok, et après ?


---
transition: slide-up
level: 2
layout: section
---

## Code HTML des utilisés dans les templates, parts et patterns

Le code HTML représente des éléments (blocs, patterns, etc..). Les valeurs contenues dans les commentaires sont les réglages des éléments.
Le code est parsé pour être rendu dans l'éditeur. En front les commentaires sont supprimés.

### Un container group

```html
<!-- wp:group {"layout":{"type":"constrained"}} -->
    <div class="wp-block-group">
    </div>
<!-- /wp:group -->
```

### Un paragraphe

```html
<!-- wp:paragraph -->
<p>Deserunt excepteur sunt consequat ad ea nulla ex.
Ut ullamco nostrud do exercitation id pariatur exercitation sunt qui est aliquip.</p>
<!-- /wp:paragraph -->
```

### Un titre

```html
<!-- wp:heading {"textAlign":"center","fontSize":"3xlarge"} -->
<h2 class="wp-block-heading has-text-align-center has-3-xlarge-font-size">Ut ullamco nostrud do</h2>
<!-- /wp:heading -->
```



---
transition: slide-up
level: 2
layout: section
---

# Méthode 1

## Je créer mes élements directement dans l'interface de l'éditeur de site

- Templates
- parts (header, footer, etc..)
- patterns (compositions)


---
transition: slide-up
level: 2
layout: section
---

### Je peux exporter le thème sous forme de fichier

Dans tous les panneaux d'édition de l'éditeur de site > Options > Export (Tools)

<img src="/assets/media/export.gif" class="w-160 mx-auto shadow" />


---
transition: slide-up
level: 2
layout: section
---


# Méthode 2

## Je fais directement dans mon éditeur de code tous les fichiers dans le thème (Mode je sais ce que je fais !)

From scratch ou en utilisant un Block Theme :

- <https://olliewp.com/>
- <https://github.com/WordPress/twentytwentyfour>

<div class="mt-10"></div>
PS : J'ai le droit d'utiliser l'interface ;)


---
transition: slide-up
level: 2
layout: section
---

## Comme je ne connais pas tous les élements, je peux utiliser l'interface de l'éditeur de site pour m'aider.

Je peux faire mes templates, templates part via l'interface et copier le code source.

Dans tous les panneaux d'édition de l'éditeur de site > Options > Copy all blocks (Tools)

ou passer en mode "Code Editor" et copier la source.


<img src="/assets/media/code-source.png" class="w-134 mx-auto mt-10 shadow" />


---
transition: slide-up
level: 2
layout: section
---


## Comme je privilégie les versions fichiers (locales), je ne conserve pas les versions modifiées en base de données.


J'efface les customisations via :

- dans le panneau gauche de l'edition d'un élément

<img src="/assets/media/reset-edit.png" class="w-134 mx-auto mt-10 shadow" />

---
transition: slide-up
level: 2
layout: section
---

### ou via l'interface de gestion des templates (ou parts, patterns)

<img src="/assets/media/reset-list.png" class=" mx-auto mt-10 shadow" />


---
transition: slide-left
level: 2
layout: section
---

# À retenir


- Toutes les modifications sont enregistrées en base de données
- Les fichiers du thème ne sont jamais modifiés
- Aucun fichier n'est créé
- On peut exporter le thème complet modifié avec la fonction disponible dans l'interface
- Pour prendre en compte le fichier et non la version DB, il faudra effacer les customisations

<div class="mt-10"></div>

**Toutes les customisations sont enregistrées dans la table ```{prefix}posts```. Avec des post_types "wp_template_part, wp_template, wp_navigation, etc.."**


---
transition: slide-up
layout: section
level: 2
---

# Le fichier theme.json
## Un des fichiers le plus important du FSE
---
transition: slide-up
level: 2
---

### Par défaut, votre WordPress utilise déjà le theme.json qui se trouve dans wp-include.

*si vous utilisez Gutenberg !*

## Il permet de configurer l'interface de Gutenberg et de mettre des styles par défaut.


```json
{
    "$schema": "https://schemas.wp.org/wp/6.3/theme.json",
    "version": 2,
    "settings": {},
    "styles": {}
}
```

<div class="mt-6 p-5 rounded bg-gray-100 text-gray-600">

*Spécifier la version est obligatoire.*

*Le `$schema` permet de valider le fichier et d'avoir l'autocomplétion.*

</div>

---
transition: slide-up
level: 2
layout: section
---

## La partie "settings"

<div class="mt-10"></div>

Pour définir les réglages disponibles pour les blocs au niveau global

```json{2-4}
{
    "settings": {
        // réglages globaux
    },
}
```

ou au niveau des blocs pour les réglages spécifiques

```json{2-7}
{
    "settings": {
        // réglages globaux
        "blocks": {
            // réglages par bloc
        }
    },
}
```

---
transition: slide-up
level: 2
---

```json
{
    "settings": {
        "color": {
            "palette": [
                {
                    "name": "Black",
                    "slug": "black",
                    "color": "#000000"
                },
            ]
        },
        "blocks": {
            "core/paragraph": {
                "color": {
                    "palette": [
                        {
                            "name": "Red",
                            "slug": "red",
                            "color": "#ff0000"
                        }
                    ]
                }
            }
        }
    }
}
```

---
transition: slide-up
level: 2
---

## Le systeme va donc générer des variables CSS propres à chaque bloc.

<div class="mt-3"></div>

```css
body {
    --wp--preset--color--black: #000000;
}

.wp-block-paragraph {
    --wp--preset--color--red: #ff0000;
}
```

<img src="/assets/media/settings.png" class="w-80 mx-auto mt-10 shadow" />


---
transition: slide-up
level: 2
layout: section
---

## La partie "styles"

<div class="mt-10"></div>

### Pour définir les styles par défaut.

```json{2}
{
    "styles": {},
}
```

Comme pour la partie settings, nous avons des styles globaux et ensuite nous pouvons affiner par élements et blocs.

<div class="mt-10"></div>

### Ce sont des styles par defaut. Vous pouvez les modifier dans l'interface Gutenberg au moment de l'édition.

---
transition: slide-up
level: 2
---

## Premier niveau de styles

```json
{
    "styles": {
        "border": {
            ...
        },
        "filter": {
            "duotone": "value"
        },
        "color": {
            "background": "value",
            "gradient": "value",
            "text": "value"
        },
        "spacing": {
            "blockGap": "value",
            "margin": {},
            "padding": {}
        },
        "typography": {}
    },
    ...
}
```

---
transition: slide-up
level: 2
---

## Le style pour les éléments

<div class="mt-10"></div>

```json
{
    "styles": {
        ...
        "link": {
                "border": {},
                "color": {},
                "spacing": {},
                "typography": {}
            },
            "h1": {},
            "h2": {},
            "h3": {},
            "h4": {},
            "h5": {},
            "h6": {}
        }
    },
    ...
}
```

---
transition: slide-up
level: 2
---

## Le style pour les blocs

<div class="mt-10"></div>

```json
{
    "styles": {
        ...
       "blocks": {
            "core/group": {
                "border": {},
                "color": {},
                "spacing": {},
                "typography": {},
                "elements": {
                    "link": {},
                    "h1": {},
                    "h2": {},
                    ...
                }
            },
            "etc": {}
        }
}
```

---
transition: slide-up
level: 2
layout: section
---

## Pour les styles, la bonne pratique est de reprendre les variables générées par la partie settings.

<div class="mt-10"></div>

```json
{
    "styles": {
        "color": {
            "background": "var(--wp--preset--color--black)",
            "text": "var(--wp--preset--color--white)"
        }
    }
}
```

---
transition: slide-up
level: 2
layout: section
---

# Quelques exemples de réglages

---
transition: slide-up
level: 2
layout: section
---

## Layout

Quand le parent du bloc est en mode ```"layout":{"type":"constrained"}```.

```json
"layout": {
   "contentSize": "650px",
   "wideSize": "1200px"
  },
```

- contentSize : taille du contenu par défaut
- wideSize : taille du contenu en mode "wide"
- Reste le mode "full" qui prend toute la largeur de l'écran.

<!-- <img src="/assets/media/layout-settings.png" class="w-50 mx-auto mt-1 shadow" /> -->

---
transition: slide-up
level: 2
layout: section
---

## Typography (fontFamilies)

```json
"typography": {
   "dropCap": false,
   "fluid": true,
   "fontFamilies": [
    {
     "fontFace": [
      {
       "fontFamily": "DM Sans",
       "fontStretch": "normal",
       "fontStyle": "normal",
       "fontWeight": "400",
       "src": [
        "file:./assets/fonts/dm-sans/DMSans-Regular.woff2"
       ]
      },
      ...
     ],
     "fontFamily": "\"DM Sans\", sans-serif",
     "name": "DM Sans",
     "slug": "dm-sans"
    },
   ]
  ...
}
```


---
transition: slide-up
level: 2
layout: section
---

## La partie "fontFamilies" permet d'utiliser la Font API.

- Première chose, on retrouve les polices dans l'éditeur pour les éléments. Plutôt pratique :D
- La Font API charge la police uniquement si elle est utilisée ! Top pour la performance.

*Attention fonctionne uniquement avec des polices locales.*

### <twemoji-rocket class="w-10 h-10"/> 6.4 arrivée de la Font Library

---
transition: slide-up
level: 2
layout: section
---

## Typography (fontSizes)

Tips => fluid: true

```json
"typography": {
   "dropCap": false,
   "fluid": true,
   "fontFamilies": [
    {...},
   "fontSizes": [
    {
     "fluid": {
      "min": "0.875rem",
      "max": "1rem"
     },
     "size": "1rem",
     "slug": "small"
    },
    ...
   ]
```

---
transition: slide-up
level: 2
layout: section
---


## La partie "fontSizes"

- Comme pour le reste, on retrouve les tailles de polices dans l'éditeur pour les éléments.
- On peut utiliser des tailles fluides (min et max). Pour s'adapter à la taille de l'écran.

Génère un code dans ce style :

```css
--wp--preset--font-size--medium: clamp(0.9rem, 0.9rem + ((1vw - 0.48rem) * 0.577), 1.2rem);
```

---
transition: slide-up
level: 2
layout: section
---

## Root padding

Permet de gérer le padding des blocs globalement.

```json
{
    "settings": {
        "useRootPaddingAwareAlignments": true
    },
    "styles": {
        "spacing": {
            "padding": {
                "top": "0px",
                "right": "2rem",
                "bottom": "0px",
                "left": "2rem"
            }
        }
    }
}
```

```css
.has-global-padding > .alignfull {
  margin-right: calc(var(--wp--style--root--padding-right) * -1);
  margin-left: calc(var(--wp--style--root--padding-left) * -1);
}
```

---
transition: slide-up
level: 2
layout: section
---

# Trop compliqué le json !


---
transition: slide-up
level: 2
layout: section
---

# Méthodes alternatives

<div class="mt-10"></div>

Pour les réglages, il faut passer obligatoirement par le fichier json. Pas le choix !
Il faut donc se former un minimum au format json et aux valeurs possibles.

Par contre, pour le styles, vous pouvez utiliser l'interface "Styles" de l'éditeur de site.
Faire vos styles pour les éléments et les blocs et ensuite exporter le fichier json.

---
transition: slide-up
level: 2
layout: section
---

<img src="/assets/media/styles.gif" class="mx-auto shadow" />

---
transition: slide-up
level: 2
layout: section
---

<img src="/assets/media/stylebook.gif" class="mx-auto shadow" />

---
transition: slide-up
level: 2
layout: section
---

## Ou vous pouvez utiliser des generateurs de theme.json

Exemple :
- <https://wpturbo.dev/generators/theme-json/>
- <https://www.gutenberg-devtools.com/generator/themejson-support>
---
transition: slide-left
level: 2
layout: section
---

# Dernière chose sur le theme.json

<div class="mt-10"></div>

Passez en mode debug pour éviter le cache en mode developpement.

```php
define('WP_DEBUG', true);
```

---
transition: slide-up
level: 2
layout: section
---

# Les compositions (patterns)

---
transition: slide-up
level: 2
layout: section
---

# Pour moi, c'est un élément qui change tout !

<div class="mt-10"></div>

## Sans les patterns, Gutenberg et le FSE seraient moins fun !

---
transition: slide-up
level: 2
layout: section
---

Les patterns sont des assemblages de blocs déjà stylisés. Ils sont disponibles dans le sélecteur de blocs > Compositions.

Permet à un utilisateur de créer un contenu rapidement et de façon harmonieuse.

<img src="/assets/media/pattern-exemple.png" class="w-134 mx-auto mt-10 shadow" />

---
transition: slide-up
level: 2
layout: section
---

## Simple à créer et facile à utiliser

- Créer un pattern est plutôt accessible.
- Directement disponible dans le sélecteur (inserter).
- Preview du pattern dans le sélecteur.
- Inséré en un clic.
- Possibilité de le synchroniser pour modifier le pattern en un seul endroit.

---
transition: slide-up
level: 2
layout: section
---

## Fichiers PHP avec des commentaires (obligatoire)

```php
<?php
/**
 * Title: Hidden 404
 * Slug: trio/hidden-404
 * Inserter: no
 */
?>
```

**Inserter: no** permet de ne pas afficher le pattern dans le sélecteur de blocs.

<div class="mt-10"></div>

<https://developer.wordpress.org/block-editor/reference-guides/block-api/block-patterns/#register_block_pattern>


---
transition: slide-up
level: 2
layout: section
---

# Des fichier PHP mais attention !

Oui, il est possible de mettre du code php dans les patterns mais dès qu'il est incorporé dans un contenu, il est transformé en HTML. Plus de partie dynamique !

Pareil, si il est dans un template ou un part. Si vous éditez le contenu de l'élément, le php est automatiquement transformé en statique (HTML).

Exemple : j'ai un pattern dans le fichier du footer dans mon thème. Si j'édite le footer, le pattern est transformé en HTML. Donc si j'ai du texte avec ```__('mon texte', 'domaine');```. Il devient mon ```mon text``` et ne sera pas traduit.


---
transition: slide-up
level: 2
layout: section
---

# Autoload

<div class="mt-10"></div>

Les fichiers déposés dans ```/patterns``` sont disponibles automatiquement dans le sélecteur de composition.

---
transition: slide-up
level: 2
layout: section
---

# Catégories

<div class="mt-10"></div>
On peut utiliser les catégories existantes :
Buttons, Columns, Featured, Gallery, Text, About, Call to action, Contact, Footers, Headers...

ou en créer pour notre thème.

```php
if ( function_exists( 'register_block_pattern_category' ) ) {
    register_block_pattern_category(
      'mycategory',
      array(
            'label' => __( 'My Category', 'text-domain' ),
            'description' => __( 'Theme and more', 'text-domain' ),
       )
   );
}
```

---
transition: slide-up
level: 2
layout: section
---

# Les patterns synchronisés

<div class="mt-10"></div>

Si un pattern est utilisé dans plusieurs contenus, il est possible de le synchroniser.
Pour le modifier à un seul endroit et que les modifications soient répercutées partout.

---
transition: slide-up
level: 2
layout: section
---

<img src="/assets/media/pattern-sync.gif" class="w-180 mx-auto shadow" />

---
transition: slide-up
level: 2
layout: section
---

# Pattern Directory

Il est possible de le désactiver.

```
add_filter( 'should_load_remote_block_patterns', '__return_false' );
```

---
transition: slide-up
level: 2
layout: section
---

# Lock

On peut verrouiller un pattern pour qu'il ne soit pas modifiable par l'utilisateur.
L'utilisateur peut uniquement éditer le contenu.

Évite les mauvaises manipulations.

Verrouillage possible via l'interface ou dans le fichier.

---
transition: slide-up
level: 2
---

<img src="/assets/media/lock.gif" class="w-160 mx-auto shadow" />

---
transition: slide-up
level: 2
layout: section
---

## Empêcher le déverrouillage par les éditeurs

```php
add_filter(
 'block_editor_settings_all',
 static function( $settings, $context ) {
  // Allow for the Editor role and above.
  $settings['canLockBlocks'] = current_user_can( 'delete_others_posts' );

  // Only enable for specific user(s).
  $user = wp_get_current_user();
  if ( in_array( $user->user_email, array( 'user@example.com' ), true ) ) {
   $settings['canLockBlocks'] = false;
  }

  // Disable for posts/pages.
  if ( $context->post && $context->post->post_type === 'page' ) {
   $settings['canLockBlocks'] = false;
  }

  return $settings;
 },
 10,
 2
);
```

---
transition: slide-left
level: 2
layout: section
---

## Limites des patterns

Une fois insérer dans le contenu, le pattern devient un simple bloc. Et donc on ne peut plus le modifier globalement.

Il n'y a pas de solution simple pour modifier en masse des patterns déjà inseré dans le contenu.

Alternative :

- Utiliser des blocs réutilisables
- Utiliser des Templates parts
- Utiliser des blocs


---
transition: slide-up
level: 2
layout: section
---

# Les templates

---
transition: slide-up
level: 2
layout: section
---

# Comme déjà mentionné, ils sont **100% HTML**.


---
transition: slide-up
level: 2
layout: section
---

# La hierarchie des templates reste la même

<div class="mt-10"></div>

## J'espère que vous connaissez la hiérarchie des templates de WordPress !

---
transition: slide-up
level: 2
layout: section
---

<img src="/assets/media/wordpress-hierarchie-des-fichiers-modeles-juillet-2022.png" class=" mx-auto w-[88%] shadow" />


---
transition: slide-up
level: 2
layout: section
---

# Il faut garder des templates assez minimalistes

<div class="mt-10"></div>

## Reporter les gros morceaux de code dans des patterns ou des templates parts.

---
transition: slide-up
level: 2
layout: section
---

```html
<!-- wp:template-part {"slug":"header","tagName":"header"} /-->

<!-- wp:group {"tagName":"main"} -->
<main class="wp-block-group">
    <!-- wp:group {"layout":{"type":"constrained"}} -->
    <div class="wp-block-group">

        <!-- wp:pattern {"slug":"prefix/hero"} /-->

        <!-- wp:post-title {"level":1} /-->
    </div>
    <!-- /wp:group -->

    <!-- wp:post-content {"layout":{"type":"constrained"}} /-->

    <!-- wp:template-part {"slug":"comments","tagName":"section"} /-->

</main>
<!-- /wp:group -->

<!-- wp:template-part {"slug":"footer","tagName":"footer"} /-->
```

---
transition: slide-left
level: 2
layout: section
---

## Exemple de code pour intégrer des patterns, template parts ou block

Pattern:
```html
<!-- wp:pattern {"slug":"prefix/hero"} /-->
```

Template part:
```html
<!-- wp:template-part {"slug":"header","tagName":"header"} /-->
```

Block:
```html
<!-- wp:gravityforms/form {"formId":"2","title":false,"description":false,"ajax":true,"inputPrimaryColor":"#204ce5"} /-->
```

---
transition: slide-up
level: 2
layout: section
---

# Les blocs

---
transition: slide-up
level: 2
layout: section
---

## Bloc statique ou dynamique ?

- Un bloc statique est un bloc qui une fois sauvé, le contenu est figé (statique) :
    - Un titre
    - Un paragraphe
    - Une image
    - Un bouton
    - ...

- Un bloc dynamique possède un rendu serveur. Une fonction PHP génère le contenu a afficher :
    - Liste de posts
    - Elements dynamiques

---
transition: slide-up
level: 2
layout: section
---

## Quand créer un bloc ?

- Quand on doit afficher un champ personnalisé (ACF)
- Si on veut créer un élément reutilisable sur plusieurs projets (FAQ, Carousel, ...)
- Quand on veut afficher un code HTML différent de la norme Gutenberg/FSE


---
transition: slide-up
level: 2
layout: section
---

## Comment créer un bloc ?

- Apprendre JavaScript, React JS !
- Installer Node JS, etc..
<div class="mt-10"></div>

```bash
npx @wordpress/create-block@latest todo-list
```
<div class="mt-10"></div>

## Clairement, pas à la porté de tout le monde ! :D

---
transition: slide-left
level: 2
layout: section
---

## Advanced Custom Fields

<div class="mt-10"></div>

ACF permet de créer des blocs assez facilement :

- Les blocs sont uniquement dynamiques.
- Les champs de réglages s'affichent dans la colonne de droite de l'éditeur.
- L'expérience est pas aussi bonne que les blocs natifs mais ça fait le job.

**Par contre, cela créer une dépendance avec ACF.**

---
transition: slide-up
level: 2
layout: section
---

# i18n et le FSE


---
transition: slide-up
level: 2
layout: section
---

# Pas encore natif.

Prévu dans la phase 4 de la feuille de route à long terme.


---
transition: slide-up
level: 2
layout: section
---

# Polylang

Pas géré. Gère uniquement les traductions des contenus. Pas des templates.

---
transition: slide-up
level: 2
layout: section
---

## J'ajoute des templates avec un suffixe de langue

Exemple : page-fr.html

Et j'ajoute des templates dans le tableau des templates recherchés par WordPress.

```php
add_filter('frontpage_template_hierarchy', 'add_language_templates', 10, 1);
add_filter('home_template_hierarchy', 'add_language_templates', 10, 1);
add_filter('index_template_hierarchy', 'add_language_templates', 10, 1);
add_filter('page_template_hierarchy', 'add_language_templates', 10, 1);
...
```

---
transition: slide-up
level: 2
layout: section
---

## Mon hack pour Polylang

```php
function add_language_templates($template_file)
{
  // new template files array
  $template_file_lg = [];
  // get current language
  $lang = apply_filters('gm_current_language', null);
  // template defined in editor
  $template = get_page_template_slug();
  if($template) {
    $template_file[] = $template;
  }
  foreach ($template_file as $key => $value) {
    // add before template file name with the lang pattern = index-{lang}.php
    if ($lang !== '') {
      $template_file_lg[] = str_replace('.php', '-' . $lang . '.php', $value);
    }
    $template_file_lg[] = $value;
  }
  if ($lang !== '') {
    $template_file_lg[] = 'index-' . $lang . '.php';
  }
  $template_file_lg[] = 'index.php';
  return $template_file_lg;
}
```


---
transition: slide-up
level: 2
layout: section
---

# WPML

## Prend en charge le FSE !

Gère la traduction des templates, pattern, block, navigation, etc..

Par contre, il ne trouve pas les éléments fichiers. Il faut modifier et sauver en base pour les voir disponibles dans l'interface de traduction.

Pas simple à gérer.

---
transition: slide-left
level: 2
layout: section
---

<img src="/assets/media/wpml.png" class="w-200 mx-auto shadow" />


---
transition: slide-up
level: 2
layout: section
---

# Les librairies et ressources


---
transition: slide-up
level: 2
layout: section
---

## Ressources

Documentation officielle : <https://developer.wordpress.org/block-editor/>

Sites :

- <https://fullsiteediting.com>
- <https://gutenberg.10up.com/>


---
transition: slide-up
level: 2
layout: section
---


## Block Library :

- <https://wordpress.org/plugins/layout-grid/>
- <https://github.com/godaddy-wordpress/coblocks>

## Thèmes :

- <https://olliewp.com/>
- <https://generateblocks.com/>
- <https://www.kadencewp.com/blog/introducing-blocks-3/>
- <https://wpspectra.com/>

## Figma :

- <https://johannes-wp.com/>


---
transition: slide-up
level: 2
layout: section
---

## À venir

Le prochain thème par défaut de WordPress (6.4) :

<https://make.wordpress.org/core/2023/08/24/introducing-twenty-twenty-four/>


---
transition: slide-up
---

<div class="flex items-center gap-10 h-full">
<div class="flex-1">

# Merci !
</div>
<div class="flex-1">
<img src="/assets/media/wapuu-surf-1.webp" class="w-80" />
</div>
</div>


---
---
<div class="flex flex-col justify-center items-center h-full">

<img src="/assets/media/qr.png" class="w-80" />

https://wp-biarritz-23.goodmotion.fr

</div>
