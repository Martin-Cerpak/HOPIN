# HOPIN
Testovacie zadanie pre pracovný pohovor.


- nevedel som pohnúť s funckoiu onClick ktorá mala klonovať element do outputu ( hľadal som po stackoverflow, mdn, google search nejaké riešenia,
takmer všetky som našiel len na jednoduché polia a nie na polia objektov ako v tomto prípade, v reále by som mal možnosť sa opýtať skúsenejsšieho 
kolegu, ktorý by ma vedel nasmerovať akým sa uberať pri riešení problému čo v tomto prípade nebolo možné, nie je to výhovorka len konštatujem,
že každý sa zasekne na nejakom probléme aj keď je sebemenší :-) ...a po dobrom tipe od niekoho a vyriešení príde ten aha moment :D , ktorý pozná každý )

- nasledujúce funkcie, ktoré mali byť naviazané na klonovaný element som vypracoval oddelene
 
 PS: v zadaní je asi chyba:
 - podla aktualneho casu spraivs rozdiel casov a zistis ci je mensi ( malo by byť väčší ) ako attribute "limit"
 - ak je mensi ( malo by byť väčší ) ako limit tak HTML element kde sa ma zobrazit vystup bude mat pozadie zelenej farby, inak cervene

---------------
Znenie zadania:

- Snažíme sa používať čistý javascript bez nijakých knižníc pokiaľ to nie je potrebné
- Uvažujeme s tým že do funkcie nejdú vždy také data aké očakávame, takže treba ošetriť takéto prípady

test:

HTML & CSS
- napíš jednoduché HTML a CSS (bonusové body za použitie Sass)
- výsledok nech vyzerá +- ako príkladový obrázok
- dbaj na responzivitu

Javascript
- napíš objekt, ktorý bude obsahovať funkcie na vygenerovanie HTML
- obsah HTML elementov bude "text" z array of objects (data)
- HTML elementy budu obsahovat attributes "time" a "limit" 
- pokial sa neda s danymi datami pracovat tak ignorujme cely objekt, nevykreslime ho do HTML
- elementy budu mat onclick funkciu kde sa zoberie "time" attribute
- podla aktualneho casu spraivs rozdiel casov a zistis ci je mensi ako attribute "limit"
- ak je mensi ako limit tak HTML element kde sa ma zobrazit vystup bude mat pozadie zelenej farby, inak cervene
- vo vystupe sa taktiez ukaze: text z HTML elemntu, aktualny cas v podobe HH:MM a vypocitany rozdiel
- kod ma byt napisany tak aby sa dal automatizovane testovat

bonusove body za vylepsenie UX stranky, napr. vizualna zmena HTML elementov pri onClick funkciach atd.

- vysledok: github repo

priklad dat, ktore dostanes zo serveru:



var data = [

   {
    text: "Bratislava",
    time: "21:50",
    limit: "5"
   },
    
   {
    text: "Kosice",
    time: "18:20",
    limit: 10
   },
    
   {
    text: "Trnava",
    time: "21:00",
    limit: "12"
   },
    
   {
    text: "Trencin",
    time: "16:25",
    limit: 30
   },
	
   {
    text: "Martin", 
    time: "16:25",
    limit: null  
   },
	
   {    
    text: "Kysuce",
    time: null,
    limit: 100
   }
];
