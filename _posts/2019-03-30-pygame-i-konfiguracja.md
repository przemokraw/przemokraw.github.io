---
layout: post
title: Piszemy grę w Pythonie I - konfiguracja środowiska
---

## Instalacja Pythona

1. Wchodzimy na oficjalną strinę Pythona [(link)](https://www.python.org/) i pobieramy najnowszą wersję
2. Podczas instalacji zaznaczamy opcję `Add Python 3.X to PATH`, a następnie wybieramy `Install now`
   
   ![_config.yml]({{ site.baseurl }}/images/2019-03-30-python.gif)


## Instalacja i konfiguracja Visual Studio Code

1. Wchodzimy na stronę programu [(link)](https://code.visualstudio.com/), pobieramy najnowszą wersję
   oraz instalujemy - nie ma tam żadnych interesujących kroków
2. Gdzieś w systemie plików tworzymy sobie pusty katalog, w którym będziemy przechowywali
   pliki z grą.
3. Uruchamiamy program Visual Studio Code, a następnie w prawym górnym rogu klikamy `File -> Open folder`.
   Wybieramy nasz folder
4. Folder na razie jest pusty. Zanim coś do niego dodamy, musimy jeszcze zainstalować dwie dodatkowe
   biblioteki Pythona: [pygame](https://www.pygame.org/wiki/GettingStarted) oraz [ipython](https://ipython.org/).
   Pierwsza z nich to biblioteka niezbędna do napisania gry. Druga jest opcjonalna - będziemy
   mieli dzięki niej nieco lepszą konsolę Pythona. Aby zainstalować dodatkowe bibioteki, naciskamy
   kombinację klawiszy Ctrl + Shift + ` lub wybieramy z menu Terminal -> new terminal. Na dole powinno
   nam się pokazać okienko Windows Powershell. Aby zainstalować biblioteki Pythona, wpisujemy
   w tej konsoli następujące polecenia:

   ```
   py -m pip install -U pygame --user
   py -m pip install -U ipython --user
   ```

   ![_config.yml]({{ site.baseurl }}/images/2019-03-30-pip.gif)

## Sprawdzamy, czy wszystko się powiodło

1. Wchodzimy na stronę samouczka `pygame` [(link)](https://www.pygame.org/docs/tut/PygameIntro.html) i szukamy sekcji `Taste`.
2. Tworzymy nowy, pusty plik o nazwie `gra.py` w katalogu naszego projektu
   i wklejamy do niego zawartosć kodu, który znajduje się w sekcji `Taste`
   samouczka
3. Klikamy prawym przyciskiem myszki na obrazek piłki, który znajduje się
   na stronie samouczka i zapisujemy go do katalogu głównego naszego projektu.
4. Klikamy na plik `gra.py` w Visual Studio Code, naciskamy kombinację klawiszy
   `Ctrl + Shift + P`. W okienku, które się pojawi, wpsiujemy `Python: uruchom plik pythonowy w terminalu` i naciskamy `Enter`. Powinno pojawić się okienko
   z poruszającą się piłką.

## Zadania

Zanim przystąpimy do dalszej części projektu możesz trochę poeksperymentować
z kodem w pliku `gra.py`, żeby poczuć, jak działa biblioteka `pygame`:

1. Spróbuj zmienić rozmiar ekrany na 1280 na 720
2. Spróbuj spowolnić / przyśpieszyć ruch piłki
3. Spróbuj zmienić kolor tła
4. Spróbuj wstawić drugą piłkę (trudniejsze)

To wszystko. Jeśli coś nie zadziało, napisz w komentarzu lub wyślij maila
bezpośrednio do mnie.