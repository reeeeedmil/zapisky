# Von Neumannova struktura počítače
Principy práce počítače a základní stavbu navrhl v roce 1945 americký matematik John von Neumann. Tato struktura je s určitými obměnami základem počítačů dodnes.

Pravidla stanovená von Neumannem:
1. Počítač se skládá z řadiče, aritmetickologické jednotky, paměti, vstupního a výstupního zařízení.
2. Struktura počítače je nezávislá na řešeném problému.
3. V paměti jsou data uložena společně s instrukcemi programu.
4. Paměť je rozdělena na buňky stejné velikosti, ke kterým se přistupuje prostřednictvím adresy.
5. Program je tvořen posloupností instrukcí.
6. Pořadí provádění instrukcí je sekvenční (postupné) s výjimkou instrukcí skoku.
7. Instrukce, data a adresy jsou kódovány binárně.

![[neumann.png]]


# Harvardká struktura počítače
Harvardská struktura počítače předpokládá existenci dvou oddělených pamětí. V první paměti jsou uloženy instrukce (programy) a ve druhé jsou uložená proměnná data. Každá paměť se adresuje samostatně. Umožňuje paralelní čtení instrukce při běhu programu – dochází ke zrychlení zpracování instrukcí. Tato koncepce se využívá např. v jednoúčelových programovatelných automatech nebo kapesních kalkulátorech.

![[harvard.png]]