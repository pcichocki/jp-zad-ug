## Bash -- zadania

1\. Używając linii poleceń stwórz strukturę katalogów:

```sh
mkdir temp/{dom,nauka/{c,logo,pascal},praca/{dokumenty,zlecenia/{zrealizowane,niezrealizowane}}} -p
```

2\.Przejdź do katalogu dom i utwórz katalog wazne-sprawy.

```sh
cd dom
mkdir wazne-sprawy
```

3\Wejdź do katalogu wazne-sprawy i utwórz tam pusty plik rachunki.txt.

```sh
cd wazne-sprawy
touch rachunki.txt
```

4\.Będąc w katalogu wazne-sprawy skopiuj plik rachunki.txt do katalogu zrealizowane.

```sh
cp rachunki.txt ~/temp/praca/zlecenia/zrealizowane/
```

5\.Przejdź do katalogu zrealizowane i zmień nazwę pliku rachunki.txt na wykonano.txt.

```sh
cd ~/temp/praca/zlecenia/zrealizowane/
mv rachunki.txt wykonano.txt
```
