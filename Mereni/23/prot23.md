# Měření na rezonančním obvodu
## Zkoušený předmět - Rezonanční obvod
### Zadání
1) Zobrazte časové a fázové diagramy pro sériový rezonanční obvod v zapojení s ideálním kondenzátorem a ideální cívkou a pro obvod s ideálním kondenzátorem a reálnou cívkou.
2) Zobrazte amplitudové a fázové frekvenční charakteristiky pro RLC pásmovou propust (pro různé hodnoty tlumicího odporu R, např. R = 100 ohm, 200 ohm, 500 ohm)
3) Zobrazte amplitudové a fázové frekvenční charakteristiky pro RLC pásmovou zádrž (pro různé hodnoty tlumicího odporu R, např. R = 100 ohm, 200 ohm, 500 ohm)

### Rozbor
#### Sériový rezonanční obvod
Elektrický obvod tvořený zdrojem střídavého elektrického napětí budícího střídavý elektrický proud procházející sériovým zapojením odporu, indukčnosti a kapacity. Při určité tzv. rezonanční frekvenci se v tomto obvodu vyrovnává kapacitní a induktivní reaktance a rezonanční obvod se pro tuto frekvenci chová jako rezistance. Cívka je charakteristická svou indukčností a kondenzátor svou kapacitou. Při průchodu proudu obvodem se v cívce periodicky vytváří a zaniká magnetické pole a kondenzátor se periodicky nabíjí a vybíjí. Tento jev se nazývá rezonance.
#### Paralelní rezonanční obvod
Elektrický obvod, který se skládá z rezistoru, kondenzátoru a cívky, propojených paralelně. Tento obvod je významný tím, že má specifickou rezonanční frekvenci, při které má obvod maximální proud. Paralelní rezonanční obvod se často používá v elektronických zařízeních jako filtr s úzkopásmovou charakteristikou. Obvod může být také využit jako rezonanční transformátor, kde se vstupní a výstupní signál propojí s cívkou a kondenzátorem, které jsou naladěny na stejnou frekvenci.
#### Pásmová propust
Elektrický obvod, který umožňuje propustit signály v určitém pásmu frekvencí a potlačí signály mimo toto pásmo. To znamená, že propouští signály s frekvencemi v určitém rozsahu a blokuje signály s frekvencemi mimo tento rozsah. Existuje několik typů pásmových propustí, ale základním prvkem všech těchto obvodů je kombinace filtračních prvků jako jsou kondenzátory, cívky a rezistory, které jsou propojeny v určité konfiguraci. Pásmová propust umožňuje propustit signály v určitém pásmu frekvencí a blokovat signály s frekvencemi mimo tento rozsah. Pásmová propust lze navrhnout pomocí kombinace dolní a horní propusti, které jsou propojeny dohromady. Tímto způsobem lze dosáhnout vytvoření pásmového filtru, který má přesně definovanou propustnou šířku.
#### Pásmová zádrž
Elektrický obvod, který potlačuje signály v určitém pásmu frekvencí a propouští signály mimo toto pásmo. To znamená, že blokuje signály s frekvencemi v určitém rozsahu a propouští signály s frekvencemi mimo tento rozsah. Pásmová zádrž se obvykle skládá z kombinace horní a dolní propusti, které jsou propojeny v záporné zpětné vazbě. Tato zpětná vazba vytváří rezonanční obvod s rezonanční frekvencí, která se přesně shoduje s frekvencí, kterou chceme blokovat. Pásmová zádrž může být užitečná například pro eliminaci rušení v audio signálu nebo pro potlačení určitého signálu v oblasti, kde je jinak příliš vysoký. To může být užitečné při přenosu signálu, kde se chceme zbavit určitého typu šumu.

### Postup
Při měření na RC2000 postupujeme podle zadání a ukládáme jednotlivé charakteristiky.

### Použité vztahy
Thompsonův vztah:
$$
f_0 = \frac{1}{2\pi\sqrt{LC}} [Hz; H, F]
$$