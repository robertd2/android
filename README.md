# android
Android project

Projekt jak do tej pory udało mi się zakończyć na części GUI oraz odczyt danych z serwera + wysyłka wiadomości
GUI troszkę zmieniłem w odniesieniu do oryginału:
- zmieniłem kolory w stosunku do tego, co zostało zaproponowane - możliwe do zmiany w każdym momencie
- na górze ekranu znajduje się "fragment" zawierający nazwę pomieszczenia - nazwa zostanie pobrana z serwera podczas inicjacji;
- środkowy fragment odpowiedzialny jest za wyświetlanie dostępności pomieszczenia, w ramach dostępności wprowadziłem nastęujące statusy pomieszczeń: AVAILABLE, RESERVED, OCCUPIED oraz odpowiednie kolory. Zanim zostanie ustawiony status dostępności, pierwotnym statusem jest UNKNOWN - będzie się wyświetlał w przypadku braku komunikacji z serwerem lub przed inicjacją danych
- dolny fragment ekranu, nazwany panelem z opcjami - TO DO - będzie zawierał wszelkie dodatkowe potrzebne infrmacje oraz opcje w zależnoci od statusu sali konferencyjnej - widoki TO DO; aktywności TO DO
- na samym dole ekranu, zielony pasek to przycisk, który symuluje na sztywno przykładowe dane przesłane przez serwer; po kolejnych przyciśnięciach zmieniają się statusy sali - do usunięcia po zrealizowaniu komunikacji
- w klasie MainActivity metody: sendMessage oraz connectWebSocket służą do komunikacji
- w metodzie connectWebsocketDummy generowane są przykładowe dane
