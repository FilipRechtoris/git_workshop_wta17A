[Odkaz na Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/)

# Úvod do testovania
*OMYL* - ľudská činnosť, ktorá vedie k nesprávnemu alebo neočakávanému výsledku

*BUG* - problém v kóde (v systéme), spôsobený predchádzajúcim omylom

*ZLYHANIE* - výsldok činnosti chybného softvéru alebo iného vonkajšieho zlyhania

**TESTOVANIE** je súbor procesov a činností, ktoré slúžia na kontrolu kvality softvérového produktu z hľadiska
* funkčnosti
* spoľahlivosti
* použitešnosti
* výkonnosti
* bezpečnosti

**CIELE TESTOVANIA** 
* verifikácia požiadaviek
* nachádzanie defektov a ich prevencia
* poskytnutie informácií pre ďalšie rozhodovanie v procese vývoja
* redukcia rizika neadekvátnej kvality
* budovanie dôvery

**Prečo testujeme:**
- Aby bol produkt spoľahlivý
- Aby sme overili kvalitu
- Aby bol zákazník spokojný 

**7 princípov testovania**
1. Tesovanie poukáže na prítomnosť defektov nikdy však na ich neprítomnosť.
2. Vyčerpávajúce trstovanie nie je možné.
3. Včasné testovanie ušetrí peniaze aj čas.
4. Zhromažďovanie defektov.
5. Pesticídny paradox.
6. Tesovanie závisí od kontextu.
7. Falošná neprítomnosť defektov.

**Omyl, defekt, bug**

- OMYL- ľudská činnosť, ktorá vedie k nesprávnemu alebo neočakávanému výsledku;
- DEFEKT (BUG) - problém v kóde spôsobený predchádzajúcim omylom;
- ZLYHANIE - výsledok činnosti chybného softvéru alebo iného vonkajšieho zlyhania



# Session based testing 
je kontrolovaný Exploratory testing. 
>Schémou testovania je rýchle objavenie chýb, Test-design v priebehu testovania a okamžité reportovanie a vyhodnotenie.

*EXPLORATORY TESTING* - je forma testovania pre základnú verifikáciu produktu, kde analýza a písanie testov sa robia zároveň s testovaním a používa sa pri agilnom vývoji.

Základné pojmy - MISSION, CHARTER, SESSION, REPORT, DRBRIEF

![](https://blog.qatestlab.com/wp-content/uploads/2011/02/exploratory-testing-process.jpg)


# Jira and Bug 
je nástroj na riadenie projektu.
> Medzi základné funkcie patrí manažovanie úloh ako vytváranie a prideľovanie úloh ako aj "hlásenie" stavu úloh v reálnom čase a tvorba reportov. 

**PRIORITA** - ako rýchlo má byť odstránená chyba
**SEVERITA** - aký dopad má chyba


*Exploratory testing* - je jeden z prístupov testovaniu, kedy sa súbežne tester učí ako aplikácia funguje, navrhuje vhodné testy a paralelne robí exekúciu.

# Jira and Bug


# Manažment testovania 
Proces testovania musí byť plánovaný a riadený a zahŕňa
* analýzu a návrh testov
* implementáciu a vykonanie testovania
* vyhodnotenie kritérií a reportovanie
* aktivity uzatvorenia testov

**TESTRAIL** - platforma na manažovanie testov, vytváranie testovacích prípadov, exekúcia testovacích prípadov a reportovanie. 
Je možná integrácia s inými nástrojmi.

# Modely vývoja software-u 
Poznáme:
* **sekvenčné modely** - majú lineárny, sekvenčný tok činností. Nová fáza vývoja začína až po skončení predchádzajúcej a testovanie začína až na konci  - WATERFALL, V-MODEL, W-MODEL
* **cyklické modely** - iteratívne a inkrementálne

* ďalším prístupom k testovaniu je **AGILITA**
* **SCRUM** Metodika.

**Waterfall**
- sekvenčný model vývoja softvéru
- vznikol v 70. rokoch
- skladá sa z fáz, ktoré nasledujú jedna po druhej, nie je možné sa vrátiť späť
- testovanie prichádza príliš neskoro, čím sa môžu zvýšiť náklady (princíp včasného testovania)
- v súčastnosti sa používa pre malé projekty, kde je veľmi detailná špecifikácia/dokumentácia


[Agilný manifest](https://agilemanifesto.org/iso/sk/manifesto.html)

1. Ľudia a komunikácia sú viacz než procesy a nástroje.
2. Funkčný sotfvér je viac než vyčerpávajúca dokumentácia.

3. Spolupráca so zákazníkom je viac než dojednávanie zmluvy.


4. Radšej reagovať na zmenu než sa držať plánu.


**Agilné metodiky a techniky:**
- Extrémne programovanie
- Test driven development
- Behavior driven development
- DevOps 
- Lean software development
- Kanban
- Scrum 


# Techniky tvorby testov
1./ *techniky založené na špecifikácii* (ak nepoznéme internú štruktúru kódu) - čierna skrinka
* rozdelenie ekvivalencie
* analýza hraničných hodnôt
* testovanie rozhodovacích tabuliek
* testovanie prechodu stavov
* testovanie prípadov použitia

2./ *techniky založené na štruktúre* (ak poznáme štruktúru kódu) - biela skrinka
* testovanie a pokrytie príkazov
* testovanie a pokrytie rozhodovaní
* ďalšie

3./ *techniky založené na skúsenosti testerov*
* odhadovanie omylov
* prieskumné testovanie - exploratory testing

**Kategórie Techník tvorby testov**
- *Založené na špecifikácií*
- *Založené na štruktúre*
- *Založené na skúsenostiach*

**Založené na špecifikácií** (Čierna skrinka)
- používajú sa formálne a neformálne modely
- nevýhodou je, že nevieme akú časť kódu sme testami pokryli
- najčastejšie používané v praxi
- môžu byť funkcionálne (čo systém robí) a nefunkcionálne (ako systém funguje)
1. Rozdelenie ekvivalencie
2. Analýza hraničných hodnôt
3. Testovanie rozhodujúcich tabuliek
4. Testovanie prechodu stavov
5. Testovanie prípadov použitia


**Založené na štruktúre** (biela skrinka)
- vieme ako vyzerá štruktúra kódu 
- Rozsah pokrytia softvéru môže byť meraný pre existujúce testovacie prípady
- pri návrhu testov je používaná interná znalosť kódu ako aj rôzne programovacie techniky pri návrhu testov

1. Testovanie a pokrytie príkazov
2. Testovanie a pokrytie rozhodovaní
- Existujú silnejšie úrovne pokrytia štruktúr okrem pokrytia rozhodovaní, napríklad pokrytie podmienok a pokrytie viacnásobných podmienok 


**Založené na skúsenostiach**
- používajú sa skúsenosti a znalosti ľudí
- testy píšu ľudia so znalosťami softvéru
 1. Odhadovanie omylov (error guessing)
- testeri majú tendenciu nájsť defekty na základe skúseností
2. štruktúrovaný prístup znamená vypracovanie zoznamu možných omylov a návrhu testov, ktoré budú na tieto omyly útočiť.
- tento štruktúrovaný prístup sa volá útok na chyby (fault attack)

Prieskumné testovanie (exploratory testing)
- je to súbežný návrh, vykonávanie, zaznamenávanie testov a učenie sa aplikácie.
- najúčinnejšie tam, kde nie sú dostatočné špecifikácie a silný časový tlak.



# HTML, CSS, JavaScript 

**HTML** - popisný jazyk, ktorý definuje štruktúru stránky (obsah stránky) 

**CSS** - definuje ako má stránka vyzerať - vizuál

**JAVA SCRIPT** - programovací jazyk, ktorý vdýchne stránke život

# Nástroje testovania 

* zaznamenávajú a sprehľadňujú nápady a idey
* umožňujú nám testovanie
* nahrádzajú manuálne testovanie
* zefektívňujú testovanie
* umožňujú manažovať testovanie
* automatizácia
* umelá inteligencia

# Testovanie API 
API - aplikačné programové rozhranie na komunikáciu, dopytovanie - REQUESTy a následný RESPONSE - požadované dáta

Prenosové protokoly - HTTP a HTTPS 

*HTTP request* - header + body

*HTTP response* - status code + header + body

**Metódy na požiadavky:**
1. GET
2. POST
3. PUT
4. DELETE

**JSON** dátový formát na prenos dát - {"key":"value"}

**POSTMAN** - nástroj na manuálne a automatické testovanie rozhraní 

# SQL
je jazyk, resp. štandard pre manažovanie dát v relačných databázach

*Databáza* - množina štruktúrovaných dát
**Primárny kľúč (Primary key)** - jeho úlohou je jednoznačne identifikovať  každý záznam v tabuľke. Nesmie mať hodnotu null. 

*Relačná databáza* - je založená na relačnom modeli, ktroý definuje spôsob uloženia dát v tabuľke

*Request metódy* - GET, POST, PUT, DELETE

*DML metódy* - SELECT, INSERT, UPDATE, DELETE

*Príkazy* - SELECT, WHERE, LIKE, IN, DISTINCT, BETWEEN, agregačné funkcie - COUNT, MAX, MIN, SUM, AVG, GROUP BY, ORDER BY, ALIAS - AS, HAVING, NULL, JOIN 


