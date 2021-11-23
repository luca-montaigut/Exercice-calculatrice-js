## Calculatrice JS

Pour cet exercice, le fichier HTML et le CSS sont fournis, vous n'avez pas le droit de les modifier directement sans Javascript.

Faire fonctionner la calculette à télécharger ici : https://github.com/luca-montaigut/Exercice-calculatrice-js

<img src="./preview.png" alt="drawing" width="400"/>

Note :

- si vous avez un doute sur un comportement, essayez sur la calculatrice de votre pc ;)
- l'utilisation de la fonction `eval` est formellement interdite, c'est de toute façon une fonction [qui ne devrait jamais être utilisée.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval#Never_use_eval!)
- L'exercice est sur 10, chaque étape franchie vous rapportera **1 point**

### Etape 1 :

Ajouter un évènement (`addEventListener`) sur chacun des boutons numériques pour détecter un clic de l'utilisateur. Afficher la valeur dans le champ du haut lorsque l'on **clique** sur une valeur numérique. Pensez à conserver la valeur affichée (`displayValue`) quelques part, vous risquez d'en avoir besoin plus tard.

### Etape 2 :

Faite en sorte de pouvoir taper des nombres et pas seulement des chiffres dans le champs du haut (maximum 9 chiffres). Attention, si vous tapez un `0` au départ, il ne doit pas y avoir plusieurs 0 qui s'affichent.

### Etape 3 :

Créer 4 fonctions :

- `add`
- `subtract`
- `mulitply`
- `divide`

Chacune prenant 2 nombres en argument et qui renvoie (`return`) le résultat de leur opération respective. Vous pouvez essayer vos fonctions dans la console du navigateur.

### Etape 4 :

Créer une fonction `operate` qui prend en argument 2 nombres et un opérateur. Cette fonction doit additionner, soustraire, multiplier ou diviser en fonction de l'opérateur qui lui est passé en argument (ceci grâce aux fonctions précédemment créées). Vous pouvez tester votre fonction dans la console du navigateur.

### Etape 5 :

Faite fonctionner la calculette ! Stocker la première valeur entrée par un utilisateur, puis stocker l'opérateur, puis la seconde valeur et appeler `operate` avec ces valeurs lorsque l'utilisateur clique sur la touche `=`. Afficher le résultat dans le champ du haut (le `displayValue`)

A vous de trouver comment stocker les valeurs et appeler la fonction avec.

### Etape 6 :

A tout moment l'utilisateur peut cliquer sur `AC` et la calculatrice retourne à son état initial. Assurez-vous de bien annuler toutes les précédentes interactions de l'utilisateur.

### Etape 7 :

Vous devez pouvoir enchainer plusieurs opérations et avoir le bon résultat, par exemple : `15 + 3 - 6 * 2 =` doit donner `24`. **Votre calculatrice ne doit pas évalué plus d'une paire de nombre à la fois. Si vous entrez un nombre, puis un opérateur, puis un autre nombre alors le résultat devra être affiché SI la prochaine entrée est un opérateur. Le résultat devra être utilisé comme première entrée du prochain calcul.**

### Etape 8 :

Chasse au bugs.
Si l'utilisateur essaye de diviser par `0`, vous devez afficher `not valid` dans le champ du haut (`displayValue`).

Si le résultat de l'opération fait plus de 9 chiffres, afficher `too long!` .

Gérer le cas où un utilisateur tape plusieurs fois d'affiler sur un opérateur ou s'il tape sur `=` sans avoir rentré de second nombre.

Votre calculatrice ne doit jamais crasher.

### Etape 9 :

Faite fonctionner le bouton pour avoir des nombres négatifs.

### Etape 10 :

Fait également fonctionner la calculatrice avec le clavier (vous pouvez utiliser `Alt` sur windows/linux ou `⌥` Option sur mac pour la touche des nombres négatifs)
