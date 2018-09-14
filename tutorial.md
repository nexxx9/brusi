# Tutorial / navodila za dodajanje materiala

Tukaj je začasno osnovno napisano in razloženo kako kej nardit kar se tiče večine pogosto uporabljenih stvari. Te informacije komot najdeš na internetu če poguglaš tipo markdown in pol karkoli pač hočeš nardit z njim ampak useno je lažje to prebrat tu.

<br>

## Stvari znotraj markdowna (.md)

### Tekst

V dokument pišeš normalen tekst in pol pred vrstico ali okoli besede / besed daš določene znake ki pol uplivajo na ta tekst. Tekst v novi vrstici bo še vedno veljal kot isti `<p></p>`, za nov `<p></p>` mora bit vmes vsaj 1 vrstica. Za efekte na tekstu lahko narediš to:

|     Output     |  Kako to nardit  |
| -------------- | ---------------- |
| normalno       | `normalno`       |
| **odebeljeno** | `**odebeljeno**` |
| __odebeljeno__ | `__odebeljeno__` |
| *ležeče*       | `*ležeče*`       |
| _ležeče_       | `_ležeče_`       |
| ~~prečrtano~~  | `~~prečrtano~~`  |

Za naslove (od h1 do h6) imaš `#`. Kar je naslov mora bit v svoji vrstici in `#` na začetku vrstice. Število `#` je število naslova torej h5 jih bo imel pet.

Priporočeno je da po h1 daš 1 al 2 razmaka in po h2 enega. Razmak je vrstica kjer je samo `<br>`. Ubistvu spacing lahko delaš po občutku ampak je dobro če je enakomerno čez cel dokument.

<br>

## Linki in slike

Za naredit link kjerkoli je koda `[text](url linka)`. Fail text je kar bo prikazano in podčrtano modro, url pa je dejanski link. To je useskupaj ubistvu `<a href="{url linka}">{text}</a>` ko je vnešeno v stran oz. zrenderano.

[Primer linka](www.google.com) čeprav je lahko kjerkoli znotraj texta ni nujno da je na začetku.

Slike dodajat je skoraj enako s tem da je pred vsem skupaj klicaj in namesto teksta linka je tisto tekst ki se prikaže če se slika ne zlouda. Koda je torej `![fail text](url slike)`.

<br>

![Rolex nnnice](https://image.ibb.co/ntEH2z/rolex_daytona_2018.png)

<br>

Glede na to da moreš za sliko imet url priporočam da jo začasno uploadaš na [imgbb](https://imgbb.com/). S stem da ko uploadaš sliko uni link ki ga pokaže ni pravi za linkat sliko direkt. Za dobit tapravi link prvo klikni na sliko in potem ko jo pokaže večjo desno klikni na njo šenkrat in kopiraj url.

<br><br>

## Tabele

Poguglaj markdown tables.

<br>

## Enačbe in podobno

Matematične formule se piše v [LaTeX syntaksi][latex-syntax-wiki].  Uporabi se [generator][latex-to-svg] ki ti iz formule nardi svg sliko in pol jo daš v md dokument. Sliko uploadaš na [imgbb][img-upload-dest].

<br>

### Postopek dodajanja enačbe v dokument

Trenutno je postopek zajeban kr še ni pravi support za normalne markdown račune ampak to tudi boljše dela + maš svg kar je nnnajs.

<br>

- Napiši formulo v [LaTeX][latex-syntax-wiki] sintaksi v [ta generator.][latex-to-svg] Če rabiš grške črke jih [imaš tu.][greek-latex]
- Na [gist.githubu][gist-gh] naredi nov __hidden gist__
  - Napišeš v _filename including extension_ npr. `vaja1racun1del1.svg`
  - SVG kodo kopirano iz generatorja minimiziraš v [SVG minifierju][minifysvg] (od 70 do 92% ponavadi manjši file)
  - V tavelik kvadrat prilepiš __svg source code__ kopirano iz minifierja
  - Klikneš __create secret gist__
- Kopiraš link na katerega te je vrglo ko si kliknu na __create secret gist__
- Prilepiš ta link v [rawgit.com][rawgit]
- Kopiraš url ki je pod __Use this URL in production__
- Ta url daš za img url ko pišeš markdown kodo za uni račun

<br>

Primer enačbe `cos\gamma = \frac{ a^2 + b^2 - c^2 }{ 2ab }` se zgenerira v to:

![E=mc2][demo-enacba-1]

in `\frac{a}{sin\alpha} = \frac{b}{sin\beta} = \frac{c}{sin\gamma} = 2R` v:

![demo enačba 2][demo-enacba-2]







[latex-syntax-wiki]: https://en.wikibooks.org/wiki/LaTeX/Mathematics#Brackets
[latex-to-svg]: https://viereck.ch/latex-to-svg/
[greek-latex]: http://web.ift.uib.no/Teori/KURS/WRK/TeX/sym1.html
[rawgit]: https://rawgit.com/
[gist-gh]: https://gist.github.com/
[minifysvg]: https://www.svgminify.com/

[demo-enacba-1]: https://cdn.rawgit.com/elieven/50028fbc243f18d41eef4e8292aaa457/raw/c96f6caede3fa946d34546622010067486f94722/demo-enacba-1.svg
[demo-enacba-2]: https://cdn.rawgit.com/elieven/17368b8043be600b52155010fc96d3a8/raw/1d998f6efcafcf5093543caa65bf567a38efbce5/demo-enacba-2.svg
