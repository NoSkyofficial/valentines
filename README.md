# Walentynkowa strona

Jednostronicowa strona z interakcjami, zbudowana w jednym pliku `index.html` (HTML, CSS i JavaScript bez bibliotek i bez procesu budowania).

## Co pokazuje strona

1. **Pytanie** - ekran z przyciskami „TAK" i „Nie…". Przy każdym kliknięciu „Nie" przycisk się zmniejsza i zmienia treść; po sześciu kliknięciach znika.
2. **Przejście** - po kliknięciu „TAK" pojawia się animacja serc, a następnie odsłaniają się pozostałe ekrany.
3. **Kapsuła czasu** - odtwarzacz Spotify (utwór startuje po kliknięciu „TAK") oraz karuzela zdjęć z podpisami i datami. Karuzela przełącza się automatycznie co 6 sekund; obsługuje strzałki, kropki i przesunięcie palcem na ekranie dotykowym.
4. **Licznik** - dni, godziny, minuty i sekundy od daty `RELATIONSHIP_START`, aktualizowane co sekundę.
5. **Quiz** - siedem pytań z informacją zwrotną po każdej odpowiedzi i wynikiem końcowym.
6. **List** - po kliknięciu przycisku na końcu strony list pisze się znak po znaku, a na końcu pojawia się serce.

## Uruchomienie

Otwórz plik `index.html` w przeglądarce. Nie trzeba instalować zależności ani uruchamiać serwera.

Strona korzysta z internetu: czcionki są ładowane z Google Fonts, a odtwarzacz Spotify jest osadzony z `open.spotify.com`.

## Konfiguracja

Ustawienia znajdują się na początku bloku `<script>` w `index.html`:

- `RELATIONSHIP_START` - data startu licznika
- `SPOTIFY_TRACK_ID` - identyfikator utworu w Spotify
- `PHOTOS` - lista zdjęć karuzeli (`src`, `caption`, `date`). Pliki zdjęć mają leżeć obok `index.html`. Jeśli wpis nie ma `src`, zamiast zdjęcia pokazywany jest tekst zastępczy.
- `QUIZ_QUESTIONS` - pytania quizu (`question`, `options`, `correctIndex`, `feedback`)
- `LOVE_LETTER` - treść listu

## Pliki

| Plik | Opis |
|---|---|
| `index.html` | cała strona: HTML, CSS i JavaScript |
| `wakacje.JPG`, `zachod.JPG`, `lazienki.JPG`, `swieta.JPEG`, `dzien.JPG` | zdjęcia używane w karuzeli (wpisy `PHOTOS`) |
| `IMG_4114.JPEG` | zdjęcie w repozytorium, którego strona nie używa |
