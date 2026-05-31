# 🎮 Emilka — Łowczyni Wiedzy

Jednoplikowa gra edukacyjna dla dzieci **4–6 lat**, działająca w przeglądarce (najlepiej na tablecie). Cała aplikacja to jeden plik `index.html` — bez instalacji, offline-friendly.

![styl](https://img.shields.io/badge/styl-Duolingo%20dla%20dzieci-ff4d9d) ![tech](https://img.shields.io/badge/tech-HTML%2BCSS%2BJS-22bfe6)

## ✨ Co potrafi

- **4 kategorie nauki**, każda z własną **mapą 30 poziomów** (ścieżka w stylu Duolingo):
  - 🔤 **Literki** — rozpoznawanie liter, dopasowanie litera↔obrazek, *wpisz brakującą literę*, *napisz słowo z obrazka* (własna klawiatura ekranowa)
  - 🔢 **Liczby** — liczenie, dopasowanie ilości, większa liczba, **dodawanie i odejmowanie**, brakująca liczba
  - 🧩 **Zagadki** — co nie pasuje (kolor / kształt / kategoria), wzory/sekwencje
  - 🤔 **Prawda/Fałsz** — ~116 ciekawostek w 11 tematach, z **uzasadnieniem** i progresją trudności
- ⭐ **Gwiazdki 1–3 za poziom** (zależnie od błędów) — waluta do odblokowań
- 🗣️ **Polski lektor** (Web Speech API) z **wyborem głosu** i preferencją głosu żeńskiego/naturalnego
- 👗 **Szatnia** — 6 stylów postaci (mała blondynka Emilka), 7 kolorów włosów, tła, zwierzaki-towarzysze, 4 czcionki, wybór głosu
- 🔓 Odblokowania za gwiazdki, 📊 **statystyki** dzienne/tygodniowe, 🏆 **osiągnięcia**
- 📐 Działa **pionowo i poziomo**, duże przyciski dotykowe, brak „Game Over"
- 💾 Zapis postępów w `localStorage`

## ▶️ Jak uruchomić

Najprościej — otwórz `index.html` w przeglądarce. Możesz też wystawić lokalny serwer:

```bash
node serve.js     # http://localhost:8795
```

Na tablecie warto dodać stronę do ekranu głównego (działa jak aplikacja). Dźwięk włącza się po pierwszym dotknięciu (wymóg przeglądarek).

## 🛠️ Technologia

- Czysty **HTML + CSS + JavaScript** (jeden plik, brak zależności)
- Postacie i kształty rysowane jako **inline SVG**
- Mowa: **Web Speech API** (`pl-PL`)
- Czcionki: Google Fonts (Fredoka / Baloo / Poppins / Comfortaa) — przy 1. uruchomieniu wymagają internetu, potem działają z cache

## 🗺️ Status

Wersja rozwojowa. `index.html` zawiera flagę `UNLOCK_ALL` (testowo odblokowuje wszystkie poziomy — ustaw `false`, aby przywrócić progresję poziom-po-poziomie).

---
Tworzone z ❤️ dla Emilki.
