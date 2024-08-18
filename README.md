// Questão 1

#include <stdio.h>

// Função que soma os elementos de um array
int soma_array(int array[], int tamanho);
int main() {
    int n;
// Solicita o tamanho do array 
    printf("Digite o tamanho do array: ");
    scanf("%d", &n);
    
    int array[n];
// Solicita os elementos do array
    printf("Digite %d números inteiros:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }
// Calcula a soma dos elementos do array
    int resultado = soma_array(array, n);
// Exibe o resultado da soma
    printf("A soma dos elementos do array é: %d\n", resultado);
    
    return 0;
}




int soma_array(int array[], int tamanho) {
    int soma = 0;
    for (int i = 0; i < tamanho; i++) {
        soma += array[i];
    }
    return soma;
}
