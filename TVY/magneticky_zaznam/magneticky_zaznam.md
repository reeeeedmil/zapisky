#magneticky_zaznam 
## Magnetický disk HDD (Hard Disk Drive)

jedná se o paměť počítače, která slouží k dlouhodobému uchování dat. 
jsou energeticky nezávislé, tzn. po odpojení napájení se data nevymažou.
### Výhody 
Pevné disky mívají velkou kapacitu, nižší cenu na jednotku úložného prostoru a dlouhou životnost.
### Nevýhody 
Nevýhodou může být pomalejší rychlost přístupu k datům ve srovnání s modernějšími technologiemi jako SSD (Solid State Drive), náchylnost k mechanickému poškození a hlučnost.
### Hlavní díly HDD
- **plotna** - nachází se na ní vrstva magnetického materiálu 
- **čtecí hlava** - slouží pro čtení a zápis na plotnu 
- **pohon disku** - motorky s kapalinovými ložisky  
- **řídící elektronika** - zajišťuje komunikaci mezi diskem a počítačem. 
#### rozděleni plotny: 
![[pevnydisk_cluster.jpeg]]
### Zápis dat na HDD
Řadičová elektronika odesílat data v podobě magnetických impulsů na povrch disku. Tyto impulsy mění magnetické pole povrchu disku podle informací, které se mají uložit.
Data jsou na povrchu pevného disku organizována do soustředných kružnic zvaných stopy na obou stranách plotny 
Sektor je nejmenší adresovatelnou jednotkou disku

### Čtení dat na HDD
 Je založeno na principu elektromagnetické indukce. To znamená, že když čtecí hlava zaznamená změnu v magnetickém poli na plotně z 0 na 1 a z 1 na 0 se indukuje v cívce napětí a do je zesíleno a dekódováno na digitální signál . Přechod mezi stavy je interpretován jako informace  
### Parametry 
- **Kapacita** - v dnešní době se jedná řádově o jednotky až desítky TB
- **Formát** - 3,5" / 2,5"
- **Rychlost otáčení** - např. 5400, 7200 otáček/min
- **Rychlost čtení / zápisu** - 110 - 180 MB/s
- **Vyrovnávací paměť** - 64 MB
- **Technologie zápisu** -CMR ?

### funkce disku 

1. **Chytré funkce (S.M.A.R.T.)**: Mnoho moderních disků obsahuje technologii S.M.A.R.T. (Self-Monitoring, Analysis, and Reporting Technology), která umožňuje sledování stavu disku a předpovídání možných selhání nebo problémů. Tato funkce je integrována do řadičové elektroniky a umožňuje uživatelům monitorovat zdraví disku.
    
2. **Řízení pohonu a otáček disku**: Elektronika HDD může také řídit pohyb motoru a otáčky disku. To zahrnuje regulaci rychlosti otáček disku podle potřeby a udržování optimálního chodu disku.

## RAID
Redundant Array of Independent Disks
spojuje několik pevných disků do logického celku


1. **RAID 0 (J_bod):** Zahrnuje dva nebo více disků a provádí distribuci dat napříč disky (stripping) pro zvýšení rychlosti čtení a zápisu dat. Nicméně, RAID 0 nenabízí žádnou redundanci, takže pokud selže jeden disk, mohou být ztracena všechna data.

2. **RAID 1:** Používá minimálně dva disky, kde data jsou zrcadlena (mirroring). Každá informace je zálohována na dalším disku, což poskytuje zvýšenou spolehlivost. Avšak kapacita úložiště je poloviční z kapacity všech disků kvůli zrcadlení.

3. **RAID 5:** Vyžaduje minimálně tři disky a kombinuje stripping dat s paritní kontrolou, což umožňuje obnovu dat v případě selhání jednoho disku. Kapacita úložiště je rozdělena mezi disky a je možné pokračovat v práci i po výpadku jednoho disku.

![[raid5_3.png]]


