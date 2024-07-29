# Zadanie 1.

HTML zawiera listę kategorii ul#categories.

Z wykorzystaniem właściwości i metod elementów DOM napisz skrypt, który:

1. Policzy i wypisze w konsoli liczbę kategorii w ul#categories, czyli elementów li.item.
2. Dla każdego elementu li.item na liście ul#categories znajdzie i wypisze w konsoli tekst nagłówka elementu (tagu h2) oraz liczbę elementów w kategorii (wszystkich li, które są w nim zagnieżdżone).

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 2

Napisz skrypt tworzący galerię obrazów na podstawie tablicy danych. HTML zawiera listę ul.gallery.

Wykorzystaj tablicę obiektów images do utworzenia elementów <img>, umieszczonych wewnątrz <li>.

Możesz utworzyć i dodać elementy HTML za pomocą document.createElement() i elem.append(), lub szablonów ciągów i elem.insertAdjacentHTML().

* Wszystkie elementy galerii powinny być dodawane do DOM w jednej operacji dodawania.
* Dodaj minimalne stylizowanie galerii za pomocą flexboxów za pomocą klas CSS.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 3

Napisz skrypt, który podczas wprowadzania tekstu do inputu input#name-input (zdarzenie input) podstawia jego bieżącą wartość do span#name-output jako imię do powitania. Upewnij się, że wartość w inpucie jest oczyszczana z białych znaków na krańcach. Jeśli input jest pusty lub zawiera tylko spacje, to zamiast imienia w spanie powinien pojawić się ciąg "Anonymous".

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 4

Napisz skrypt do zarządzania formularzem logowania.

1. Przetwarzanie wysyłania formularza form.login-form powinno odbywać się poprzez zdarzenie submit.
2. Podczas wysyłania formularza strona nie powinna być przeładowywana.
3. Jeśli podczas submit w formularzu są nieuzupełnione pola, wyświetl alert z komunikatem 'All form fields must be filled in'. Nie dodawaj atrybutu required do inputów, walidacja powinna odbywać się za pomocą JS.
4. Jeśli użytkownik wypełnił wszystkie pola i wysłał formularz, zbierz wartości pól do obiektu z dwoma właściwościami, gdzie kluczem jest nazwa inputów, a wartością są odpowiednie wartości tych inputów, oczyszczone z białych znaków na krawędziach. Do uzyskania dostępu do elementów formularza użyj właściwości elements.
5. Przy submit formularza wypisz obiekt z wprowadzonymi danymi w konsoli i zresetuj wartości pól formularza za pomocą metody reset.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 5

Napisz skrypt, który po kliknięciu na button.change-color zmienia kolor tła elementu <body> za pomocą stylu inline i przypisuje tę wartość koloru do span.color.

Aby wygenerować losowy kolor, użyj funkcji getRandomHexColor().

Zauważ, że funkcja getRandomHexColor() zwraca kolor w formacie heksadecymalnym (hex), podczas gdy kolor tła na <body> będzie w formacie rgb. To jest normalne i nie wymaga żadnych poprawek.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 6

Napisz skrypt do tworzenia i czyszczenia kolekcji elementów z następującą funkcjonalnością.


Istnieje input, do którego użytkownik wprowadza żądaną liczbę elementów. Po naciśnięciu przycisku Create powinna być renderowana (dodawana do DOM) kolekcja z odpowiednią liczbą elementów i czyścić się wartość w inpucie. Po ponownym naciśnięciu przycisku Create powinna być renderowana nowa kolekcja powyżej starej. Po naciśnięciu przycisku Destroy kolekcja elementów powinna być wyczyszczona.


Po naciśnięciu przez użytkownika przycisku Create, wartość w input musi być zwalidowana i musi mieć wartość w zakresie od 1 do 100 włącznie. Tylko wtedy nowe elementy <div> powinny być dodawane do DOM.


Aby renderować elementy na stronie, stwórz funkcję createBoxes(amount), która przyjmuje jeden parametr - liczbę, która przechowuje ilość elementów do zrenderowania. Funkcja powinna tworzyć tyle elementów <div>, ile jest podane w parametrze amount, i dodawać je do DOM jako dzieci dla div#boxes.

1. Rozmiary pierwszego elementu <div> powinny wynosić 30px na 30px.
2. Każdy kolejny element powinien być szerszy i wyższy od poprzedniego o 10px.
3. Wszystkie elementy powinny mieć losowy kolor tła. Użyj gotowej funkcji getRandomHexColor() do uzyskania losowego koloru.

Aby wyczyścić kolekcję po naciśnięciu przycisku Destroy, stwórz funkcję destroyBoxes(), która usuwa zawartość div#boxes, usuwając wszystkie utworzone elementy.

