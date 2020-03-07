#include <stdio.h>
#include <stdlib.h>

struct aluno
{
    char nome[10];
    float nota[3], media;   
};

//sintaxe de atribuição de um valor a uma variavel de um struct é %otipo%*c (que é por referencia, que muda diretamente ele no endereço de memória)
//quando declaro um array com data[5] quer dizer que eu quero ocupar 5 posições onde a 1 posição é o index 0
int main(){ 

    struct aluno alunos[5];

    int i,cont;

    for(i = 0; i < 5; i++){
        system("cls");
        printf("digite o nome do aluno:\n");
        scanf("%s%*c", &alunos[i].nome);

        for(cont = 0; cont  < 3; cont++){
            printf("digite a %i nota:\n", cont+1);
            scanf("%f%*c", &alunos[i].nota[cont]);
            alunos[i].media += alunos[i].nota[cont];
        }

        alunos[i].media /= cont;
    }

        system("cls");

    for(i = 0; i < 5; i++){
        printf("------------------------------------------------\n");
        printf("Aluno: %s\n", alunos[i].nome);

        for(cont = 0; cont  < 3; cont++){
            printf("%i nota: %.1f\n", cont+1,alunos[i].nota[cont]);
        }

        printf("------------------------------------------------\n");
        printf("Media: %.1f\n", alunos[i].media);
    }

    system("pause");
    return 0;
}
