# LFA
Exercicios de Linguagens Formais e Autômatos

#include <stdio.h>
#include <stdlib.h>
int main (void)
{
  float coin, total=0, troco=0;
 
  printf("************  Máquina de Refrigerante  ************\n\n");
  printf("*** Só aceitamos moedas de 10 ou 25 centavos *** \n");
  printf("\t*** OBS: NÃO DEVOLVEMOS TROCO !!! *** \n\n");
 
  do{
  printf("Insira um valor: ");
  scanf("%f/0.01", &coin);
 
   if((coin != 10) && (coin != 25)){
   printf("*** Só aceitamos moedas de 10 ou 25 centavos *** \n");
   }else{
     total += coin;
        printf("Total: R$ 0,%0.f\n",total);
   if(total > 45){
        troco = total - 45;
        printf("*** Refrigerante Liberado *** \n");
        printf("Troco R$ 0,%0.f\n",troco);
        printf("*** Não devolvemos troco ***\n");
        printf("\n*** OBRIGADO PELA PREFERÊNCIA ***\n");
        system ("pause");
    return(0);
      }
    }
  }while(total != 45);
      printf("*** Refrigerante Liberado *** \n");
      printf("Troco R$ 0,%0.f\n", troco);
      system ("pause");
      return(0);
}
