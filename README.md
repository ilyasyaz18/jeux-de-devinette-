# jeux-de-devinette-ceci est mon 1er projet en c 

#include <stdio.h>

int main() {

    int n=50,nbre,trouver=0;
    int i=5;
    
do{

    printf("\n entrer un nbre ou bien deviner un nbre ");
    scanf("%d",&nbre);
    
    if(nbre>n){
        printf("\n le nbre est plus petit que %d",nbre);
        i--;
        printf("\n il vous reste %d chances",i);
    }
    else if(nbre<n){
        printf("\n le nbre est plus grand que %d",nbre);
        i--;
        printf("\n il vous reste %d chances",i);
    }
    else{
        printf("\n bravooooooo vous avez trouver le nbre a deviner est %d ",n);
        trouver=1;
        break;
    }
}while(i!=0);

if(!trouver){

    printf("\n c'est pas grave de ne pas trouver le nbre la prochaine fois");
}



    return 0;
}
