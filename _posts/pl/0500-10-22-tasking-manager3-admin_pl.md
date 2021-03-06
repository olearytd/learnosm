---
layout: doc
title: Tworzenie projektu w Tasking Managerze 3
permalink: /pl/coordination/tasking-manager3-project-admin/
lang: pl
category: coordination
---

# OSM Tasking Manager - Tworzenie projektu i administrowanie nim

> Ten przewodnik może zostać pobrany jako samodzielny moduł: [tasking-manager3-admin_pl.odt](/files/tasking-manager3-admin_pl.odt) lub [tasking-manager3-admin_pl.pdf](/files/tasking-manager3-admin_pl.pdf) 

**Ten przewodnik opisuje aktualną wersję Tasking Managera. Jeżeli interfejs użytkownika wersji, którą używasz jest inny od opisanego tutaj, powinieneś spojrzeć na [podręcznik do poprzedniej wersji](/pl/coordination/tasking-manager-project-admin)**

Spis treści działu
-------------
-  [Logowanie się](/pl/coordination/tasking-manager3-project-admin/#logging-in-&amp;amp;-access-levels)  
-  [Zainicjuj nowy projekt - zdefiniuj obszar zainteresowania](/pl/coordination/tasking-manager3-project-admin/#initiate-a-new-project-within-tm3)  
-  [Tworzenie zadania - podziel obszar zainteresowania](/pl/coordination/tasking-manager3-project-admin/#initiate-a-new-project-within-tm3)
-  [Utwórz projekt - określ, co Twoi użytkownicy powinni wiedzieć](/pl/coordination/tasking-manager3-project-admin/#create-the-project)
    -  [Opis - pierwsza rzecz, której użytkownicy dowiadują się o Twoim projekcie](/pl/coordination/tasking-manager3-project-admin/#description)
    -  [Wskazówki - co użytkownicy powinni zrobić](/pl/coordination/tasking-manager3-project-admin/#instructions)
    -  [Metadane - do czego należy projekt](/pl/coordination/tasking-manager3-project-admin/#metadata)
    -  [Obszary priorytetowe - gdzie użytkownicy powinni zacząć mapowanie](/pl/coordination/tasking-manager3-project-admin/#priority-areas)
    -  [Podkład - baza do mapowania](/pl/coordination/tasking-manager3-project-admin/#imagery)
    -  [Uprawnienia - kto jest dopuszczony do mapowania i weryfikowania](/pl/coordination/tasking-manager3-project-admin/#permissions)
    -  [Użyteczne wskazówki - jak powinieneś wypełnić te wszystkie pola](/pl/coordination/tasking-manager3-project-admin/#instruction-notes)
    -  [Opublikuj - nie zapomnij, albo nigdy nie będziesz miał skończonej pracy](/pl/coordination/tasking-manager3-project-admin/#proofread-and-publish)

OpenStreetMap Tasking Manager jest niezbędny do przeprowadzania mapathonów, zarządzania aktywacjami HOT lub tworzenia zadań mapowania dla uczniów. Tasking Manager dzieli pracę na łatwe do opanowania geograficznie kawałki, które zmniejszają konflikty edycyjne, zwłaszcza przy dużej liczbie rozproszonych maperów. Tasking Manager wspiera również dokładność mapowania i jakość danych poprzez dostarczanie zwięzłych zestawów instrukcji dla maperów (np. 'zmapuj wszystkie drogi i budynki'). W skrócie, Tasking Manager jest tym, co kieruje pracami przy otwartych działaniach mapowania. Ten moduł opisuje podstawy administracji OSM Tasking Managera dla udanych wydarzeń mapowania. 

 Ten przewodnik jest napisany zwłaszcza dla tych osób, które potrzebują wskazówek o administracji w OSM Tasking Managerze, w tym o tworzeniu i modyfikowaniu projektów mapowania dla otwartych wydarzeń mapowania, np. 'mapathonów'. Ten przewodnik ma zastosowanie konkretnie do instancji OSM Tasking Managera w wersji 3, w tym [HOT Tasking Manager](http://tasks.hotosm.org) i [TeachOSM Tasking Manager](http://tasks.teachosm.org).

 HOT lub OSM Tasking Manager wersja 3 jest często określany jako **TM3,** jako skrót od Tasking Manager, wersja 3.

## Logowanie się i poziomy dostepu

Pierwszą rzeczą jest zrozumienie poziomów dostępu. Każdy dostęp do TM3 jest autoryzowany poprzez [stronę OpenStreetMap](https://www.openstreetmap.org). Aby uzyskać dostęp do TM3 potrzebujesz konta OpenStreetMap (OSM). Jeżeli masz już to konto, odwiedź [Tasking Manager](http://tasks.hotosm.org) i kliknij **Zaloguj do OpenStreetMap**, co przekieruje Cię z powrotem na stronę OSM, gdzie możesz autoryzować Tasking Managera, aby miał ograniczony dostęp do Twojego konta OSM. 

### Poziomy dostępu w OSM Tasking Managerze

OSM Tasking Manager ma trzy poziomy dostępu użytkownika:
-  **Użytkownik** - Najbardziej podstawowy poziom. Użytkownik może się zalogować do TM3 i używać jego funkcji do znalezienia i wybrania projektu mapowania do pracy. Ten poziom użytkowania jest w pełni opisany w [Przewodniku OSM Tasking Manager w LearnOSM](/pl/coordination/tasking-manager-3/). Zauważ, że niektóre projekty takie, jak będące w stanie szkicu (np. nieopublikowane) są niewidoczne dla użytkowników.  
-  **Menadżer projektu** - Menadżerowie projektów mają dostęp do tworzenia i aktualizowania projektów w TM3.  
-  **Administrator** - Administratorzy mają dostęp umożliwiający im zarządzanie poziomami dostępu użytkowników w TM3.

Potrzebujesz poziomu dostępu Menadżer projektu, aby tworzyć nowe projekty przy użyciu TM3.

## Zainicjuj nowy projekt w TM3 

![TM New][]

Kliknij swoją nazwę użytkownika w prawym górnym rogu, a następnie **Utwórz nowy projekt.** Możesz wybrać pomiędzy rysowaniem obszaru zainteresowania (AOI) na mapie, a zaimportowaniem obszaru zainteresowania z pliku geojson;  

> Importowanie pliku ze zdefiniowanym obszarem jest zawsze preferowane przed ręcznym rysowaniem projektu Tasking Managera. Narzędzia takie, jak JOSM, QGIS, itd. mogą być użyte do utworzenia plików do zaimportowania w Tasking Managerze. Sugerowana ścieżka, to utworzenie pliku .osm z AOI przy użyciu JOSM i wygenerowanie przez http://geojson.io/ pliku GeoJSON.

### Wyrysuj obszar zainteresowania do zmapowania

1. Kliknij przycisk 'Rysuj' w prawym górnym rogu.
2. Aby narysować wielokąt przestawiający AOI na mapie przytrzymaj prawy przycisk myszy i przesuwaj mapę bez klikania, co doda węzeł. Wielokąt powinien ściśle obramować obszar zainteresowania. Zaoszczędzi to czas na uzupełnianie kafelków, które są nieistotne (np. ocean, las)  
3. Kliknij na punkcie początkowym, aby ukończyć wielokąt  
4. Po skończeniu wielokąta możesz przesuwać węzły lub dodawać nowe, aby otrzymać dokładnie taki obszar, jaki chcesz.

lub

### Prześlij plik GeoJSON lub KML z obszarem zainteresowania do zmapowania  

1. Kliknij przycisk "Importuj",  
2. W oknie przesyłania przejdź do swojego pliku,  
3. Kliknij nazwę pliku, aby go podświetlić i kliknij 'Otwórz'.  
4. Zaimportowane obszary zainteresowania nie mogą być edytowane.


## Tworzenie zadania

AOI projektu jest dużym obszarem do zmapowania. Obszar ten jest podzielony na mniejsze kawałki nazywane zadaniami. 

AOI określony poprzez przesłanie pliku lub ręczne rysowanie pojawi się na mapie, a wtedy zostaniesz poproszony o wybranie sposobu podzielenia go na indywidualne zadania. Są na to dwie możliwości:  

1. Kwadratowa siatka - Tasking Manager podzieli równomiernie cały obszar projektu na kwadraty o takich samych wymiarach. Jest to zazwyczaj dobry pomysł dla ogólnych projektów wspólnego mapowania.
2. Dowolne geometrie - Jeżeli wgrywasz plik określający obszar Twojego projektu, możesz również w nim zawrzeć kształty poszczególnych zadań. Mogą pojawić się specjalne potrzeby, żeby tworzyć zadania o nieregularnych kształtach. Na przykład projekt importu dróg może wymagać dopasowanych kształtów zadań lub powstaną one w wyniku procesu redukcji AOI.

### Używanie kwadratowej siatki do zadań w kwadratch

Aby utworzyć jednolite kwadratowe kafelki, wybierz opcję Kwadratowa siatka.  

![TM Tile Sizes][]

AOI jest automatycznie dzielony na siatkę komórek, a każda komórka staje się zadaniem. Określ optymalny rozmiar kafelków używając przycisków "Większe" i "Mniejsze", aby dopasować je do rozmiarów zadań. Mniejszy rozmiar kafelków oznacza więcej zadań. Optymalny rozmiar kafelków zależy jednocześnie od wielkości obszaru (twórz mniejsze kafelki dla dużych projektów) i liczby obiektów, które powinny być zmapowane w każdym z nich. Generalnie rzecz biorąc, im większy jest AOI i/lub liczba pożądanych obiektów, tym mniejsze powinny być kafelki. 

Zauważ, że **przy określaniu rozmiaru kwadratów zadań jest dostępnych do użycia wiele warstw mapy**. Przycisk w prawym dolnym rogu mapy dostarcza listę opcji dla warstw mapy. Prawdopodobnie najlepszą opcją jest wybranie jednego z podkładów, ponieważ pozwala Ci zobaczyć aktualny obraz tego, co będzie mapowane.

Jeżeli masz własny podkład dla projektu, możesz go również załadować używając przycisku w prawym górnym rogu mapy i podając url do TMS lub WMS.

Możesz także utworzyć zadania w kilku różnych rozmiarach używając narzędzi "Podziel". Kwadraty zadań mogą być dzielone wiele razy. Ponownie, użycie warstwy podkładu pomoże Ci zdecydować, gdzie zadanie wymaga podzielenia. Przycisk "Resetuj" zresetuje wszystkie podzielone zadania. Opcja Podziel (wielokąt) pozawala narysować wielokąt nad obszarem, aby utworzyć mniejsze zadania, a Podziel (punkt) pozwala wybrać pojedyncze zadania do podziału. Przycisk Reset usuwa wszystkie Twoje niestandardowe podziały.

> Ogólnie, powinieneś używać mniejszych kafelków nad gęsto zabudowanymi obszarami mieszkalnymi. Celem powinno być utworzenie zadań, które da się wykonać w 10-15 minut.

***Rozważania przed podjęciem decyzji o rozmiarze kafelków***

-  Całkiem nowy maper na mapathonie mapuje obszar około cztery razy wolniej niż doświadczony (wielu zaczyna dużo wolniej, ale wkrótce przyspiesza). 
-  Nowy maper uważa, że trudno jest znaleźć na podkładzie satelitarnym obiekty, które inni dostrzegają. Znajdowanie okrągłych chat krytych strzechą na obszarze okrągłych krzaków jest trudnym procesem uczenia się dla 'nowicjusza'.
-  Nowy maper uważa również, że wiele obiektów trudno jest odwzorować, jak np. budynki.
-  Później w tym procesie masz możliwość 'podzielenia' maperowi kwadratu - podzielenie go na mniejsze kwadraciki pomoże uzyskać nowemu maperowi taki rozmiar, z którym sobie poradzi.  
-  Częściami kwadratu, które sprawiają największe problemy są krawędzie i narożniki. Dlatego też mniejsze kwadraty oznaczają więcej rogów i krawędzi, co w efekcie daje duplikaty lub brakujące obiekty. Więc jest to kompromis pomiędzy tym, jakie małe zrobisz kwadraty, by ułatwić pracę nowym maperom, a wzrostem błędów z powodu dużej liczby krawędzi i narożników.
-  Kwadrat może zostać podzielony, ale nie ma możliwości połączenia kwadratów z powrotem, aby je powiększyć. Bądź uważny przy dzieleniu.
-  **Wniosek** Spróbuj samemu zmapować obszar projektu, aby zobaczyć, czy będzie łatwo i z jakie napotkasz problemy. Pomoże Ci to zdecydować o optymalnym rozmiarze kwadratu. Dopuszczaj dzielenie, ale nie bez końca - niektórzy nowi maperzy dzielą kwadraty tak długo, aż są na tyle małe, że stają się ekstremalnie trudne do mapowania.  

Po ustaleniu rozmiaru zadań, kliknij "Dalej".

### Dowolne geometrie

Jeżeli przesyłasz plik do określenia obszaru projektu, to może on dodatkowo zawierać informacje o dokładnych kształtach, jakie chcesz, aby miały indywidualne zadania. Jeżeli AOI zawiera jeden wielokąt, projekt będzie miał tylko jedno zadanie. Generalnie nie używa się tego, ale jest przydatne w konkretnych potrzebach.

Dowolne geometrie nie mogą być dzielone.

### Przycinanie obszaru projektu

Po określeniu rozmiarów zadań możesz skorzystać z opcji "Przytnij" Twój AOI. Możesz przyciąć AOI zarówno do dokładnego kształtu wielokąta, który narysowałeś lub zaimportowałeś (polecane), jak i do najbliższego kwadratu, który zawiera Twój AOI.

Po zakończeniu przycinania AOI, kliknij "Dalej".

## Utwórz projekt

Nadaj projektowi tytuł (może być edytowany na następnym ekranie) i kliknij "Utwórz"

To założy projekt w Tasking Managerze i otworzy ekran, na którym będziesz mógł podać opis, wskazówki i inne informacje o projekcie. Pamiętaj, że nie możesz tego lekceważyć. Spora część maperów (w wielu przypadkach większość) nie będzie miała wcześniejszego doświadczenia z OpenStreetMap i/lub HOT, więc nie będą zaznajomieni z wytycznymi dotyczącymi tagowania. Jest bardzo ważne, żeby cele projektu są jasno określone i wszystko, co maperzy powinni wziąć pod uwagę jest przedstawione tutaj. Często zaleca się, aby umieścić w projekcie jedną klasę obiektów do zmapowania. Jeżeli potrzebujesz podstawowej mapy obszaru, lepiej jest podzielić to na kilka projektów: jeden dla dróg, jeden dla budynków, itd. Wtedy początkujący będą mogli skupić się na małej klasie obiektów w czasie nauki prawidłowego mapowania. W przeciwnym wypadku możesz zostać z mnóstwem kafelków, które zawierają po trochu wszystkiego, ale nic rzeczywiście kompletnego.

Po utworzeniu projektu, będziesz mógł edytować wszystkie powiązane z nim ustawienia:

- Opis - Używany do wyświetlenia na liście i informacji motywujących maperów
- Wskazówki - Szczegółowe wskazówki co i jak mapować, potrzebne obiekty/wystąpienia/cechy
- Metadane - Dodatkowe informacje używane do kategoryzowania projektu. Często używane przy filtrowaniu całej listy projektów.
- Podkład - Miejsce do wprowadzenia adresu URL TMS i wymaganej licencji.
- Obszary priorytetowe - Pozwala określić części projektu, które powinny być zmapowane jako pierwsze.
- Uprawnienia - Pozwala Ci ograniczyć dostęp do mapowania i weryfikowania projektu.
- Ustawienia - Termin realizacji projektu i szablon JOSM.
- Akcje - Wyślij wiadomości do twórców, weryfikuj i odrzucaj cały projekt jednym kliknięciem.

### Opis

![TM Description][]

Ten ekran pozwala Ci ustawić priorytet projektu, jego status jako szkic, opublikowany lub zarchiwizowany, krótki opis używany na liście projektów i długi opis dostępny po wybraniu projektu przez mapera.

Zarówno krótki, jak i długi opis powinny zawierać informacje o tym dlaczego projekt istnieje, kto będzie używał danych i spodziewany wpływ, jaki będzie miało mapowanie. Te pola wspierają formatowanie Markdown oraz mogą zawierać obrazy i filmy.

### Wskazówki

![TM Instructions][]

**Wystąpienia do zmapowania** - Lista obiektów, które chcesz, aby użytkownicy zmapowali. Ogólnie, im mniej obiektów tym lepiej, jako że łatwiej o ukończenie.

> Projekty, które wymagają zmapowania wielu wystąpień są trudne dla maperów i trudne do zweryfikowania. Zajmują więcej czasu, aby uzyskać z nich dobry zestaw danych. Rozmiar zadań też ma wpływ na wydajność przy różnych typach mapowania, np. budynki wymagają mniejszych kwadratów zadań, drogi i rzeki większych. Tworzenie wielu projektów na tym samym obszarze, osobno dla budynków i dla obiektów liniowych, jest najlepszą praktyką.

**Komentarz zestawu zmian** - To jest domyślny komentarz zestawu zmian, który zostanie dodany do wszystkich danych wysyłanych do OSM. Zazwyczaj zawiera coś, co określa, na jakim Tasking Managerze znajduje się projekt i obiekty, które zostały zmapowane. Jest zazwyczaj używany do "hasztagów", aby pomóc zidentyfikować potrzebującą organizację i/lub mapujących. Może też opisywać, co zostało zmapowane, np. "Mapowanie budynków".

> Użytkownicy powinni być poinstruowani, aby wypełniać sensownie komentarze o tym, co zmapowali, ale pomaganie im odpowiednim komentarzem domyślnym jest zawsze dobrym pomysłem.

**Szczegółowe wskazówki** - To jest miejsce, gdzie znajdzie się większość Twoich szczegółowych wskazówek, które, mamy nadzieję, każdy maper i weryfikator przeczyta dokładnie i będzie ich przestrzegał.

Zobacz poniższe uwagi o tworzeniu dobrych wskazówek.

**Instrukcje na zadanie** - To będzie wyświetlone, kiedy maper wybierze zadanie, a także ma specjalną funkcję, która pozwala na tworzenie specyficznych dla zadania adresów URL bazujących na współrzędnych x, y, z "uproszczonej mapy".

### Metadane

![TM Metadata][]

> Wszystkie te pola powinny być wypełnione i będą wymagane w przyszłych wersjach TM3.

**Poziom mapera** - To jest wskaźnik trudności projektu mapowania. Są 3 opcje do wyboru początkujący, pośredni i zaawansowany. To ustawienie wskazuje maperowi, jaki poziom doświadczenia powinien mieć, aby pomyślnie ukończyć projekt mapowania. Może być używany w filtrowaniu listy projektów, a na ekranie uprawnień można określić sugerowany poziom, który może być wymagany.

**Rodzaj mapowania** - Używany w filtrowaniu listy projektów i pomaga maperom znaleźć projekty, jakie lubią mapować.

**Organizacja** - Pozwala Ci określić organizację, która będzie używać zmapowanych danych. Używane w filtrowaniu projektów.

**Kampania** - To pozwala Ci połączyć projekt z innymi, które są częścią większego wysiłku mapowania. Używane w filtrowaniu listy projektów.

### Obszary priorytetowe

![TM Priority Area][]

Użyj dostępnych narzędzi do narysowania obszarów, które powinny być zmapowane w pierwszej kolejności. Możesz mieć wiele obszarów priorytetowych w projekcie. Możesz je również zmieniać w każdej chwili.

> Podczas mapowania katastrof, na początku wydarzenia, posiadanie dużego obszaru zainteresowania i używanie obszarów priorytetowych do skupienia się na nadchodzących informacjach jest najlepszym podejściem.

### Podkład

Pole URL - Pole, w którym podajesz URL do TMS, który zostanie automatycznie zastosowany w edytorze OSM, którego używa maper lub weryfikator. Zwróć uwagę na przykład, ponieważ jest bardzo ważne, żeby link był sformatowany prawidłowo, aby działał we wszystkich edytorach.

Licencja - Opcjonalnie, jeżeli jest wymagana specyficzna licencja, którą musi zaakceptować maper, możesz ją wybrać tutaj. Jeżeli potrzebujesz licencji, która jest niedostępna, skontaktuj się z administratorem instalacji Tasking Managera i poproś go o dodanie jej.

### Upoważnienia

![TM Permissions][]

Poziom mapera - Pozwala Ci ustawić wymóg posiadania odpowiedniego poziomu przez mapera do pracy w tym projekcie (ekran Metadane powyżej). Poziomy maperów mogą być ustawiane ręcznie, ale są automatycznie przypisywane na podstawie ilości zestawów zmian.

Wymagaj roli weryfikatora - To pozwala Ci wymagać, aby ludzie weryfikujący, byli sprawdzeni i zakwalifikowani jako weryfikatorzy. Uznanie kogoś za weryfikatora, menadżera projektu jest procesem wzajemnej oceny, więc istniejący weryfikatorzy mogą oznaczyć każdego użytkownika jako sprawdzonego weryfikatora.

Prywatny projekt - To ograniczy dostęp do projektu tylko dla listy użytkowników. Użytkownik musi przynajmniej raz zalogować się do Tasking Managera, zanim będzie można dodać go do projektu.

### Ustawienia

Domyślne ustawienia regionalne - Umożliwia ustawienie domyślnego języka instrukcji dla projektu.

### Działania

![TM Actions][]

Powiadom wszystkich współtwórców - Wysyła wiadomość w Tasking Managerze do wszystkich, którzy oznaczyli zadania jako ukończone lub zweryfikowane. Można tego użyć, aby podziękować i/lub wskazać twórcom inne projekty w portfolio/kampanii. Może też być użyte przed wybraniem opcji Weryfikuj/Odrzuć wszystkie zadania opisanej poniżej.

Zweryfikuj wszystkie zadania - To oznaczy "zielonym" zweryfikowanym statusem wszystkie zadania, z wyjątkiem tych, które są oznaczone jako "Zły podkład"

Odrzuć wszystkie zadania - To oznaczy "czerwonym" odrzuconym statusem wszystkie zadania, z wyjątkiem tych, które są oznaczone jako "Zły podkład"

Usuń projekt - To usunie całkowicie projekt z Tasking Managera.

Klonuj projekt - To utworzy duplikat projektu z wyjątkiem obszaru zainteresowania, który będziesz musiał ponownie zaimportować lub narysować.

### Wskazówki

Używaj prostego języka, ponieważ angielski może nie być ojczystym językiem dla Twojej docelowej grupy.

1. Tytuł projektu powinien ujawniać, co jest do zmapowania. Preferowane są tytuły takie, jak
*#1396 - Missing Maps: stan Niger (północ), Nigeria (projekt 1: drogi i obszary zamieszkane)*
2. Najważniejsze wiadomości powinny pojawić się na karcie z informacjami, aby zagwarantować ich przeczytanie. Trzeba też zawrzeć tam specjalny podkład do użycia zamiast Binga. Pierwsze zdania mogą mówić, na przykład o tym, że nie jest wymagane odwzorowanie każdego budynku jeżeli jest to projekt dotyczący dróg i obszarów zamieszkanych. Lub trzeba zmapować każdy dom, jeżeli projekt ma być użyty do oszacowania gęstości zaludnienia. To są wiadomości, które powinny pojawić się również na karcie opisu.
3. Inne punkty wyjaśniające: Jeżeli projekt jest odpowiedni tylko dla maperów z konkretnym poziomem doświadczenia. Na przykład projekt używa importów albo istniejące dane powinny być dopasowane do śladów GPS albo innego podkładu (por. z poprzednią sekcją). Wyjaśnij, że nowi maperzy powinni czuć się zaproszeni do innych projektów, ale prosisz o wyrozumiałość i zrozumienie, że w tym wystąpieniu potrzebne są zaawansowane techniki.
4. Istnieją wytyczne, które opisują typowe błędy popełniane przy weryfikowaniu. Jednym z przykładów jest kompilacja Blake'a Girardota o [mapowaniu w Zachodniej Afryce](http://wiki.openstreetmap.org/wiki/User:Bgirardot/West_African_HOT_Mapping_Tips). Użyj tego linku we wskazówkach i wyjaśnij, że wymagane jest stosowanie się do tych wytycznych.
5. Ostatecznym źródłem tagowania jest [OpenStreetMap wiki](http://wiki.openstreetmap.org/wiki/Pl:Map_Features). Dla wielu zadań powiązanych z HOT strona [tagowanie dróg w Afryce](http://wiki.openstreetmap.org/wiki/Highway_Tag_Africa) jest odpowiednią i mocno polecaną lekturą dla każdego mapera. Jeżeli Twój projekt musi odpowiadać różnym standardom tagowania, napisz podobną stronę w wiki i zalinkuj ją w swoich wskazówkach.


### Rozważania o podkładzie

W większości przypadków używamy "standardowego" podkładu Bing. Ale są pewne sytuacje, w których możesz chcieć wybrać inne źródło:

1. Bing nie dostarcza pokrycia Twojego obszaru zainteresowania w wysokiej rozdzielczości.
2. Bing ma sporo chmur w tym obszarze.
3. Potrzebujesz nowszego podkładu do oceny sytuacji po katastrofie.

Jeżeli Bing nie jest odpowiedni, następnym wyborem jest Mapbox. Powinieneś szukać innych źródeł jeśli żadne z tych dwóch nie spełniają Twoich wymagań.

W takich przypadkach nie wystarczy tylko wybrać źródła o odpowiedniej licencji i udostępnić go przez usługę WMS lub TMS. Twój obszar zainteresowania prawdopodobnie jest już częściowo zmapowany przy użyciu podkładów Bing lub Mapbox i może pojawić się znaczące przesunięcie pomiędzy tymi obrazami. Musisz dokładnie przyjrzeć się różnym miejscom w Twoim obszarze zainteresowania i określić przesunięcie pomiędzy Twoim podkładem i wcześniej zmapowanymi danymi. Jeżeli istniejące dane OSM są nieznacznie przesunięte w stosunku do Twojego podkładu, ale pasują do Binga, to zazwyczaj przyjmujemy, że Bing jest "złotym standardem", dopóki nie mamy śladów GPS, które zaprzeczą temu założeniu.

Jeżeli przesunięcie pomiędzy Twoim podkładem, a Bingiem jest stałe w całym obszarze zainteresowania, to można to skorygować na serwerze tak, że obrazy z różnych źródeł załadowane do edytora będą do siebie pasować. Jeżeli to nie jest możliwe, jeżeli przesunięcie jest zmienne lub istniejące dane są dopasowane do różnych źródeł, to przychodzi czas na plan B:

Ważnym zadaniem dla Ciebie jest to, że musisz przemyśleć, jak poradzić sobie z tymi problemami i dostarczyć szczegółowe instrukcje maperom i weryfikatorom. Zdecydowanie polecamy określenie takiego projektu jako "tylko dla doświadczonych maperów" i wyjaśnienie, że doświadczenie, w tym wypadku, nie oznacza zmapowania 200+ budynków, ale umiejętności radzenia sobie z problemami dopasowania i różnymi źródłami podkładów.

Jedna z możliwych strategii może składać się z następujących kroków:

1. Jasno określ, który podkład jest brany jako odniesienie, do którego wszystko inne powinno być dopasowane. W tym przykładzie załóżmy, że bazą jest Bing.
2. Upewnij się, że wszystkie istniejące obiekty, widoczne na podkładzie Bing, są do niego wyrównane, ew. je dopasuj ponownie.
3. Dopasuj alternatywny podkład do istniejących obiektów (a więc do Binga) używając funkcji przesunięcia podkładu w edytorze.
4. Od teraz możesz dodawać nowe obiekty prawidłowo wyrównane do swojego podkładu.

Jest ważne, aby krok 3 powtórzyć dla każdego zadania w projekcie, a pojedyncze kwadraty zadań nie powinny być zbyt duże, ponieważ przesunięcie podkładu może być zmienne w obszarze zainteresowania, zwłaszcza jeśli teren nie jest płaski. Nawet nieciągłości podkładu mogą się zdarzyć w projekcie - sprawdź to i ewentualnie ostrzeż twórców o takim problemie.

Tutaj jest kilka sugerowanych kawałków informacji, które możesz zawrzeć we wskazówkach do projektu:

- [ogólne wytyczne dla różnych edytorów](https://wiki.openstreetmap.org/wiki/Using_Imagery)
- [animowany gif o wyrównywaniu podkładu w iD](https://wiki.openstreetmap.org/w/images/1/1a/Id-adjust-imagery.gif)
- [rozdział learnOSM o wyrównywaniu podkładu w josm](http://learnosm.org/pl/josm/correcting-imagery-offset)


### Sprawdzenie i publikowanie
Sprawdź różne zakładki, aby upewnić się, że słownictwo i formatowanie jest prawidłowe, a wskazówki są jasne. Jeżeli potrzebujesz wprowadzić zmiany albo poprawić swój projekt, kliknij link 'Edytuj' w prawym górnym rogu strony. 
Jeżeli projekt jest gotowy do mapowania, kliknij link 'Opublikuj'. Kiedy projekt zostanie opublikowany, staje się dostępny do mapowania dla każdego, kto ma konto OSM, chyba że została określona grupa użytkowników na karcie 'Dozwoleni użytkownicy', to tylko oni będą mogli pracować nad projektem. Jeżeli pojawi się taka potrzeba, zmiany w projekcie mogą być wprowadzane po opublikowaniu poprzez kliknięcie linku 'Edytuj'.

[TM Tile Sizes]: /images/coordination/tm3_tile_sizes.png
[TM New]: /images/coordination/tm3_create_new.png
[TM Description]: /images/coordination/tm3_description.png
[TM Instructions]: /images/coordination/tm3_instructions.png
[TM Metadata]: /images/coordination/tm3_metadata.png
[TM Priority Area]: /images/coordination/tm3_priority_area.png
[TM Permissions]: /images/coordination/tm3_permissions.png
[TM Actions]: /images/coordination/tm3_actions.png