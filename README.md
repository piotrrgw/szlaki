# 🚂 Szlaki Kolejowe (Railway Routes)

Kompleksowy system narzędzi webowych do zarządzania, wizualizacji i planowania tras kolejowych. Projekt służy zarówno do celów administracyjnych (tworzenie rozkładów, edycja geometrii szlaków), jak i operacyjnych (wsparcie pracy Kierownika Pociągu, wizualizacja dla użytkownika końcowego).

Aplikacja działa w oparciu o architekturę **Client-Side** (HTML/JS), wykorzystując pliki JSON jako bazę danych, co zapewnia szybkość działania i łatwość hostowania (GitHub Pages).

## 🚀 Dostępne Narzędzia

Projekt składa się z czterech niezależnych modułów:

### 1. 🗺️ Wizualizacja Trasy (Strona Główna)
Narzędzie dla użytkownika końcowego pokazujące trasowanie pociągów na mapie.
* **Funkcje:** Wybór pociągu i daty, wizualizacja przebiegu trasy na podkładzie OpenRailwayMap/OSM, statusy odcinków.
* **Link:** [Uruchom Wizualizację](https://piotrrgw.github.io/szlaki/) (`index.html`)

### 2. 📋 Kontrolka Kierownika Pociągu
Narzędzie operacyjne pozwalające Kierownikowi Pociągu w łatwy sposób uzupełnić dokument *"KARTA ZNAJOMOŚCI INFRASTRUKTURY KOLEJOWEJ I BOCZNIC"*.
* **Funkcje:** Automatyzacja wypełniania dokumentacji, szybki dostęp do danych o szlaku.
* **Link:** [Otwórz Kontrolkę](https://piotrrgw.github.io/szlaki/kontrolka.html) (`kontrolka.html`)

### 3. 🚆 Manager Pociągów (Panel Administratora)
Narzędzie pozwalające administratorowi repozytorium zarządzać bazą pociągów (`trains.json`).
* **Funkcje:** Tworzenie nowych pociągów, definiowanie ich trasowania, zarządzanie kalendarzem kursowania.
* **Link:** [Zarządzaj Pociągami](https://piotrrgw.github.io/szlaki/train_menager.html) (`train_menager.html`)

### 4. 🛠️ Kreator Szlaków (Edytor Geometrii)
Zaawansowane narzędzie administratora do edycji bazy szlaków (`szlaki_master.json`).
* **Funkcje:** Tworzenie nowych definicji szlaków, rysowanie geometrii na mapie (Leaflet Draw), eksport danych do JSON, walidacja spójności bazy.
* **Link:** [Edytor Szlaków](https://piotrrgw.github.io/szlaki/creator_szlaki.html) (`creator_szlaki.html`)

---

## 💻 Technologie

Projekt został zbudowany z naciskiem na dostępność i responsywność:
* **HTML5 / CSS3:** Pełna zgodność ze standardami **WCAG** oraz **EAA**. Interfejs przygotowany zgodnie z zasadami **RWD** (Responsive Web Design) – działa na komputerach i urządzeniach mobilnych.
* **JavaScript (ES6+):** Czysty JS bez ciężkich frameworków.
* **Leaflet.js:** Obsługa map interaktywnych.
* **JSON:** Przechowywanie danych o pociągach i geometrii szlaków.

## 📂 Struktura Plików

* `index.html` - Główny widok aplikacji - wizualizacja tras jazdy pociągów.
* `trains.json` - Baza danych pociągów z ich szlakami.
* `szlaki_master.json` - Baza danych geometrii i definicji odcinków.
* `kontrolka.html` - Moduł dla Kierownika Pociągu ułatwiający uzupełniania kontrolki.
* `train_menager.html` - Edytor pociągów.
* `creator_szlaki.html` - Edytor mapy oraz szlaków.

## 👥 Autorzy

* **Piotr M** 🚂 - Główny twórca, koncepcja i dane.
* **Gemini** - Wsparcie w kodowaniu i optymalizacji.

---
*Wersja aplikacji: v1.0*