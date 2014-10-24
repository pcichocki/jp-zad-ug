##Rozwiązania zadań

_Przyznam się, że niektórych zadań nie potrafiłem na chwilę obecną sam ogarnąć, ale szukając pomocy w internecie przetestowałem działanie każdej nowo poznawanej opcji. ;)_

1\.Wyświetl listę plików z aktualnego katalogu, zamieniając wszystkie małe litery na duże.

```sh
ls -l |tr [:lower:] [:upper:]
```

2\.Wyświetl listę praw dostępu do plików w aktualnym katalogu, ich rozmiar i nazwę.

```sh
ls -l | cut -b 1-11,33-36,51-
```

3\.Wyświetl listę plików w aktualnym katalogu, posortowaną według rozmiaru pliku.

```sh
ls -Sl
```

4\.Wyświetl zawartość pliku /etc/passwd posortowaną według numerów UID w kolejności od największego do najmniejszego.

```sh
cat passwd | sort --reverse --general-numeric-sort --key3
```

5\.Wyświetl zawartość pliku /etc/passwd posortowaną najpierw według numerów GID w kolejności od największego do najmniejszego, a następnie UID.

```sh
cat /etc/passwd/ | sort --general-numeric-sort --key 4,3 --reverse
```

6\.Podaj liczbę plików każdego użytkownika.

```sh
find /home/ -type f | wc -l
```

_Oczywiście pracując będąc zalogowanym na Sigmie brak uprawnień do wykonania polecenia._

7\.Sporządź statystykę praw dostępu (dla każdego z praw dostępu podaj ile razy zostało ono przydzielone).

```sh
find -printf "%M\n" | sort | uniq -c
```

8\.Czy potrafisz odpowiedzieć jaki będzie efekt wykonania poniższych poleceń?

1#
