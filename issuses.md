Formatowanie kodu
No milestone
No one is assigned

Aby uzyskać ładne wcęcia w kodzie korzystamy z programu indent.

Wchodzimy na terminal i logujemy się na sigmie:

ssh akiszel@sigma.ug.edu.pl

Następnie wykonujemy kopiuj kod i wklej go na terminalu.
Przykładowo:

cat > zad5.c
... ctrl+shift+v lub wybieramy wklej z menu terminala
CTRL+d

Teraz wykonujemy na terminalu:

indent -kr zad5.c

