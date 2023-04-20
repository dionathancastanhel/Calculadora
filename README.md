#include <stdio.h>

int main(void) {
  int quantos, cal;
  float soma = 0, multiplicacao = 1, numero, n1, n2;
  printf("Qual cálculo você deseja fazer?\n1-Soma\n2-Subtração\n3-Multiplicação\n4-Divisão\n");
  scanf("%d", &cal);
  if (cal == 1) {
    printf("Quantos números serão somados no final?\n");
    scanf("%d", &quantos);
    for (int i = 1; i <= quantos; i++) {
      printf("Informe o %dº número: ", i);
      scanf("%f", &numero);
      soma += numero;   
    }
    printf("A soma dos números é: %.2f\n", soma);
  } else if  (cal == 2) {
    printf("Informe o maior número: ");
      scanf("%f", &n1);
        printf("Informe o menor número: ");
      scanf("%f", &n2);
    printf("A subtração dos números é: %.2f", n1 - n2);
  } else if (cal == 3) {
    printf("Quantos números serão multiplicados no final?\n");
      scanf("%d", &quantos);
    for (int i = 1; i <= quantos; i++) {
       printf("Informe o %dº número: ", i);
      scanf("%f", &numero);
      multiplicacao *= numero;
    }
     printf("A multiplicação dos números é: %.2f\n", multiplicacao);
  } else if  (cal == 4) {
    printf("Informe o dividendo: ");
      scanf("%f", &n1);
        printf("Informe o divisor: ");
scanf("%f", &n2);
    printf("A divisão dos números é: %.2f", n1 / n2);
  } else {
    printf("Você não inseriu um número válido! Repita o processo!");
  }
  return 0;
}
