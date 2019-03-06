# Exercicio24

Exercício 24
#include <stdio.h>
#include <string.h>

int main ()
{
    system("color 0b");
    char frase [50];
    char * ponteiro ;

    printf("Digite uma frase: ");
    gets(frase);

    printf (" Pesquisando o caractere 'l' na frase\n %s\n", frase ) ;
    ponteiro = strchr ( frase , 'l' );

    while ( ponteiro != NULL )
    {
    printf (" encontrada em% d \n", ponteiro - frase + 1 ) ;
    ponteiro = strchr ( ponteiro + 1 , 'l' );
    }

    return 0; 
}
