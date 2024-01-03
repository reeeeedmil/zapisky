# Chyby analogových měřicích přístrojů
1. Chyba metody ($\Delta{}_M$)
	- Chyby vznikají vzájemným působením měřicího přístroje a měřeného objektu
	- Měřicí přístroje potřebují pro svoji činnost určitou energii, kterou odebírají z měřeného objektu
	- Chyby metody jsou chybami soustavnými
	- Známe jejich příčiny, můžeme určit jejich velikost i znaménko, tzn. můžeme je korigovat

2. Chyby měřicích přístrojů ($\Delta{}_P$)
	- Vznikají nedokonalostí měřicího přístroje sestávajících se ze značného množství součástí, které jsou samy o sobě zatíženy nepřesnostmi (např. Výrobní tolerance)
	- Chyby měřícího přístroje je třeba znát v celém měřicím rozsahu
	- Základní chybu vykazuje měřicí přístroj při měření ustálených hodnot za referenčních podmínek (referenční podmínky zahrnují klimatické veličiny, mechanické veličiny, veličiny ovlivňující napájení, pole a záření - např. magnetické pole)

3. Lidský faktor
	- Tyto chyby mohou významnou měrou ovlivnit kvalitu měření
	- Příčinou jejich vzniku jsou:
		- volba nevhodné metody
		- nesprávné připojení nástrojů
		- Chybná obsluha
		- Nízká pečlivost
		- Chybné vyhodnocení výsledků

4. Celková chyba měření ($\Delta{}_{MAX}$)
	- Největší možná chyba měření
	- Celková chyba měření udává tolerance, ve kterých leží skutečná hodnota měřené veličiny:
		- $\Delta{}_{MAX} = (\Delta{}_{M}+|\Delta{}_{P}|) * SIGN(\Delta{}_{M})$
		- SIGN je funkce, která zjistí znaménko čísla


5. Multiplikativní chyba
	- Z charakteru změn údaje lze soudit na určité příčiny vzniku chyb
	- Ve všech těchto chybách je vyznačena ideální a skutečná převodní charakteristika $M_P$, který převádí měřenou veličinu $X_M$ na výstupní $Y_M$ v celém měřicím rozsahu $X_R$ 
	- Absolutní
		- Tato chyba se lineárně zvětšuje s rostoucí měřenou hodnotou
		- Vzniká nepřesným nastavením měřicího přístroje (MP)
	- Aditivní
		- Může mít příčiny v chybně nastavené nulové poloze nebo chybovém napětí (offsetu zesilovače)
		- Absolutní hodnota této chyby nezávisí na velikosti měřené veličiny a je konstantní po celém rozsahu MP
		- Tato chyba je způsobena nepřesností montáže
	- Chyba linearity
		- Tato chyba se mění v průběhu měřicího rozsahu (MR) nerovnoměrně
		- Je způsobena nelineárními charakteristikami použitých materiálů a součástek MP
		- U přesných MP se odchylky od linearity zachycují tzv. korekční křivkou přístroje 

# Chyby digitálních měřicích přístrojů
- Rozlišení DMP se často udává v počtu digitů (číslic)
- Podle konvence 1/2 (půl digit) může zobrazit pouze 0 nebo 1; 3/4 od 0 do 2 nebo až do 8 (nejčastěji do 3 nebo 5)
- Např. DMP 5 1/2 má bude mít 5 číslic, které budou zobrazovat čísla od 0 do 9 a jedno, které bude zobrazovat jen 0 nebo 1
	- Takový DMP bude moci zobrazit hodnoty
		- od 0 do 1 999 99
- Pokud bude mít DMP display 3 3/4
	- Hodnoty od 0 do 5 999 (nebo 3 999, závisí na výrobci)

- Chyby DMP nejsou vyjádřeny třídou přesnosti
- Ustálila se forma vyjádření základní chyby při referenčních podmínkách; pokud nejsou referenční podmínky dodrženy, vznikají přídavné chyby
- Základní chyba DMP se vyjadřuje součtem dvou složek
$|\delta{}| = |\delta{}_M| + |\delta{}_R|$

- Chyba $\Delta{}_M$
	- Zahrnuje zejména nedokonalost nastavení hlavních měřicích prvků
	- Má charakter multiplikativní chyby

- Chyba z rozsahu $\Delta{}_R$
	- Má charakter chyby aditivní
	- Zahrnuje zejména chybu způsobenou posunutím nuly vstupního zesilovače (driftem, zbytkovým napětím spínačů a kvantováním)
	- Někteří výrobci udávají chyby DMP: $|\delta{}| = |\delta{}_M| + |d|$ kde d je chyba udaná v počtu jednotek posledního místa displeje
		- Její hodnota v jednotkách měřené veličiny závisí na zvoleném měřicím rozsahu a počtu D indikovanáých míst displeje
	- $\delta{}_R = \frac{d}{D} * 100$
	- Při vyhodnocování přesnosti měření se udává největší možná chyba údaje vyjádřena jako absolutní chyba DMP
	- $|\Delta{}_P| = |\Delta{}_M| + |\Delta{}_R| = \frac{|\delta{}_M*X_M| + |\delta{}_R*X_R|}{100}$
	- Absolutní chyba $\Delta{}_P$ roste s měřenou veličinou - má multiplikativní charakter
	- Absolutní chyba z rozsahu je po celém měřicím rozsahu konstantní - má aditivní charakter

- Relativní chyba údaje DMP
	- Dána součtem dvou chyb
	- $\delta{}_{DP} = |\frac{|\Delta{}_P|}{X_M}| * 100 = |\delta{}_M| + |\delta{}_R*\frac{X_R}{X_M}|$
	- Při růstu měřené veličiny bude chyba menší

Příklad:
Pro příklad uveďme údaje běžného DMP např. M890G, uvažujeme rozsahu pro měření DC napětí.
DMM má uvedené m. rozsahy v dekadických násobcích 2, jedná se o takzvaný 3 1/2 display s maximální hodnotou 1999

| Rozsah | Chyba | Rozlišení | 
|-|-|-|

## Praktický příklad
![[dmm-1.png]]
Na uvedeném DMM bylo naměřeno napětí 1.78V na rozsahu 20V
Spočítejte celkovou relativní chybu rozsahu, relativní chybu pro naměřenou hodnotu

$$|\Delta_P| = |\Delta_M| + |\Delta_R| = \frac{|\delta_M*U_M| + |\delta_R*U_R|}{100} = \frac{|\pm 0.5 * 1.78| + |0.05*20V|}{100} = \pm 18.9mV$$

$$U_S \space\epsilon \space <1.7611; 1.7898>V$$
Vhodně zvolený rozsah = 2V

Na rozsahu 2V bylo naměřeno napětí 1.778 voltů.
$|\Delta_P| = 9.89mV$
$$U_S \space\epsilon \space <1.768; 1.788>V$$
Z výsledků je vidět, že v tomto případě je chyba podstatně větší. Je tedy evidentní, že rozsah nebyl pro toto napětí zvolen správně, a proto nebylo možné efektivně využít přesnost měřicího přístroje. Na displeji MP si rovněž musíme všimnout, že první číslice není obsazená. To znamená, že pro měření tohoto napětí je multimetr přepnut na zbytečně vysoký rozsah.

## Výpočet chyby měření

| Rozsah | Chyba | Rozlišení |
| ---- | ---- | ---- |
| 200mV | +-0.5%rdg | 100mV |
| 2V | +-1digit | 1mV |
| 20V |  | 10mV |
| 200V |  | 100mV |
| 1000V |  | 1V |

| Rozsah | Chyba     | Rozlišení |
| ------ | --------- | --------- |
| 200mA  | +-0.5%rdg +-1digit | 0.1mA     |
| 2mA     |   | 1mA       |
| 200mA    |           | 10mA      |
| 200mA   | +-1.2%rdg +-1digit          | 100mA     |
| 2A  | +-2%rdg +-5digit          | 1mA        |
svorka ampérmeter do série, paralelně rezistor a voltmetr, svorka
Přímým měřením zjistíme hodnotu napětí a proudu. Vypočteme hodnotu výkonu P.
Výslednou chybu odvodíme z chyb přímo měřených veličin.
Protože obě veličiny jsou udány ve svých jednotkách, nelze jednoduše sečíst absolutní chyby.

Byly naměřeny tyto hodnoty:
I = 125.4mA
U = 15.56V
