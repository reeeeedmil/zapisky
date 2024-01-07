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


Hrozby na sítích
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

Bezpečností politika
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