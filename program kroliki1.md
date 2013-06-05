<b>PROGRAM LICZACY KROLIKI NA WYSPIE<b/><br><br>
```c
#include <stdio.h>
#include <math.h>


#define r 4
#define MAX 5000.0

/*
const double r = 3.7;
const double MAX = 5000.0;*/

int main(){
  double k;
	
	int l;
	
	printf("podaj poczatkowa ilosc krolikow ");
	scanf("%d", &l);
	if(l==1){
		printf("jeden krolik nie da potomstwa");
		return 0;
	}
	if(l==0){
		printf("zero krolikow nie da potomstwa");
		return 0;
	}	
	if(l<0){
		printf("liczba krolikow nie moze byc ujemna");
		return 0;
	}
	if(l>(int)MAX){
		printf("liczba krolikow przekracza maksimum");
		return 0;
	}
	
	k = ((double)l)/MAX;

	int i;
	for(i=0; i<21; ++i){ //powtarzamy zaczynajac od i=0, zwiekszajac o 1 az dojdziemy do 21. Przy 21 petla sie juz nie powtorzy.
		printf("liczba krolikow po %d lat: %.0lf\n", i, round(k*MAX));
		k=k*(1.0-k)*r;
	
	}


	return 0;
}
```
