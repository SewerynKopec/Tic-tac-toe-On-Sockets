# Autorzy
[Julian H.](https://github.com/Nailu776)

[Seweryn K.](https://github.com/SewerynKopec)

# Opis projektu
Gra dla mobilnych bezprzewodowych sieci ad-hoc.
Gra Kolko i krzyzyk polegajaca na turowym wysylaniu miedzy graczami planszy z wykonanym ruchem.
Gre mozna uruchomic jako nowa rozgrywke lub dolaczyc do czekajacego gracza.
Gracze nie musza znac swoich adresow, musza jedynie znajdowac sie w tej samej sieci, gdyz plansza jest wysylana rozgloszeniowo.
Po dolaczeniu do rozgrywki, losowane sa znaki, ktorym beda poslugiwac sie gracze - X zawsze zaczyna pierwszy.

# Pliki zrodlowe

*game.c*
Plik game.c jest plikiem glowym programu. Inicjowane jest w nim gniazdo komunikacji, wybor graczy oraz
petle graczy.

*sender*
Pliki sender zawieraja ustawienia gniazda dotyczace wysylania ramek oraz budowania ich.

*receiver*
Pliki receiver zawieraja ustawienia gniazda dotyczace odbierania ramek oraz interpretowania ich zawratosci.

*tictactoe*
Pliki tictactoe odpowiedzialne sa za implementacje zasad gry, wyswietlanie plansz oraz ruchy graczy.

# Sposob uruchomienia
Program kompiluje sie poleceniem 'make'
Skompilowany program uruchamia sie nastepujacym poleceniem:
    ./game INTERFACE_NAME OPTION
Argument INTERFACE_NAME jest numerem uzywanego interfejsu sieciowego.
Argument OPTION moze przybrac wartosc START lub JOIN. Pierwsza tworzy nowa rozgrywke,
druga dolacza do czekajacego gracza.
