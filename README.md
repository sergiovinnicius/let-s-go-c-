# let-s-go-c-
This program in c ++ sums all values obtained in two 2x2 matrices and shows the result on the screen.

#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <locale.h>

int main() {
	int matriz1[2][2];
	int matriz2[2][2];
	int i, j;
	int resultado;
	
	setlocale(LC_ALL, "Portuguese");
	
	for(i = 0; i < 2; i++) {
		for (j = 0; j < 2; j++){
		printf("\nDigite os valores da matriz 1[%d][%d]: ", i,j);
		scanf("%d", &matriz1[i][j]);
		}
	}
	
	for(i = 0; i < 2; i++) {
	    for (j = 0; j < 2; j++){
     	printf("\nDigite os valores da matriz 2[%d][%d]: ", i,j);
    	scanf("%d", &matriz2[i][j]);
		}
	}
	
    for(i = 0; i < 2; i++) {
	    for (j = 0; j < 2; j++) {
			resultado = matriz1[0][0] + matriz1[0][1] + matriz1[1][0] + matriz1[1][1] + matriz2[0][0] + matriz2[0][1] + matriz2[1][0] + matriz2[1][1];
		}
	}
	
	 for(i = 0; i < 2; i++) {
	    for (j = 0; j < 2; j++) {
		   printf("\nO RESULTADO DA SOMA ENTRE OS VALORES DAS DUAS MATRIZES É : %d\n\n\n", resultado);
	       break;
		}
	    break; 
	}
	
	
	system("pause");
	return 0;
}
