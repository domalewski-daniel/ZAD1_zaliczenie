# ZAD1_zaliczenie
Zadanie 1 na zaliczenie ćwiczeń z przedmiotu Programowanie Java

Projekt: Java Spring - MVC

Opis projektu

Ten projekt to prosty przykład aplikacji webowej stworzonej przy użyciu Spring Framework. Składa się z:
Kontrolera (HelloController), który zarządza logiką aplikacji.
Pliku HTML (frontendu), który służy jako widok renderowany przez serwer z użyciem biblioteki Thymeleaf.

Struktura projektu:
- Kontroler

Plik HelloController zawiera dwie metody obsługujące żądania HTTP:
hello(): Obsługuje żądanie GET na endpoint /. Zwraca prosty tekst "Hello Vistula, in my first Spring controller!".
greeting(): Obsługuje żądanie GET na endpoint /greeting. Akceptuje parametr name, który domyślnie ustawiany jest na "World". Przekazuje tę wartość do widoku jako zmienną name i renderuje stronę HTML.

Jak działa aplikacja?:

Użytkownik wysyła żądanie HTTP GET na endpoint / lub /greeting.
Spring Framework przekierowuje żądanie do odpowiedniej metody kontrolera:

hello() dla /

greeting() dla /greeting (z opcjonalnym parametrem name)

Kontroler przetwarza żądanie i w razie potrzeby przekazuje dane do widoku (Thymeleaf).
Widok Thymeleaf generuje stronę HTML na podstawie danych z modelu i zwraca ją użytkownikowi.
