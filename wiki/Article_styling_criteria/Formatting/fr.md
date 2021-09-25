---
outdated: true
outdated_since: a92869bad198adeb411099cc45da9aaf71893c2a
---

# Mise en forme

*Pour les normes de rédaction, voir : [Critères de style des articles/Rédaction](../Writing)*

*Note : Cet article utilise [RFC 2119](https://tools.ietf.org/html/rfc2119) pour décrire les niveaux d'exigence.*

## Locales

Vous trouverez ci-dessous la liste des langues correctement supportées pour le wiki :

| Nom du fichier | Nom en Français | Écriture native |
| :-- | :-- | :-- |
| `en.md` | Anglais | English |
| `ar.md` | Arabe | اَلْعَرَبِيَّةُ |
| `be.md` | Biélorusse | Беларуская мова |
| `bg.md` | Bulgare | Български |
| `cs.md` | Tchèque | Česky |
| `da.md` | Danois | Dansk |
| `de.md` | Allemand | Deutsch |
| `gr.md` | Grec | Ελληνικά |
| `es.md` | Espagnol | Español |
| `fi.md` | Finlandais | Suomi |
| `fr.md` | Français | Français |
| `hu.md` | Hongrois | Magyar |
| `id.md` | Indonésien | Bahasa Indonesia |
| `it.md` | Italien | Italiano |
| `ja.md` | Japonais | 日本語 |
| `ko.md` | Coréen | 한국어 |
| `nl.md` | Néerlandais | Nederlands |
| `no.md` | Norvégien | Norsk |
| `pl.md` | Polonais | Polski |
| `pt.md` | Portugais | Português |
| `pt-br.md` | Portugais du Brésil | Português (Brasil) |
| `ro.md` | Roumain | Română |
| `ru.md` | Russe | Русский |
| `sk.md` | Slovaque | Slovenčina |
| `sv.md` | Suédois | Svenska |
| `th.md` | Thaïlandais | ไทย |
| `tr.md` | Turc | Türkçe |
| `uk.md` | Ukrainien | Українська мова |
| `vi.md` | Vietnamien | Tiếng Việt |
| `zh.md` | Chinois (simplifié) | 简体中文 |
| `zh-tw.md` | Chinois traditionnel (Taïwan) | 繁體中文（台灣） |

*Note : Le site web donnera aux lecteurs la version d'un article dans la langue qu'ils ont choisie. Si celle-ci n'est pas disponible, la version anglaise sera donnée.*

### Parité de contenu

Les traductions sont soumises à une stricte parité de contenu avec leur article anglais, ce qui signifie qu'elles doivent avoir le même message, indépendamment de la grammaire et de la syntaxe. Toute modification du sens des traductions doit être accompagnée de modifications équivalentes de l'article anglais.

Dans certains cas, il est permis de différer le contenu :

- Articles rédigés à l'origine dans une langue autre que l'anglais (dans ce cas, l'anglais doit faire office de traduction)
- Explications de mots anglais qui sont des termes courants dans la communauté d'osu!
- Liens externes
- Tags
- Explications spécifiques aux sous-communautés

## Page de garde

La page de garde doit être placée tout en haut du fichier. Elle est écrite en [YAML](https://fr.wikipedia.org/wiki/YAML#Exemple) et décrit des informations supplémentaires sur l'article. Elle doit être entourée de trois traits d'union (`---`) sur les lignes qui la précèdent et la suivent, et d'une ligne vide avant l'intitulé du titre.

### Articles nécessitant une aide

*Note : Évitez de traduire les articles anglais avec cette balise. En outre, cette balise doit être ajoutée lorsque la traduction nécessite un nettoyage propre.*

La balise `needs_cleanup` peut être ajoutée aux articles qui nécessitent une réécriture ou une aide à la mise en forme. Il est également acceptable d'ouvrir un problème sur GitHub dans ce but. Cette balise doit être écrite comme indiqué ci-dessous :

```yaml
needs_cleanup: true
```

Lorsque vous ajoutez cette balise à un article, vous devez également ajouter des [commentaires](#commentaires) pour expliquer ce qu'il faut faire pour supprimer la balise.

### Articles obsolètes

*Note : Évitez de traduire les articles anglais avec cette balise. Si l'article anglais a cette balise, la traduction doit également avoir cette balise*.

Les articles traduits qui sont obsolètes doivent utiliser la balise `outdated` lorsque la variante anglaise est mise à jour. Les articles anglais peuvent également devenir obsolètes lorsque le contenu qu'ils contiennent est trompeur ou n'est plus pertinent. Cette balise doit être écrite comme indiqué ci-dessous :

```yaml
outdated: true
```

Lorsque vous ajoutez cette balise à un article, vous devez également ajouter des [commentaires](#commentaires) pour expliquer ce qui doit être mis à jour pour supprimer la balise.

### Tags

Les tags aident le moteur de recherche du site à mieux rechercher les articles. Les balises doivent être rédigées dans la même langue que l'article et inclure la liste originale des balises. Les tags doivent utiliser des lettres minuscules, le cas échéant.

Par exemple, un article intitulé "Discussions sur la beatmap" peut inclure les balises suivantes :

```yaml
tags:
  - discussions sur la beatmap
  - modding V2
  - MV2
```

### Traductions sans révision

*Note : Les responsables du wiki détermineront et appliqueront cette marque avant la fusion.*

Il arrive que des traductions soient ajoutées au wiki sans être révisées par d'autres personnes de langue maternelle. Dans ce cas, la marque `no_native_review` est ajoutée pour faire savoir aux futurs traducteurs qu'il faudra peut-être la vérifier à nouveau. Cette balise doit être écrite comme indiqué ci-dessous :

```yaml
no_native_review: true
```

## Désignation de l'article

*Voir aussi : [Noms de dossiers](#noms-de-dossiers) et [Titres](#titres)*

Les titres des articles doivent être au singulier et utiliser la casse. Pour plus de détails, consulter l'[article sur les conventions de dénomination de Wikipédia](https://en.wikipedia.org/wiki/Wikipedia:Naming_conventions_(plurals)).

Les titres des articles doivent correspondre au nom du dossier dans lequel ils se trouvent (les espaces peuvent remplacer les traits de soulignement (`_`) le cas échéant). Si le nom du dossier change, le titre de l'article doit être modifié en conséquence et vice versa.

---

Les articles sur les concours et les tournois constituent une exception. Le nom du dossier doit utiliser des abréviations, des acronymes ou des initiales. Le titre de l'article doit être le nom complet du concours ou du tournoi.

## Structure des dossiers et des fichiers

### Noms de dossiers

*Voir aussi : [Désignation de l'article](#désignation-de-l'article)*

Les noms de dossiers doivent être en anglais et respecter la casse.

Les noms de dossiers ne doivent utiliser que ces caractères :

- les lettres majuscules et minuscules
- les nombres
- les traits de soulignement (`_`)
- les traits d'union (`-`)
- les points d'exclamation (`!`)

### Noms des fichiers d'articles

Le nom du fichier d'un article peut être trouvé dans la colonne `Nom du fichier` de la section [locales](#locales). L'emplacement d'un article traduit doit être placé dans le même dossier que l'article anglais.

### Articles d'index

Les articles d'index doivent être créés si le dossier est destiné à contenir uniquement d'autres articles, et doivent contenir une liste d'articles qui se trouvent dans son propre dossier. Ils peuvent également contenir d'autres informations, telles qu'un paragraphe principal ou des descriptions des articles liés.

### Articles de désambiguïsation

Les articles de [désambiguïsation](/wiki/Disambiguation) doivent être placés dans le dossier `/wiki/Disambiguation`. La page principale doit être mise à jour pour les inclure. Voir l'exemple de [Désambiguïsation/Mod](/wiki/Disambiguation/Mod).

Les redirections doivent être mises à jour afin que les mots clés ambigus soient redirigés vers l'article de désambiguïsation.

Les articles liés à partir d'un article de désambiguïsation doivent avoir une hatnote [pour d'autres utilisations](#for-other-uses).

## HTML

Le HTML ne doit pas être utilisé, à l'exception des [commentaires](#commentaires). La structure de l'article doit être refaite si du HTML est utilisé.

### Commentaires

Les commentaires HTML doivent être utilisés pour marquer les tâches à faire, mais peuvent également servir à annoter du texte. Ils doivent être placés sur leur propre ligne, mais peuvent être placés en ligne dans un paragraphe. S'ils sont placés en ligne, le début du commentaire ne doit pas comporter d'espace.

Mauvais exemple :

```markdown
Les commentaires HTML <!-- TODO explain HTML comments --> devraient être utilisés pour marquer les tâches à faire ou annoter le texte.
```

Un bon exemple :

```markdown
Les commentaires HTML<!-- TODO explain HTML comments --> devraient être utilisés pour marquer les tâches à faire ou annoter le texte.
```

*Note : Ne pas traduire les commentaires, car ces derniers sont destinés à des changements sur la version anglaise, il n'y a pas lieu de les traduire.*

## Édition

### Séquence de fin de ligne

*Attention : Si vous téléchargez des fichiers Markdown en utilisant `CRLF` (retour chariot et saut de ligne) via GitHub, ces fichiers utiliseront `CRLF`. Pour éviter cela, définissez la fin de ligne à `LF` (saut de ligne) avant de télécharger.*

Les fichiers Markdown doivent être enregistrés en utilisant la séquence de fin de ligne `LF`.

### Espacement

La syntaxe Markdown doit être espacée si nécessaire. Toutefois, les titres des articles sont analysés en tant que texte brut et ne doivent donc pas être espacés.

### Paragraphes

Chaque paragraphe doit être suivi d'une ligne vide.

### Sauts de ligne

Les sauts de ligne doivent utiliser une barre oblique inversée (`\`).

Les sauts de ligne doivent être utilisés avec parcimonie.

## Hatnote

*À ne pas confondre avec [Note](#note).*

Les hatnotes sont de courtes notes placées en haut d'un article ou d'une section pour aider les lecteurs à naviguer vers des articles connexes ou les informer sur des sujets connexes.

Les hatnotes doivent être en italique et placées immédiatement après le titre. Si plusieurs hatnotes sont utilisées, elles doivent figurer dans le même paragraphe et être séparées par un saut de ligne.

### Page principale

La hatnote *Page principale* dirige le lecteur vers l'article principal d'un sujet. Lorsque cette hatnote est utilisée, elle implique que la section sur laquelle elle se trouve est un résumé de ce dont traite la page liée. Cette hatnote ne doit comporter qu'un seul lien. Elle doit être formatée comme suit :

```markdown
*Page principale : {article}*

*Pages principales : {article} et {article}*
```

### Voir aussi

Les hatnotes *Voir aussi* suggèrent aux lecteurs d'autres points d'intérêt d'un article ou d'une section donnée. Elles doivent être formatées comme suit :

```markdown
*Voir aussi : {article}*

*Voir aussi : {article} et {article}*
```

### Pour voir

Les hatnotes *Pour voir* sont similaires aux hatnotes *Voir aussi*, mais sont généralement plus descriptives et directes. Cette hatnote peut utiliser plus d'un lien si nécessaire. Elles doivent être formatées comme suit :

```markdown
*Pour {description}, voir : {article}`*

*Pour {description}, voir : {article} et {article}`*
```

### À ne pas confondre avec

Les hatnotes *À ne pas confondre avec* aident à distinguer les titres ou sections d'articles ambigus ou mal compris. Elles peuvent utiliser plus d'un lien si nécessaire. Elles doivent être formatées comme suit :

```markdown
*À ne pas confondre avec {article}.*

*À ne pas confondre avec {article} ou {article}.*
```

### Pour d'autres utilisations

Les hatnotes *Pour d'autres utilisations* sont similaires aux hatnotes *À ne pas confondre avec*, mais renvoient directement à l'article de désambiguïsation (#articles-de-désambiguïsation). Elles doivent uniquement renvoyer à l'article de désambiguïsation. Elles doivent être formatées comme suit :

```markdown
*Pour d'autres utilisations, voir {article de désambiguïsation}.*
```

## Note

*À ne pas confondre avec [Hatnote](#hatnote).*

Une note doit être placée à l'endroit approprié dans une section, mais doit commencer le paragraphe et utiliser l'italique. Les notes peuvent contenir des caractères gras lorsque cela est approprié, mais ils doivent être limités autant que possible. Les notes doivent être rédigées sous forme de phrases complètes. Ainsi, contrairement à la plupart des [hatnotes](#hatnote), elles doivent utiliser un point (`.`) ou un point d'exclamation (`!`) si nécessaire. Tout ce qui se trouve dans le même paragraphe qu'une note doit également être en italique. Elles doivent être formatées comme suit :

```markdown
*Note : {note}.*

*Remarque : {Remarque}.*

*Attention : {attention}.*

*Avertissement : {avertissement}.*
```

- `Note` doit être utilisé pour les détails factuels ou anecdotiques.
- `Remarque` doit être utilisé pour des rappels ou pour attirer l'attention sur quelque chose dont le lecteur doit être informé.
- `Attention` doit être utilisé pour avertir le lecteur afin d'éviter des malentendus.
- `Avertissement` doit être utilisé pour avertir le lecteur que des mesures peuvent être prises à son encontre.

## Mise en valeur

### Gras

Les caractères gras doivent utiliser des doubles astérisques (`**`).

Les paragraphes de tête peuvent mettre en gras la première occurrence du titre de l'article.

### Italiques

Les italiques doivent utiliser des astérisques simples (`*`).

Les noms des œuvres ou des jeux vidéo doivent être en italique. osu! (le jeu) est exempté de cette règle.

La première occurrence d'une abréviation, d'un acronyme ou d'un sigle peut être mise en italique.

L'italique peut également être utilisé pour accenter un ou plusieurs mots ou faciliter la lecture.

## Rubriques

Toutes les rubriques doivent respecter la casse.

Les rubriques doivent utiliser le style [ATX (dièse)](https://github.github.com/gfm/#atx-headings) et doivent être précédées et suivies d'une ligne vide. Le titre est une exception lorsqu'il se trouve sur la première ligne. Dans ce cas, il suffit de laisser une ligne vide après le titre.

Les rubriques ne doivent pas dépasser un niveau d'en-tête de 5 et ne doivent pas être utilisées pour styliser ou formater le texte.

### Titres

*Voir aussi : [Désignation de l'article](#désignation-de-l'article)*

*Attention : Les titres sont analysés en tant que texte brut ; ils ne doivent pas être espacés.*

Le premier titre de tous les articles doit être un titre de niveau 1, c'est-à-dire le titre de l'article. Tous les titres suivants doivent être des [titres de section](#sections). Les titres ne doivent pas contenir de formatage, de liens ou d'images.

L'intitulé du titre doit figurer sur la première ligne, sauf si la [page de garde](#page-de-garde) est utilisée. Si c'est le cas, l'intitulé du titre doit être placé à la suite de celui-ci et une ligne vide doit précéder l'intitulé du titre.

### Sections

Les titres de section doivent utiliser les niveaux 2 à 5. L'en-tête de section qui précède le [titre](#titres) doit être un en-tête de niveau 2. Contrairement aux titres, les titres de section peuvent comporter de petites icônes d'image.

Les titres de section ne doivent pas sauter un niveau de titre (c'est-à-dire ne pas passer d'un titre de niveau 2 à un titre de niveau 4) et ne doivent pas contenir de formatage ou de liens.

*Remarque : Sur le site web, les niveaux de rubrique 4 et 5 n'apparaîtront pas dans la table des matières. Ils ne peuvent pas non plus faire l'objet d'un lien direct.*

## Listes

Les listes ne doivent pas dépasser 4 niveaux d'indentation et ne doivent pas comporter de ligne vide entre chaque élément.

Pour les listes imbriquées, les puces ou les chiffres doivent être alignés sur le contenu des éléments de leurs listes parentes.

L'exemple suivant a été fait de manière incorrecte (notez l'espacement avant la puce) :

```markdown
1. Faire voler un cerf-volant
  - Ne faites pas voler un cerf-volant s'il pleut.
```

L'exemple suivant a été réalisé correctement :

```markdown
1. Faire voler un cerf-volant
   - Ne faites pas voler un cerf-volant s'il pleut.
```

### À puces

Les listes à puces doivent utiliser un trait d'union (`-`) et être suivies d'un espace. (Exemple illustré ci-dessous.)

```markdown
- osu!
  - Cercles
    - Numéro du combo
    - Cercle d'approche
  - Slider
    - Cercles
    - Sliderbody
    - Slider ticks
  - Spinner
- osu!taiko
```

### Numérotée

Les chiffres d'une liste numérotée doivent être incrémentés pour représenter leur échelon.

```markdown
1. Téléchargez l'installateur d'osu!
2. Exécutez le programme d'installation.
   1. Pour modifier l'emplacement de l'installation, cliquez sur le texte situé sous la barre de progression.
   2. Le programme d'installation vous demandera de choisir un nouvel emplacement, choisissez le dossier d'installation.
3. osu! démarrera une fois l'installation terminée.
4. Se connecter.
```

### Mixte

La combinaison de listes à puces et de listes numérotées doit être faite avec parcimonie.

```markdown
1. Téléchargez un skin depuis les forums.
2. Chargez le fichier skin dans osu!
   - Si le fichier est un `.zip`, décompressez-le et déplacez le contenu dans le dossier `Skins/` (qui se trouve dans votre dossier d'installation d'osu!).
   - Si le fichier est un `.osk`, ouvrez-le sur votre bureau ou faites-le glisser dans le client du jeu.
3. Ouvrez osu!, s'il n'est pas ouvert, et sélectionnez le skin dans les options.
   - Cela a pu être fait si vous avez ouvert le fichier `.osk` ou si vous l'avez glissé dans le client du jeu.
```

## Code

Le balisage du code est un accent grave (`` ` ``). Pour mettre des accent grave dans le code, utilisez plutôt des accent grave doubles. Si l'accent grave se trouve au début ou à la fin, ajoutez un espace. (Exemple illustré ci-dessous.)

```markdown
`` ` ``
`` `Espace` ``
```

### Touches du clavier

*Remarque : Pour désigner la lettre elle-même, et non la touche du clavier, utilisez plutôt des guillemets.*

Lorsque vous représentez les touches du clavier, utilisez les majuscules pour les caractères uniques et les majuscules pour les modificateurs. Utilisez le symbole plus (`+`) (sans code) pour représenter les combinaisons de touches. (Exemple illustré ci-dessous).

```markdown
pippi s'écrit avec un "p" minuscule comme peppy.

Appuyez sur `Ctrl` + `O` pour ouvrir le dialogue d'ouverture.
```

Pour représenter un espace ou la barre d'espacement, utilisez `` `Espace` ``.

### Texte des boutons et des menus

Lorsque vous copiez le texte d'un menu ou d'un bouton, la casse des lettres doit être copiée telle qu'elle apparaît. (Exemple illustré ci-dessous.)

```markdown
Le bouton `osu!direct` est visible dans le menu principal sur le côté droit, si vous avez un tag osu!supporter actif.
```

### Noms de dossiers et de répertoires

Lors de la copie du nom d'un dossier ou d'un répertoire, la casse des lettres doit être copiée telle qu'elle apparaît, mais préférez les chemins en minuscules lorsque cela est possible. Les chemins d'accès aux répertoires ne doivent pas être absolus (c'est-à-dire qu'il ne faut pas commencer le nom du répertoire à partir de la lettre du lecteur ou du dossier racine). (Exemple illustré ci-dessous.)

```markdown
osu! est installé par défaut dans le dossier `AppData/Local`, sauf indication contraire lors de l'installation.
```

### Mots clés et commandes

Lorsque vous copiez un mot-clé ou une commande, la casse des lettres doit être copiée telle qu'elle apparaît ou telle qu'une personne la tape normalement. Le cas échéant, préférez les lettres minuscules. (Exemple illustré ci-dessous).

```markdown
Pour l'instant, les commandes `Name` et `Author` dans le fichier de configuration du skin (`skin.ini`) ne font rien.
```

### Noms de fichiers

Lorsque vous copiez le nom d'un fichier, la casse des lettres doit être copiée telle qu'elle apparaît. Le cas échéant, préférez les lettres minuscules. (Exemple illustré ci-dessous).

```markdown
Pour jouer à osu!, double-cliquez sur l'icône `osu!.exe`.
```

### Extensions de fichiers

*Remarque : Les formats de fichiers (à ne pas confondre avec les extensions de fichiers) doivent être écrits en lettres majuscules sans le préfixe point (`.`).*

Les extensions de fichiers doivent être préfixées par un point (`.`) et être suivies de l'extension du fichier en lettres minuscules. (Exemple illustré ci-dessous.)

```markdown
Le format de fichier JPG (ou JPEG) porte l'extension `.jpg` (ou `.jpeg`).
```

### Canaux de discussion

Lorsque vous copiez le nom d'un canal de discussion, commencez par un dièse (`#`), suivi du nom du canal en lettres minuscules. (Exemple montré ci-dessous.)

```markdown
`#lobby` est l'endroit où vous pouvez faire de la publicité pour votre lobby multijoueur.
```

## Texte préformaté (blocs de code)

*Remarque : La coloration syntaxique pour le texte préformaté n'est pas encore implémentée sur le site web.*

Le texte préformaté (également connu sous le nom de blocs de code) doit être clôturé à l'aide de trois accent grave. Ils doivent définir l'identifiant de la langue pour la coloration syntaxique.

## Liens

Il existe deux types de liens : en ligne et de référence. Les liens en ligne ont deux styles.

Voici un exemple des deux styles en ligne :

```markdown
[Modificateurs de jeu](/wiki/Game_Modifiers)

<https://osu.ppy.sh/home>
```

Voici un exemple de style de référence :

```markdown
[Modificateurs de jeu][lien vers les mods de jeu]

[lien vers les mods de jeu]: /wiki/Game_Modifiers
```

---

Les liens doivent utiliser le style en ligne s'ils ne sont référencés qu'une seule fois. Le style en ligne entre crochets doit être évité. Les références aux liens de référence doivent être placées en bas de l'article.

### Liens internes

*Note : les liens internes sont des liens qui restent à l'intérieur du domaine `https://osu.ppy.sh/`.*

#### Liens Wiki

Tous les liens qui pointent vers un article wiki doivent commencer par `/wiki/` suivi du chemin pour arriver à l'article visé. Des liens relatifs peuvent également être utilisés. 
  
Voici quelques exemples :

```markdown
[FAQ](/wiki/FAQ)
[pippi](/wiki/Mascots#-pippi)
[Beatmaps](../)
[Pattern](./Pattern)
```

Les liens wiki ne doivent pas utiliser de redirections et ne doivent pas comporter de barre oblique de fin de ligne. (`/`).

Les mauvais exemples sont les suivants :

```markdown
[Critères de style des articles](/wiki/ASC)
[Developers](/wiki/Developers/)
[Developers](/wiki/Developers/#game-client-developers)
```

Voici de bons exemples :

```markdown
[Critères de style des articles](/wiki/Article_styling_criteria)
[Developers](/wiki/Developers)
[Developers](/wiki/Developers#game-client-developers)
```

*Remarque : ne pas traduire les liens entre parenthèses, sinon la redirection ne fonctionnera plus.*

##### Liens vers les sous-articles

Les liens Wiki qui pointent vers un sous-article doivent inclure le nom du dossier de l'article parent dans le texte du lien. Voir l'exemple suivant :

```markdown
*Voir aussi : [Beatmap Editor/Design](/wiki/Beatmap_Editor/Design)*
```

##### Liens de section

*Remarque : Sur le site web, les niveaux de rubrique 4 et 5 ne sont pas dotés de l'attribut id. Cela signifie qu'ils ne peuvent pas être liés directement.*

Les liens Wiki qui pointent vers une section d'un article peuvent utiliser le symbole du signe de section (`§`). Voir l'exemple suivant :

```markdown
*Pour les règles de timing, voir : [Ranking Criteria § Timing](/wiki/Ranking_Criteria#timing)*
```

#### Autres liens osu!

L'URL de la barre d'adresse de votre navigateur doit être copiée telle qu'elle est lorsqu'on crée un lien vers d'autres pages Web d'osu!. La partie `https://osu.ppy.sh` de l'URL doit être conservée.

##### Profils des utilisateurs

Tous les noms d'utilisateur doivent être liés à la première occurrence. Les autres occurrences sont facultatives, mais doivent être cohérentes tout au long de l'article pour tous les noms d'utilisateur. S'il est difficile de déterminer l'identifiant de l'utilisateur, il peut être ignoré.

Lorsque vous créez un lien vers un profil d'utilisateur, le numéro d'identification de l'utilisateur doit être utilisé. Utilisez le nouveau site web (`https://osu.ppy.sh/users/{username})`) pour obtenir l'id de l'utilisateur.

Le texte du lien de l'utilisateur doit être le nom actuel de l'utilisateur.

##### Difficultés

Lorsque vous créez un lien vers une difficulté, utilisez ce format pour le texte du lien :

```
{artist} - {title} ({creator}) [{difficuty_name}]
```

Le lien vers une beatmap doit effectivement mener à cette difficulté. Les URL des difficultés de la beatmap doivent être formatées comme suit :

```
https://osu.ppy.sh/beatmapsets/{BeatmapSetID}#{mode}/{BeatmapID}
```

Le nom de la difficulté peut être laissé en dehors du texte du lien, mais cela doit être cohérent dans tout l'article.

##### Beatmaps

Lorsque vous créez un lien vers une beatmap, utilisez ce format pour le texte du lien :

```
{artist} - {title} ({creator})
```

Toutes les URL des beatmaps doivent être formatées comme suit :

```
https://osu.ppy.sh/beatmapsets/{BeatmapSetID}
```

### Liens externes

*Remarque : Les liens externes font référence aux liens qui sortent du domaine `https://osu.ppy.sh/`.*

Le protocole `https` doit être utilisé, sauf si le site ne le prend pas en charge. Les liens externes doivent être des liens propres et directs vers une source réputée. Le texte du lien doit être le titre de la page à laquelle il renvoie. L'URL de la barre d'adresse de votre navigateur Web doit être copiée telle quelle pour les liens vers d'autres pages externes.

Il n'y a pas de différences visuelles entre les liens externes et les liens Web d'osu!. Pour cette raison, le nom du site web doit être inclus dans le texte du titre. Voir l'exemple suivant :

```markdown
*Pour plus d'informations sur la théorie musicale, voir : [Théorie de la musique](https://fr.wikipedia.org/wiki/Th%C3%A9orie_de_la_musique)*
```

## Images

Il existe deux types de liens d'image : en ligne et de référence. Exemples :

**Style en ligne :**

```markdown
![](/wiki/shared/flag/AU.gif)
```

**Style de référence :**

```markdown
![][flag_AU]

[flag_AU]: /wiki/shared/flag/AU.gif
```

Les images doivent utiliser le style de lien en ligne. Les références aux liens de référence doivent être placées en bas de l'article.

Les images doivent être placées dans un dossier nommé `img`, situé dans le dossier de l'article. Les images qui sont utilisées dans plusieurs articles doivent être stockées dans le dossier `/wiki/shared/`.

### Mise en cache des images

Les images du site web sont mises en cache pour une durée maximale de 60 jours. L'image mise en cache correspond à l'URL du lien de l'image.

Lors de la mise à jour d'une image, il faut soit changer le nom de l'image, soit ajouter une chaîne de requête à l'URL. Dans les deux cas, toutes les traductions liées à l'image mise à jour doivent également être mises à jour.

### Formats et qualité

Les images doivent utiliser le format JPG en qualité 8 (80 ou 80%, selon le programme). Si l'image contient de la transparence ou du texte qui doit être lisible, utilisez plutôt le format PNG. Si l'image contient une animation, le format GIF peut être utilisé ; cependant, il doit être utilisé avec parcimonie car il peut prendre plus de temps à charger ou être plus grand que la [taille maximale du fichier](#taille-du-fichier).

### Taille du fichier

Les images doivent être inférieures à 1 mégaoctet, sinon elles ne se chargeront pas. La réduction d'échelle et l'utilisation du format JPG à 80 % permettent presque toujours de respecter la taille limite.

Toutes les images doivent être optimisées autant que possible. Utilisez [jpeg-archive](https://github.com/danielgtaylor/jpeg-archive) pour compresser les images JPEG. Par souci de cohérence, utilisez la commande suivante pour jpeg-archive :

```sh
jpeg-recompress -am smallfry <input> <output>
```

Où `<input>` est le nom du fichier à compresser et `<output>` est le nom du fichier compressé.

### Noms de fichiers

*Attention : Les extensions de fichiers doivent utiliser des lettres minuscules, sinon le chargement échouera !*

Utilisez des traits d'union (`-`) pour espacer les mots. Lorsque vous nommez une image, le nom du fichier doit être significatif ou descriptif mais court.

### Mise en page et positionnement

*Remarque : il n'est actuellement pas possible de faire flotter une image ou de faire en sorte que le texte s'enroule autour d'elle.*

Les images sur le site web seront centrées lorsqu'elles se trouvent sur une seule ligne, par elles-mêmes. Sinon, elles seront placées en ligne avec le paragraphe. L'exemple suivant placera l'image au centre :

```markdown
L'installation d'osu! est facile. Tout d'abord, téléchargez le programme d'installation depuis la page de téléchargement.

![](img/download-page.jpg)

Localisez ensuite le programme d'installation et exécutez-le.
```

### Texte alternatif

Les images doivent être accompagnées d'un texte alternatif, sauf si elles ont un but décoratif.

### Légendes

Les images sont légendées sur le site web si elles remplissent ces conditions :

1. L'image est seule.
2. L'image n'est pas à l'intérieur d'un titre.
3. L'image a un titre.

Les légendes sont reprises dans le texte du titre, qui doit être en texte clair. Les images avec légendes sont également centrées avec l'image sur le site web.

### Largeur maximale de l'image

La largeur maximale de l'image sur le site correspond à la largeur du corps de l'article. Les images ne doivent pas avoir une largeur supérieure à 800 pixels.

### Annotation des images

Pour annoter des images, utilisez *Torus Regular*. Pour les caractères chinois, coréens et japonais, utilisez *Microsoft YaHei*.

Il faut éviter d'annoter les images, car il est difficile pour les traducteurs (et autres éditeurs) de les modifier.

#### Traduire des images annotées

Lors de la traduction d'images annotées, la version localisée de l'image doit être placée dans le même répertoire que la version originale (c'est-à-dire la version anglaise). Le nom de fichier d'une version localisée de l'image doit commencer par le nom de la version originale, suivi d'un tiret, puis du nom local (en lettres majuscules). Voir les exemples suivants :

- `hardrock-mod-vs-easy-mod.jpg` pour les Anglais
- `hardrock-mod-vs-easy-mod-DE.jpg` pour les Allemands
- `hardrock-mod-vs-easy-mod-ZH-TW.jpg` pour le Chinois Traditionnel
- `hardrock-mod-vs-easy-mod-FR.jpg` pour les Français

### Captures d'écran de gameplay

Toutes les captures d'écran de jeu doivent être faites dans la version stable, sauf si c'est pour une fonctionnalité spécifique qui n'est pas disponible dans la version stable. Vous devez utiliser la fonction de capture d'écran du jeu (`F12`).

#### Paramètres du client de jeu

*Note : Si vous ne voulez pas changer vos paramètres actuels pour le wiki, vous pouvez déplacer votre `osu!.<OrdinateurUtilisateur>.cfg` hors du dossier osu! et le remettre plus tard.*

Vous devez définir ces paramètres avant de prendre une capture d'écran du client de jeu (les paramètres non indiqués ci-dessous sont supposés être à leur valeur par défaut) :

- Langue : `Français`
- Préférer les métadonnées dans la langue d'origine : `Activé`
- Résolution: `1280x720`
- Mode plein écran : `Désactivé`
- Parallaxe : `Désactivé`
- Conseils sur les menus : `Désactivé`
- Arrière-plans saisonniers : `Jamais`
- Toujours afficher la superposition des touches : `Activé`
- Skin actuel : `Default` (Première option)

### Liens d'image

Les images ne doivent pas faire partie du texte d'un lien.

Les icônes de drapeau situées à côté des liens utilisateur doivent être séparées du texte du lien. Voir l'exemple suivant :

```markdown
![][flag_AU] [peppy](https://osu.ppy.sh/users/2)
```

### Icônes de drapeaux

*Pour une liste d'icônes de drapeaux, voir : [issue \#328](https://github.com/ppy/osu-wiki/issues/328)*

Les icônes de drapeau utilisent le code à deux lettres (en majuscules) et se terminent par `.gif`. Lorsque vous ajoutez un drapeau en ligne, utilisez ce format :

```markdown
![](/wiki/shared/flag/xx.gif)
```

Où `xx` est le code pays à deux lettres [ISO 3166-2](https://fr.wikipedia.org/wiki/ISO_3166-1_alpha-2) du drapeau.

Le nom complet du pays doit être ajouté dans le texte du titre. Le code du pays dans le texte alternatif est facultatif, mais doit être appliqué à toutes les icônes de drapeau dans l'article.

## Tableaux

Les tableaux du site Web ne prennent en charge que les titres de la première ligne.

Les tableaux ne doivent pas être embellis (ne pas remplir les cellules d'espaces supplémentaires pour uniformiser leur largeur). Ils doivent comporter une barre verticale (`|`) à gauche et à droite et le texte de chaque cellule doit être complété par un espace des deux côtés. Les cellules vides doivent comporter une barre verticale (`|`) suivie de deux espaces, puis d'une autre barre verticale (`|`).

La ligne de délimitation (la ligne suivante après le titre du tableau) ne doit utiliser que trois caractères par colonne (et être complétée par un espace des deux côtés), qui doivent ressembler à l'un des éléments suivants :

- `:--` (pour l'alignement à gauche)
- `:-:` (pour l'alignement central)
- `--:` (pour un alignement à droite)

---

Voici un exemple de ce à quoi doit ressembler un tableau :

```markdown
| Équipe rouge "Picturesque" | Score | Équipe bleue "Statuesque" | Moyenne des étoiles de la beatmap |
| :-- | :-: | --: | :-- |
| **peppy** | 5 - 2 | pippi | 9.3 stars |
| Aiko | 1 - 6 | **Alisa** | 4.2 stars |
| Ryūta | 3 - 4 | **Yuzu** | 5.1 stars |
| **Taikonator** | 7 - 0 | Tama | 13.37 stars |
| Maria | Pas de concours | Mocha |  |
```

## Citations en bloc

Les citations en bloc sont limitées à la citation du texte d'une personne. Elles ne doivent pas être utilisées pour formater le texte.

## Ruptures thématiques

La rupture thématique (également connue sous le nom de règle ou ligne horizontale) doit être utilisée avec parcimonie. Voici quelques exemples d'utilisation de la rupture thématique (liste non exhaustive) :

- séparer les images du texte
- séparation de plusieurs images qui se suivent
- déplacer le sujet à l'intérieur d'une section

Elles doivent être précédées et suivies d'une ligne vide. Les ruptures thématiques ne doivent utiliser que trois tirets, comme illustré ci-dessous :

```markdown
---
```
