#include <stdio.h>

int main() {
    int V;

    while (1) {
        printf("Por favor, ingresa un numero entre 1000 y 9999: ");
        scanf("%d", &V);
        if (V >= 1000 && V <= 9999) {
            
            int miles = (V / 1000);
            int centenas = (V / 100) % 10;
            int decenas = (V / 10) % 10;
            int unidades = (V % 10);
            
            printf("Miles: %d\n", miles);
            printf("Centenas: %d\n", centenas);
            printf("Decenas: %d\n", decenas);
            printf("Unidades: %d\n", unidades);
            break;
        } else {
            printf("Numero ingresado no valido, intente de nuevo\n");
        }
    }

    return 0;
}
