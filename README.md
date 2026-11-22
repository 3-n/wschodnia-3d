# Nowa stacja Warszawa Wschodnia: model 3D

Strona pokazuje projektowaną przebudowę stacji Warszawa Wschodnia na trójwymiarowej mapie okolicy: dwie otwarte wiaty halowe nad peronami dalekobieżnymi (1–4) i podmiejskimi (5–7), siedem nowych peronów, przejścia pod torami z wejściami od ulic, budynki zaplecza przy ul. Kijowskiej i nowy ekran akustyczny. Tory są pokazane jako kolorowe linie, z kolorem według linii kolejowej. Można zmieniać widok, datę i godzinę, żeby zobaczyć cienie, włączać i wyłączać projekt oraz przełączyć na noc, żeby zobaczyć oświetlenie wiat, peronów i obu istniejących dworców.

Oficjalnych wizualizacji wiat jeszcze nie ma: program funkcjonalno-użytkowy wymaga, żeby wykonawca przygotował je dopiero przed budową. To nieoficjalna wizualizacja poglądowa, a nie dokument projektowy.

## Skąd są dane

- **Projekt:** [dokumentacja przetargowa](https://platformazakupowa.plk-sa.pl/app/demand/notice/public/42848/details) PKP PLK (linia średnicowa, etap IIa), projekt budowlany: plany zagospodarowania terenu (tom I) oraz tory, architektura stacji, konstrukcja wiat, perony, przejścia i budynki zaplecza (tom II).
- **Położenie w planie:** plany zagospodarowania terenu 1:500 dopasowane do granic działek z usługi ULDK (GUGiK); plan torów i rzut peronów dowiązane do nich. Położenie jest przybliżone, z dokładnością do ok. 0,5 m.
- **Wysokości:** rzędne z rysunków (PL-EVRF2007-NH): główki szyn z profili podłużnych, perony, wiaty i budynki z przekrojów i elewacji.
- **Teren:** numeryczny model terenu GUGiK (usługa services.gugik.gov.pl/nmt), siatka co 10 m.
- **Mapa:** ortofotomapa GUGiK z 2025 r., pobierana na żywo z geoportal.gov.pl, oraz modele 3D budynków (LoD1, 2024) i drzew (LoD1, 2023) GUGiK, przycięte do kwadratu ok. 1,9 km i uproszczone. Zapisane w pliku `surroundings.glb`.

## Dokładność

**Odczytane z rysunków:** długości, szerokości i wysokości wiat, rozstaw słupów i rzędów słupów, kratownice trójkątne i kalenicowe, układ przeszkleń w dachu, wywietrzniki, ściany czołowe, siatki z neonem, obrysy i wysokości peronów, położenie wind, zejść, budynków technicznych i wiat siedziskowych, obrysy i wysokości budynków zaplecza, przebieg torów.

**Szacunkowe:** grubości prętów, szczegóły dźwigarów krzyżowych, wygląd szkła z ogniwami fotowoltaicznymi (rysunki go nie odróżniają), kolor neonu, układ pasm iluminacji dachu, wysokość wiat siedziskowych, wysokość ekranu akustycznego względem terenu, linie kolejowe części torów poza stacją (szare).

## Znane ograniczenia

- Tory są osiami, bez rozjazdów, szyn, podsypki i sieci trakcyjnej.
- Przejścia pod torami są pod ziemią: widać tylko ich wejścia, zadaszenia i świetlik.
- Budynki z mapy przeznaczone w projekcie do rozbiórki oraz drzewa w miejscu nowych obiektów i drzewa oznaczone do wycinki znikają po włączeniu projektu.
- Ciemne plamy na zdjęciach mapy to cienie z dnia nalotu. Nie zmieniają się z godziną.
- Mapa jest wczytywana tylko do ok. 950 m od środka stacji, żeby strona działała płynnie. Dalej widać jednolite tło.
- Na mapie budynki to proste bryły z płaskim dachem, a drzewa to uproszczone korony.

## Uznanie autorstwa

Silnik: [CesiumJS](https://cesium.com/platform/cesiumjs/) (Apache 2.0). Mapa: ortofotomapa, numeryczny model terenu oraz modele 3D budynków i drzew GUGiK z geoportal.gov.pl, przetworzone jak opisano wyżej. Projekt: PKP Polskie Linie Kolejowe S.A., dokumentacja przetargowa (projektanci: Torprojekt sp. z o.o., Kuryłowicz & Associates sp. z o.o.).
