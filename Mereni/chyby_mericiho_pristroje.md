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
|200mV|\q_m0.5%rdg|100mV|
| 2V |\pm 1%digit|1mV|

0.5%rdg = deltaM
1%digit = deltaR (nebo d)

přepočet na procentní chybu z měřícího rozsahu přístroje 

$g_2 = \frac{d}{maximální počet indikovaných jednotek }* 100$  

$\delta_X=\delta_1+\delta_2*\frac{X}{X}$


vypočítat celkovou a relativní chybu pro rozsah 1000V
| $\delta_p$ | = |$\delta_m$ | + |$\delta_R$ | -> |+- 0,8% |    +    | $\frac{+-2}{1999 }* 100$ |   =0,9


b) Praktický příklad 
 hodnota na přístroji 1,78V
 rozsah 20V

na uvedenem dmn bylo naměřeno napětí 1,78 V na rozsahu 20 V 
tabulka viz. příklady

###### celková relativní rozsahu 
 $\delta_p$ | = |$\delta_m$ | + |$\delta_R$ | -> |+- 0,5% |    +    | $\frac{+-2}{1999 }* 100$ |   =0,9


###### relativní chyba pro naměřenou hodnotu 



###### výsledná absolutní chyba 


