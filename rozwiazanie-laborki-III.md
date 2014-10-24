## Rozwiązania zadań

1\.Wyświetl plik /etc/passwd z podziałem na strony przyjmując, że strona na 5 linii tekstu.

```sh
cd /etc/
more -5 passwd
```

2\.Korzystając z polecenia cat utwórz plik tekst3.txt, który będzie składał się z zawartości pliku tekst1.txt, ciągu znaków podanego ze standardowego wejścia (klawiatury) i pliku tekst2.txt.

```sh
cat tekst1.txt - tekst2.txt > tekst3.txt
```

3\.Wyświetl po 5 pierwszych linii wszystkich plików w swoim katalogu domowym w taki sposób, aby nie były wyświetlane ich nazwy.

```sh
head -q -n5 tekst1.txt tekst2.txt tekst3.txt 
```

4\.Wyświetl linie o numerach 3, 4 i 5 z pliku /etc/passwd.

```sh
cat passwd | head -n 5 | tail -n 3
```

5\.Wyświetl linie o numerach 7, 6 i 5 od końca pliku /etc/passwd.

```sh
cat passwd |tail -n 7 |head -n 3
```

6\.Wyświetl zawartość pliku /etc/passwd w jednej linii.

```sh
cat passwd |tr '/n' ' '
```

7\.Za pomocą filtru tr wykonaj modyfikację pliku plik.txt, polegającą na wypisaniu każdego słowa w osobnej linii.

```sh
cat plik.txt | tr ' ' '/n'
```

8\.Zlicz wszystkie pliki znajdujące się w katalogu /var i jego podkatalogach.

```sh
find /var/ -type f |wc -l
```

9\.Napisać polecenie zliczające ilość znaków z pierwszych trzech linii pliku /etc/passwd.

```sh
head -n 1 passwd | wc -m
```








