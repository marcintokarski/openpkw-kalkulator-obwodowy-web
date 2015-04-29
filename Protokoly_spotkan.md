# Protoko�y spotka�

## Aktualna lista TODO
- Zadania programistyczne s� na [Trello](https://trello.com/b/1PocOld8/poc-wp).
- Sprawy organizacyjne
  - Kontakty mailowe do wszystkich s� w OpenProject.
  - Tomek za�o�y list� mailingow� dla frontendowc�w OpenPKW.
  - Kto nie ma konta w OpenProject, wysy�a maila do Tomka z pro�b� o dodanie.
  - Kontakty Skypowe s� w dyskusji Skypowej.
  - Kto nie jest dodany do zespo�u OpenPKW w GitHubie, przysy�a Sebastianowi swoj� nazw� konta z GitHuba i Sebastian go dodaje.
  - Kto nie jest dodany do tablicy OpenPKW w Trello, przysy�a Sebastianowi swoj� nazw� konta w Trello i Sebastian go dodaje.
- Sebastian i Tomek - uporz�dkowanie infrastruktury
  - Przeinstalowanie systemu operacyjnego na serwerze Dobromir.
  - Skonfigurowanie od nowa Continuous Delivery.
  - Skonfigurowanie �rodowiska IT (integration tests).
  - Skonfigurowanie �rodowiska UAT (testy r�czne).
  - Skonfigurowanie �rodowiska produkcyjnego (EXT? PROD?).

## 10 kwietnia 2015, Skype, 1h
Obecni: Sebastian Celejewski, Rafa� Regu�a, Krzysztof Miksa, Kacper Jasi�ski, Marcin Tokarski, Tomasz Wo�niak, Wojciech Sz�stak, Marcin Marzec, Adam Nakoneczny

Tematyka:
- Przywitanie nowych os�b.
- Bie��ca sytuacja w projekcie OpenPKW.
- Relacja pomi�dzy projektami OPW i OpenPKW. S� to dwa osobne projekty. OpenPKW tworzy oprogramowanie dla PKW, do wykorzystania przez cz�onk�w komisji wyborczych, zgodne ze wszystkimi przepisami, wytycznymi, praktykami komisji wyborczych. OPW natomiast tworzy oprogramowanie do niezale�nego od PKW weryfikowania wynik�w wyborych, wykorzystywane przez wolontariuszy, kt�rzy b�d� wprowadza� publicznie dost�pne protoko�y wyborcze do systemu. Zespo�y OpenPKW i OPW s� w wi�kszej cz�ci wsp�lne, tj. osoby tworz�ce OpenPKW tworz� r�wnie� OPW. Uwsp�lnienie dotyczy tak�e infrastruktury, tj. OpenPKW wykorzystuje serwery OPW.
- Om�wienie statusu kodu w repozytorium PocKalkulatorWyborczyHtml. Jest to prototyp, w kt�rym �wiczymy funkcjonalno��, natomiast na razie pomijamy sprawy takie, jak bezpiecze�stwo, wydajno�� itd.
- Om�wienie ostatnich zmian w kodzie (niewiele, g��wnie uporz�dkowanie backendu).
- Om�wienie obecnej i przysz�ej technologii Kalkulatora OpenPKW. Obecnie: AngularJS na frontend i Java EE na backend.
- Om�wienie funkcjonalno�ci, kt�ra jest do zaimplementowania w najbli�szej przysz�o�ci:
  - Wprowadzanie danych i walidacja.
  - Generowanie pliku PDF.
  - Eksport danych na serwer.
- Om�wienie metody wsp�lnej pracy.
  - Ka�da funkcja systemu rozwijana b�dzie na swoim branchu. Po uko�czeniu danej funkcjonalno�ci lub jakiego� jej sko�czonego zakresu robimy merge do brancha master.
  - Zmiany wprowadzamy na swoich forkach i wysy�amy pull requesty. Pull request b�dzie zweryfikowany przez innych cz�onk�w dru�yny i wtedy b�dzie wmergowany do brancha danej funkcji.
  - B�dziemy tworzy� osobne branche lub taki dla wyda� systemu.
- Om�wienie konwencji programistycznych.
   - https://github.com/johnpapa/angular-styleguide
   - http://jscs.info/
   - Od razu wprowadzamy testy.

## 27 marca 2015, Skype, 1.5h
Obecni: Sebastian Celejewski, Adam Kowalewski, Dawid Kulesza, Marcin Tokarski, Kamil Kowalski, Kacper Jasi�ski

Tematyka:
- Frontent Kalkulatora OpenPKW - budowanie, deployment
- Continuous Integration dla frontendu - potrzebny administrator Apache
- Jak generowa� PDFy? Ze wzgl�du na spory rozmiar czcionek porzucamy na razie pomys� generowania PDFu po stronie front-endu.
- Czyli: pozostaje backend w Javie.
- Dalsze kroki: uporz�dkowanie kodu frontendu, przerobienie wszystkiego na Angulara, potem dopiero robienie walidacji, generowania XMLa i generowania PDFa.

## 23 marca 2015, Skype, 2h
Obecni: Sebastian Celejewski, Adam Kowalewski, Dennis Gabriel Kruk, Adam Brzozowski, Kacper Jasi�ski, Dawid Kulesza, Adam Nakoneczny

Tematyka:
Spotkanie wprowadzaj�ce
- Kr�tka historia OpenPKW
- Co si� obecnie dzieje (prace analityczne, deweloperskie, administracyjne i organizacyjne).
- Specyfika pracy (zesp� si� formuje, ustalamy zasady, porz�dkujemy dokumentacj� itp.)
- Who is who w projekcie
- Plan dzia�ania (pierwszy etap: Kalkulator OpenPKW).
- Kalkulator OpenPKW (funkcjonalno��, technologia, deploymenty, plany itp.).
- Zaproszenie na spotkanie w �rod�.

Zadania na najbli�szy czas:
- Przerobienie prototypu HTML z aplikacji JavaEE na aplikacj� webow� (zacz�� to ju� Marcin Tokarski).
- Zaimplementowanie brakuj�cej funkcjonalno�ci (lista zada� jest w Trello: https://trello.com/b/1PocOld8/poc-wp)
- Skonfigurowanie continuous delivery dla nowej aplikacji webowej.
