# Měření na jednocestném usměrňovači
## Zadání
1. Zapojte obvod a zobrazte a zakreslete (vyfoťte typické průběhy napětí a proudu)
2. Připojte ampérmetr a odměřte $U_{MAX}$, $U_{MIN}$, $\Delta{}U$ na proudu do zátěže $R_Z$
3. Střední hodnotu (na osciloskopu MEAN) a zvlnění ($P_K-P_K$) změřte i multimetry
4. Závislosti zakreslete a určete použitelnost pro stabilizátor 7805
5. Zkontrolujte ohmmetrem a zapište i odpory vinutí transformátoru.
## Teoretický rozbor
Jednocestný usměrňovač je pro ověření vlastností usměrňovače vhodnější protože osciloskop má propojené země a lze snadněji zobrazit vzájemnou závislost průběhů napětí v obvodu včetně proudu snímaného na odporu $1\Omega$. Měřit se musí proti společné zemi, což předpokládá inverzi jednoho z průběhů. Navíc i exponenciální pokles napětí při vybíjení kondenzátoru je názornější, protože je samozřejmě delší než u normálně používaného dvoucestného zapojení. Použité transformátory mají větší vnitřní odpor a klesá u nich při odběru porudu napětí. Autotranformátorem nastavíme napětí na priIáru tak, aby bylo snadné regulovat proud od 0,1A a napětí na osciloskopu nebyly příliš velké.


| I mA   | 0   | 133   | 203  | 297  | 398 | 501 | poznámka   |
| ------ | --- | ----- | ---- | --- | --- | --- | ---------- |
| MIN V  | 14.92   | 11.8  | 6.8  | 2.0    | 200mv    | 0    | osciloskop |
| MAX V  | 15.2   | 16.0  | 12.6 | 8.6    | 5.4    | 2    | osciloskop |
| MEAN V | 15   | 13.7  | 9.4  | 4.91    | 2.36    | 720mV    | osciloskop |
| Pk-Pk  | 0.4   | 4.20  | 6.0  | 6.60    | 5.2    | 2.2    | osciloskop |
| Uac V  | 0.005   | 1.284 | 1.77 | 2.077    | 1.74    | 0.717    |            |
| Udc V  | 15.0   | 13.65 | 9.27 | 4.850    | 2.31    | 0.701    |            |


