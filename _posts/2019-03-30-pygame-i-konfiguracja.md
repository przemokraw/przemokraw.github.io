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

