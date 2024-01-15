- [Vrstvy](./vrstvy/vrstvy.md)
	- TCP/IP
	- ISO/OSI

- přidat
	- informace o zařízení (MAC adresy etc.)
	- Jak počítat podsítě
	- Popis protokolů
	- vrstvy (ISO OSI, TCP/IP)
	- Kabely
	- Wifi



# Namalovat obrázek k čemukoliv co jde
# Hrozby na sítích
- Viry
- Jak tomu předejít
- jak to případně řešit
- co je to červ? co je to spyware?
- Hrozba na síti i je bombardování mailem. DoS/DDoS
- Uživatel je taky velká hrozba
- Formy útoku
	- Pasivní/Aktivní
	- Vnější/Vnitřní
- Kde mohou být slabiny
- Zašifrovaná data? jak se tomu chránit?

# Bezpečností politika
- Co je to aktivum?
	- Jsou rozdělená
- Aktiva se dají hodnotit do kategorií
	- Vyhodnotit a udělat pořadí které z nich je kritické
		- Řeší se dvě varianty
			- Hledisko obchodní a finanční
	- Míra dopadu?
		- Mírný, vážná škoda atd
	- Podle kategorie se hledá řešení
		- Při kritickém případě mít možnost spustit síť jinde
		- Pokud nemusí být zprovozněná hned - síť nejede pár minut - může se použít jiný systém
- Rizika aktiv (rizika co by mohla aktiva znehodnotit)
	- Analyzovat rizika
	- Vytvořit návrhy jak rizika eliminovat
	- Je třeba mít nějáký systém
		- Obecný dokument, jak se řídit v různých případech
- Možnost síťové politiky
	- Volný - všichni mohou všechno
	- Zakázat vše kromě toho, co je potřeba
	- Zakázat i ty prvky, které mohou být potenciálně nebezpečné
- Dokumenty
	- Mít stanovený postupy při různých případech
- Je třeba mít zajištěnou ochranu dat

### 3
Firewall a ochrana vrstev tcp/ip
- Definovat firewall
	- Jak se řeší - hardware, software
	- Co dělá
	- Dal by se i v omezené míře definovat na routeru
	- Demilitarizovaná zóna - definice, jak se připojuje k firewallu
		- Ke kolika firewallům se připojuje?
- Jakým způsobem se řeší ochrana na tcp/ip?
### 4
ACL
- Co to je?
- Jaký typy ACL existují?
	- K čemu slouží?
	- Pořadí pravidel ACL
	- K čemu se dají použít?
	- Jaké pravidla pro ně patří? (standardní, rozšířený - co můžeme povolit a zakázat)
	- Kdy se jejich pravidla upraví
		- Jedna adresa, rozsah adres, různé protokoly, různé zdrojové adresy, různé cílové adresy, různé porty + příklad
	- Výhody/nevýhody
	- Kam položit?
		- Standard co nejblíž ke zdroji
		- Extended co nejblíž k cíli
	- Jak použít na interfacu? Kolik jich tam můžeme mít?

### 5
Zabezpečení přístupu na zařízení
- Lokální přístup
	- Např. zamčená serverovna
	- Nechceme, aby se někdo k zařízením dostal fyzicky
	- Větší areál se dá taky zabezpečit např. čipovou kartou, kamerovým systémem
- Přístup k zařízení
	- Hesla
		- Požadavky na hesla
		- Kde, jaké hesla vytvořit
			- privilegovaný mód, přístup přes konzoli, vzdálený přístup, SSH
			- Jak zabezpečit hesla? hashování?
	- Práva - co povolit, kdo může co (např. v operačním systému)

# ISO/OSI // TCP/IP
- Nakreslit
- Vzájemný vztah
- Vrstvy
- Adresy
- Vysvětlit rozbalení/zabalení struktur
- Obecně vzpomenout protokoly
- Který formát se používá - data, segment, packet, rámec
- Jak spolu jednotlivý vrstvy komunikují?

# VLAN
- Co to je?
- K čemu se to používá?
- Kdy se to používá?
- Kterých zařízení se to týka?
- Router, L2, Switch, Switch - význam jednotlivých linek
- Vysvětlit jak vlanky pomáhají/zjednodušují fyzickou strukturu kdzž to máte řešit, že se na některém musí setkat vícero zařízení z různých sítí
- Zmínit jak se vlanky konfigurují na směrovači a na přepínači (nemusí být úplně přesně commandy)
	- Obsah databáze
- VTP zmínit
	- Režimy vstupů
	- Server, host, transparent
- Redudantí spoje
- STP
- Jak se interfejsy rozřazují do vlanek
- Kde se číslo vlanky objeví a kdy
	- Přístupý interface nebo trunk

# Dynamické směrovací protokoly
- Vysvětlit co je to směrovací protokol
- Jakým způsobem se směrovací protokoly rozdělují? (Vnější, vnitřní prej)
	- Vzdálenostně-vektorový
		- Co sem patří
	- Linkově-stavový
		- Co sem patří
	- Základní charakteristika obou
	- Jakým způsobem určují co je lepší či horší cesta
	- Jakým způsobem si předávají mezi sebou informace
	- Limity různých protokolů
- Základní princip konfigurace
- Jak se do protokolů zahrnují statické cesty
- Nakreslit, porovnat jakým by způsobem síť řešil RIP, OSPF, EIGRP
	- Jakým způsobem se stanovuje cena? Výpočet?

# VPN a Symetrická/Asymetrická kryptografie
- Co to je VPN?
	- K čemu slouží?
	- Jaké typy VPN existují?
		- Jejich porovnání, co je jejich plus či mínus
	- Který typ komunikace nahrazuje
	- Síť-to-Síť vs Vzdálený přístup
		- Prý na to Šafi udělá úlohu
- Kryptografie
	- K čemu slouží?
	- Kde se používá?
	- Co to je symetrická a asymetrická šifra?
		- Fungování, porovnat je
		- Princip
		- Kde se která používá?
		- Jak se počítá? (2 velká prvočísla)
		- Jaký směr je šifrovaný?

# IPV4 adresace
## BEZ PODSÍTÍ, TY JSOU SAMOSTATNĚ 
- Forma adres
- Co to je maska,
- Podtřídy
	- Jak je poznat?
- Co je to prefix?
- Co je to číslo sítě?
- Co je to šíslo hostitele?
- Speciální adresy?
- Co je veřejná a co neveřejná adresa?
- Skupiny
	- A, B, C, D, E
	- Využití?
- Co vznikne výpočtem z IP adresy a masky?
- Co ty jedničky a nuly v masce znamenají?
- Fáze IP adresace? (jak se to měnilo skrz čas)
	- V čem je jiný použít VLSM a konstantní podsíť?

# Podsítě
- Jak počítat?
- Proč podsítě?
- Příklad (stačí podsíťovat třídu C)