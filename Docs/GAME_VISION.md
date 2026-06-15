Chci začít stavět krátkou first-person atmosférickou hororovou hru v Unreal Engine. Jsem začátečník v Unreal Enginu, ale mám zkušenost s postupným vývojem projektů přes malé ověřené kroky, Git a AI coding asistenty.

Pracovní název projektu: Night Shift Ticket.

Cíl první verze:
Vytvořit malé 5 až 10 minutové hratelné demo bez combatu. Hráč je noční IT pracovník ve firemní budově. Přes ticketovací systém dostává úkoly, chodí do místností, používá foťák/kameru a přes foťák vidí věci, které v normálním pohledu nejsou vidět. Foťák slouží jako hlavní mechanika pro odhalování skryté vrstvy reality a spouštění událostí.

Inspirace:

* The Mortuary Assistant: pracovní rutina, která se postupně mění v horor.
* P.T.: opakující se prostor, malé změny, narušování reality.
* Outlast: first-person zranitelnost bez combatu.
* Nechci random strašení bez pravidel. Každý děsivý event by měl mít signál, důvod nebo pravidlo.

Základní prostředí první verze:

* IT kancelář jako základna s PC/ticket systémem.
* Chodba.
* Zasedací místnost.
* Malý kancl.
* Serverovna.

Core gameplay loop:

1. Hráč sedí v IT kanceláři.
2. Na PC přijde ticket.
3. Hráč jde do určené místnosti.
4. Normálně problém nevidí.
5. Přes foťák se objeví skrytá vrstva reality.
6. Hráč pořídí fotku/důkaz.
7. Vrátí se k PC.
8. Ticket se aktualizuje nebo uzavře.
9. Prostředí se po každém ticketu mírně změní.

Hlavní mechanika:
Foťák neukazuje jen duchy. Foťák ukazuje pravdivou verzi místa. Některé nápisy, objekty, siluety nebo stopy jsou viditelné pouze přes foťák. Vyfocení správné věci posune ticket nebo spustí event.

Omezení první verze:

* Žádný combat.
* Žádný inventory systém v první fázi.
* Žádný save/load systém v první fázi.
* Žádný živý OpenAI API runtime v první fázi.
* AI může pomáhat s texty, dialogy, tickety, dokumentací a návrhem Blueprint logiky, ale hra má v první fázi běžet offline.
* Použít Blueprint-first přístup. C++ až později, pokud bude opravdu potřeba.

První vertical slice:
Jedna kancelář, jedna chodba, jedna zasedačka, jeden ticket, jeden foťákový nález, jedna fotka jako důkaz, jeden update ticketu a jeden krátký hororový event.

Vývojový styl:
Postupovat jako u Panam: malé kroky, každý krok otestovat, commitovat, nepřidávat velké systémy předčasně. Nejdřív ověřit, že hlavní mechanika foťák + ticket loop působí dobře. Teprve potom rozšiřovat mapu, atmosféru a příběh.
