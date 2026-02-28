# 📖 Almanach - Gothic Axyl Helper

**Almanach** to zewnętrzny asystent, nakładka (overlay) oraz zbiór makr stworzony z myślą o optymalizacji rozgrywki w grze Gothic (dedykowany pod serwer Axyl). Program działa w tle, nie ingeruje bezpośrednio w pamięć gry i posiada w pełni zautomatyzowany system aktualizacji.

---

## ✨ Główne funkcje

* ⏱️ **Bestiariusz (System Timerów)**
  Wbudowane odliczanie do respawnu bossów na poszczególnych mapach (np. Jarkendar, Valendor). Program dyskretnie powiadamia gracza na 5 minut przed pojawieniem się bossa, wyświetlając odpowiedni komunikat na ekranie.

* 🔔 **Dziennik (Osobiste Alarmy)**
  Koniec z zapominaniem o cyklicznych zadaniach. Możliwość ustawienia własnych alarmów (odliczanie lub konkretna godzina) przypominających np. o oddaniu przedmiotów do Biologa czy Jubilera.

* ⚔️ **Skrypty Bojowe (Makra)**
  Zoptymalizowane skrypty bojowe omijające problem kolejkowania klatek (engine Gothica). Oferują płynne ataki:
  * **1H:** Atak Lewo/Prawo
  * **2H:** Atak w przód
  * *Zalecane korzystanie na sterowaniu z Gothica 1.*

* 🖥️ **Nakładka w grze (Overlay)**
  Wszystkie informacje wyświetlane są bezpośrednio na ekranie gry. Nakładkę można w każdej chwili wywołać ręcznie za pomocą klawisza **`F10`**. W ustawieniach można dostosować przezroczystość i rozmiar czcionki.

* 🔄 **Automatyczne Aktualizacje (Auto-Patcher)**
  Program przy każdym uruchomieniu weryfikuje dostępność nowej wersji. Jeśli pojawi się aktualizacja, Almanach samodzielnie pobierze ją w tle i zaktualizuje pliki, zapewniając graczom zawsze najnowszą wersję bez konieczności ręcznego pobierania paczek.

---

## ⚙️ Instalacja i Uruchomienie

1. Przejdź do zakładki **[Releases](../../releases/latest)** po prawej stronie repozytorium.
2. Pobierz najnowszy plik **`Instalator_Almanach.exe`**.
3. Uruchom instalator (zostaniesz poproszony o uprawnienia Administratora).
4. Po zakończeniu instalacji, uruchom program za pomocą utworzonego skrótu na pulpicie.

### ⚠️ Ważne informacje

* **Uprawnienia Administratora:** Almanach musi być uruchamiany jako administrator. W przeciwnym razie system Windows zablokuje działanie makr i nakładki wewnątrz gry. Instalator automatycznie konfiguruje skróty pod tym kątem.
* **Fałszywe alarmy antywirusów:** Ponieważ program generuje wirtualne wciśnięcia klawiszy (makra), niektóre antywirusy (w tym Windows Defender / SmartScreen) mogą początkowo blokować plik. Program jest w 100% bezpieczny - w razie problemów należy dodać go do wyjątków lub kliknąć "Uruchom mimo to".

---

## 🛠️ Technologie

Projekt został zbudowany przy użyciu:
* **Python 3** - Główny język logiki.
* **PyQt6** - Interfejs graficzny (GUI) i wątki w tle.
* **Nuitka** - Kompilator do natywnego pliku `.exe` (C-level performance).
* **PyArmor** - Obfuskacja i zabezpieczenie kodu źródłowego.
* **Inno Setup** - Generowanie instalatora.

---

*Stworzone przez graczy, dla graczy.* 🍻
