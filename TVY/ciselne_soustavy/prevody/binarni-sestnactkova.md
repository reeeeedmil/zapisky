# Převod mezi binární a šestnáctkovou soustavou
## Převod z šestnáctkové do binární
Pro převod z šestnáctkové do binární používáme metodu čtyř bitů. To znamená, že každý jeden znak v šestnáctkové soustavě se rovná čtyřem bitům v binární. Zde je tabulka na převod:

|Šestnáctková|Binární|
|:---:|:---:|
|0|0000|
|1|0001|
|2|0010|
|3|0011|
|4|0100|
|5|0101|
|6|0110|
|7|0111|
|8|1000|
|9|1001|
|A|1010|
|B|1011|
|C|1100|
|D|1101|
|E|1110|
|F|1111|

Takže např. číslo $54EC_{16}$ by bylo $0101 0100 1110 1100_2$. Jelikož 0 na začátku čísla můžeme vynechat, vypadalo by výsledné číslo takto: $101 0100 1110 1100_2$.

Převod z binární do osmičkové můžeme provést stejným způsobem (začneme převádět od posledního znaku - u $54EC_{16}$ bychom začali s C.)