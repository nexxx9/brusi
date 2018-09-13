# Preface

Matematične formule se piše v [LaTeX syntaksi][latex-syntax-wiki].  Uporabi se [generator][latex-to-svg] ki ti iz formule nardi svg sliko in pol jo daš v md dokument. Sliko uploadaš na [imgbb][img-upload-dest].

<br>

### Postopek dodajanja enačbe v dokument

Trenutno je postopek zajeban kr še ni pravi support za normalne markdown račune ampak to tudi boljše dela + maš svg kar je nnnajs.

<br>

- Napiši formulo v [LaTeX][latex-syntax-wiki] sintaksi v [ta generator.][latex-to-svg] Če rabiš grške črke jih [imaš tu.][greek-latex]
- Na [gist.githubu][gist-gh] naredi nov __hidden gist__
  - Napišeš v _filename including extension_ npr. `vaja1racun1del1.svg`
  - SVG kodo kopirano iz generatorja minimiziraš v [SVG minifierju][minifysvg]
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


<br>

# Matematika

[latex-syntax-wiki]: https://en.wikibooks.org/wiki/LaTeX/Mathematics#Brackets
[latex-to-svg]: https://viereck.ch/latex-to-svg/
[greek-latex]: http://web.ift.uib.no/Teori/KURS/WRK/TeX/sym1.html
[rawgit]: https://rawgit.com/
[gist-gh]: https://gist.github.com/
[minifysvg]: https://www.svgminify.com/

[demo-enacba-1]: https://cdn.rawgit.com/elieven/50028fbc243f18d41eef4e8292aaa457/raw/c96f6caede3fa946d34546622010067486f94722/demo-enacba-1.svg
[demo-enacba-2]: https://cdn.rawgit.com/elieven/17368b8043be600b52155010fc96d3a8/raw/1d998f6efcafcf5093543caa65bf567a38efbce5/demo-enacba-2.svg
