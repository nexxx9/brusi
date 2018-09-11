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

Za delat enačbe zaenkrat uporabljamo slike (kasneje bomo automatsko zrenderali sintakso v dive in to samo ni še narjeno to trenutno) in te slike generiraš na [tej strani](http://rogercortesi.com/eqn/index.php?filename=tempimagedir%2Feqn8242.jpg&latextext=&outtype=jpg&bgcolor=white&txcolor=black&res=150&transparent=1&antialias=1) in to z LaTeX sintakso ki je razložena [tukaj](https://en.wikibooks.org/wiki/LaTeX/Mathematics). Rezultati so taki in sliko seveda uploadaš na imgbb.

![Enačba](https://image.ibb.co/grTzFK/eqn3402.jpg)
