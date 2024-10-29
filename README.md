**Zadanie do samodzielnego wykonania**

Przygotuj się do wykonania poniższego zadania, korzystając z podanych informacji. Zadanie polega na stworzeniu bazy danych, tabeli z przykładowymi danymi, a następnie prostej strony w PHP, która wyświetli te dane. Na koniec zmodyfikuj stronę, dodając formularz umożliwiający dodawanie nowych rekordów do tabeli.

---

### **Część 1: Tworzenie bazy danych i tabeli**

1. **Stwórz bazę danych o nazwie `sklep`.**

2. **W bazie danych `sklep` utwórz tabelę o nazwie `produkty` z następującą strukturą:**
   - `id` INT AUTO_INCREMENT PRIMARY KEY
   - `nazwa` VARCHAR(100) NOT NULL
   - `cena` DECIMAL(10,2) NOT NULL
   - `ilosc` INT NOT NULL

3. **Dodaj do tabeli `produkty` co najmniej trzy przykładowe rekordy**, np.:
   - Nazwa: "Mysz komputerowa", Cena: 49.99, Ilość: 10
   - Nazwa: "Klawiatura", Cena: 79.99, Ilość: 5
   - Nazwa: "Monitor", Cena: 599.99, Ilość: 2

---

### **Część 2: Tworzenie strony PHP wyświetlającej dane**

1. **Stwórz plik PHP**, np. `index.php`, który połączy się z bazą danych `sklep`.

2. **Na stronie wyświetl dane z tabeli `produkty` w postaci listy punktowanej**, używając elementów HTML `<ul>` i `<li>`. Każdy produkt powinien być wyświetlony jako osobny element listy zawierający nazwę produktu oraz jego cenę.

   - **Przykład wyświetlania:**
     - Mysz komputerowa - 49.99 zł
     - Klawiatura - 79.99 zł
     - Monitor - 599.99 zł

---

### **Część 3: Dodanie formularza do dodawania nowych produktów**

1. **Zmodyfikuj stronę `index.php`, dodając formularz HTML**, który umożliwi dodawanie nowych produktów do tabeli `produkty`.

2. **Formularz powinien zawierać następujące pola:**
   - Nazwa produktu (pole tekstowe)
   - Cena (pole liczby z miejscami dziesiętnymi)
   - Ilość (pole liczby całkowitej)
   - Przycisk "Dodaj produkt"

3. **Po wysłaniu formularza:**
   - Nowy produkt powinien zostać dodany do tabeli `produkty` w bazie danych.
   - Lista produktów wyświetlanych na stronie powinna zostać zaktualizowana o nowo dodany produkt.

---

### **Dodatkowe wskazówki:**

- **Połączenie z bazą danych:**
  - Użyj rozszerzenia `mysqli` lub `PDO` do połączenia z bazą danych.
  - Pamiętaj o obsłudze ewentualnych błędów połączenia.

- **Bezpieczeństwo:**
  - Zabezpiecz aplikację przed atakami typu SQL Injection, np. poprzez użycie zapytań przygotowanych (`prepared statements`).
  - Waliduj dane wejściowe z formularza przed ich przetworzeniem i dodaniem do bazy danych.

- **Estetyka i użyteczność:**
  - Stylizuj formularz i listę produktów za pomocą CSS, aby strona była bardziej przyjazna dla użytkownika.
  - Dodaj komunikaty informujące o powodzeniu lub niepowodzeniu dodania produktu.

- **Testowanie:**
  - Przetestuj dodawanie kilku produktów o różnych wartościach, aby upewnić się, że aplikacja działa poprawnie.
  - Sprawdź, czy aplikacja poprawnie obsługuje błędne dane wejściowe (np. brak wartości w polach formularza).

---

**Powodzenia w realizacji zadania!**
