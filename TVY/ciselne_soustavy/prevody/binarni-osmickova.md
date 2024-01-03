# Převod mezi binární a osmičkovou soustavou
## Převod z osmičkové do binární
Pro převod z osmičkové do binární používáme metodu tří bitů. To znamená, že každý jeden znak v osmičkové soustavě se rovná třem bitům v binární. Zde je tabulka na převod:

|Osmičková|Binární|
|:---:|:---:|
|0|000|
|1|001|
|2|010|
|3|011|
|4|100|
|5|101|
|6|110|
|7|111|

Takže např. číslo $1370_8$ by bylo $001 011 111 000_2$. Jelikož 0 na začátku čísla můžeme vynechat, vypadalo by výsledné číslo takto: $1 011 111 000_2$.

Převod z binární do osmičkové můžeme provést stejným způsobem (začneme převádět od posledního znaku - u $1370_8$ bychom začali s 0.)