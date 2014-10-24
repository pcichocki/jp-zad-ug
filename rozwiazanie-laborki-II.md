## Rozwiązania zadań.

W katalogu c utwórz plik program.c zawierający co najmniej 10 linii kodu napisanego w języku C. (Sam kod należy wyszukać i pobrać z sieci.)

_Użyłem tego kodu: [press me button game](http://www.programmingsimplified.com/c-press-me-button-game)_

1\. Wyświetl na ekran 2 pierwsze wiersze pliku program.c. (head)

```sh
head -n 2 program.c
```

2\.Wyświetl na ekran 4 ostatnie wiersze pliku program.c.

```sh
tail -n 4 program.c
```

3\.W pliku program.c znajdź wszystkie wiersze z wystąpieniem słowa „main”.

```sh
grep main program.c
```

4\.Plikowi program.c nadaj następujące uprawnienia: właściciel – czytanie, pisanie, grupa – czytanie, pozostali użytkownicy: brak uprawnień.

```sh
chmod u=wr,g=r program.c
```
5\.Będąc w katalogu temp przenieś katalog wazne-sprawy do katalogu praca.

```sh
mv dom/wazne-sprawy/ praca/
```

6\.Zarchiwizuj cały katalog temp.

```sh
tar -czf temp.tar temp/
```

7\. Usuń katalog temp.

```sh
rmdir --ignore-fail-on-non-empty temp/
```

8\. Odtwórz z archiwum katalog temp.

```sh
tar -xv temp.tar
```

9\. Posprzątaj na swoim koncie.

```sh
rm temp.tar
rmdir --ignore-fail-on-non-empty temp/
```



