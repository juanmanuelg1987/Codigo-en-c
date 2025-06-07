#include <stdio.h>

// ============================================================================
// EJERCICIO 1: Mostrar los números del 1 al 10 usando for
// ============================================================================
// EXPLICACIÓN: Este programa utiliza un bucle for para imprimir números consecutivos
// PSEUDOCÓDIGO:
// PARA i DESDE 1 HASTA 10 HACER
//     IMPRIMIR i
// FIN PARA

void ejercicio1() {
    printf("=== EJERCICIO 1: Números del 1 al 10 ===\n");
    
    // Bucle for: inicialización (i=1), condición (i<=10), incremento (i++)
    for (int i = 1; i <= 10; i++) {
        // Imprime el valor actual de i
        printf("%d ", i);
    }
    printf("\n\n");
}

// ============================================================================
// EJERCICIO 2: Mostrar los números pares del 2 al 20 usando while
// ============================================================================
// EXPLICACIÓN: Utiliza while para mostrar solo números pares incrementando de 2 en 2
// PSEUDOCÓDIGO:
// numero ← 2
// MIENTRAS numero <= 20 HACER
//     IMPRIMIR numero
//     numero ← numero + 2
// FIN MIENTRAS

void ejercicio2() {
    printf("=== EJERCICIO 2: Números pares del 2 al 20 ===\n");
    
    // Inicializa el primer número par
    int numero = 2;
    
    // Bucle while que continúa mientras numero <= 20
    while (numero <= 20) {
        // Imprime el número par actual
        printf("%d ", numero);
        // Incrementa en 2 para obtener el siguiente par
        numero += 2;
    }
    printf("\n\n");
}

// ============================================================================
// EJERCICIO 3: Sumar los primeros 10 números naturales (for)
// ============================================================================
// EXPLICACIÓN: Suma los números del 1 al 10 y muestra el resultado
// PSEUDOCÓDIGO:
// suma ← 0
// PARA i DESDE 1 HASTA 10 HACER
//     suma ← suma + i
// FIN PARA
// IMPRIMIR suma

void ejercicio3() {
    printf("=== EJERCICIO 3: Suma de primeros 10 números naturales ===\n");
    
    // Variable acumuladora inicializada en 0
    int suma = 0;
    
    // Bucle for para sumar números del 1 al 10
    for (int i = 1; i <= 10; i++) {
        // Acumula cada número en la suma total
        suma += i;
        // Muestra el proceso de suma paso a paso
        printf("Sumando %d: total = %d\n", i, suma);
    }
    
    // Muestra el resultado final
    printf("Suma total: %d\n\n", suma);
}

// ============================================================================
// EJERCICIO 4: Pedir números hasta ingresar 0 (usar do while)
// ============================================================================
// EXPLICACIÓN: Solicita números al usuario y los muestra hasta que ingrese 0
// PSEUDOCÓDIGO:
// HACER
//     LEER numero
//     SI numero != 0 ENTONCES
//         IMPRIMIR numero
//     FIN SI
// MIENTRAS numero != 0

void ejercicio4() {
    printf("=== EJERCICIO 4: Pedir números hasta ingresar 0 ===\n");
    
    int numero;
    
    // Bucle do-while: ejecuta al menos una vez, luego verifica condición
    do {
        // Solicita número al usuario
        printf("Ingrese un número (0 para salir): ");
        scanf("%d", &numero);
        
        // Si no es 0, muestra el número ingresado
        if (numero != 0) {
            printf("Número ingresado: %d\n", numero);
        }
    } while (numero != 0); // Continúa mientras no sea 0
    
    printf("¡Programa terminado!\n\n");
}

// ============================================================================
// EJERCICIO 5: Calcular el factorial de un número (for)
// ============================================================================
// EXPLICACIÓN: Calcula el factorial de un número ingresado por el usuario
// PSEUDOCÓDIGO:
// LEER numero
// factorial ← 1
// PARA i DESDE 1 HASTA numero HACER
//     factorial ← factorial * i
// FIN PARA
// IMPRIMIR factorial

void ejercicio5() {
    printf("=== EJERCICIO 5: Calcular factorial de un número ===\n");
    
    int numero;
    // Variable para almacenar el resultado, inicializada en 1
    long long factorial = 1;
    
    // Solicita el número al usuario
    printf("Ingrese un número para calcular su factorial: ");
    scanf("%d", &numero);
    
    // Validación para números negativos
    if (numero < 0) {
        printf("Error: No se puede calcular factorial de números negativos\n\n");
        return;
    }
    
    // Bucle for para calcular factorial
    for (int i = 1; i <= numero; i++) {
        // Multiplica factorial por cada número desde 1 hasta numero
        factorial *= i;
        printf("%d! parcial = %lld\n", i, factorial);
    }
    
    // Muestra el resultado final
    printf("El factorial de %d es: %lld\n\n", numero, factorial);
}

// ============================================================================
// EJERCICIO 6: Contar cuántos números positivos se ingresan (while)
// ============================================================================
// EXPLICACIÓN: Cuenta números positivos hasta que se ingrese un número negativo
// PSEUDOCÓDIGO:
// contador ← 0
// HACER
//     LEER numero
//     SI numero > 0 ENTONCES
//         contador ← contador + 1
//     FIN SI
// MIENTRAS numero >= 0

void ejercicio6() {
    printf("=== EJERCICIO 6: Contar números positivos ===\n");
    
    int numero;
    // Contador de números positivos
    int contador = 0;
    
    printf("Ingrese números (número negativo para terminar):\n");
    
    // Bucle while que continúa mientras el número sea >= 0
    while (1) {
        printf("Número: ");
        scanf("%d", &numero);
        
        // Si es negativo, sale del bucle
        if (numero < 0) {
            break;
        }
        
        // Si es positivo, incrementa contador
        if (numero > 0) {
            contador++;
            printf("Números positivos ingresados hasta ahora: %d\n", contador);
        }
        // Si es 0, no cuenta pero continúa
    }
    
    // Muestra el resultado final
    printf("Total de números positivos ingresados: %d\n\n", contador);
}

// ============================================================================
// EJERCICIO 7: Mostrar tabla de multiplicar (usar for)
// ============================================================================
// EXPLICACIÓN: Muestra la tabla de multiplicar de un número ingresado
// PSEUDOCÓDIGO:
// LEER numero
// PARA i DESDE 1 HASTA 10 HACER
//     resultado ← numero * i
//     IMPRIMIR numero + " x " + i + " = " + resultado
// FIN PARA

void ejercicio7() {
    printf("=== EJERCICIO 7: Tabla de multiplicar ===\n");
    
    int numero;
    
    // Solicita el número para la tabla
    printf("Ingrese un número para ver su tabla de multiplicar: ");
    scanf("%d", &numero);
    
    printf("\nTabla de multiplicar del %d:\n", numero);
    printf("------------------------\n");
    
    // Bucle for para generar tabla del 1 al 10
    for (int i = 1; i <= 10; i++) {
        // Calcula el resultado de la multiplicación
        int resultado = numero * i;
        // Muestra la operación completa
        printf("%d x %d = %d\n", numero, i, resultado);
    }
    printf("\n");
}

// ============================================================================
// EJERCICIO 8: Sumar una serie de números hasta ingresar negativo (do while)
// ============================================================================
// EXPLICACIÓN: Suma números hasta que se ingrese un número negativo
// PSEUDOCÓDIGO:
// suma ← 0
// HACER
//     LEER numero
//     SI numero >= 0 ENTONCES
//         suma ← suma + numero
//     FIN SI
// MIENTRAS numero >= 0

void ejercicio8() {
    printf("=== EJERCICIO 8: Sumar números hasta ingresar negativo ===\n");
    
    int numero;
    // Acumulador para la suma
    int suma = 0;
    
    printf("Ingrese números para sumar (número negativo para terminar):\n");
    
    // Bucle do-while: ejecuta al menos una vez
    do {
        printf("Número: ");
        scanf("%d", &numero);
        
        // Si el número es positivo o cero, lo suma
        if (numero >= 0) {
            suma += numero;
            printf("Suma parcial: %d\n", suma);
        }
    } while (numero >= 0); // Continúa mientras no sea negativo
    
    // Muestra el resultado final
    printf("Suma total: %d\n\n", suma);
}

// ============================================================================
// EJERCICIO 9: Mostrar números del 10 al 1 (for descendente)
// ============================================================================
// EXPLICACIÓN: Utiliza for con decremento para mostrar números en orden descendente
// PSEUDOCÓDIGO:
// PARA i DESDE 10 HASTA 1 DECREMENTANDO HACER
//     IMPRIMIR i
// FIN PARA

void ejercicio9() {
    printf("=== EJERCICIO 9: Números del 10 al 1 (descendente) ===\n");
    
    // Bucle for descendente: inicia en 10, continúa mientras i>=1, decrementa
    for (int i = 10; i >= 1; i--) {
        // Imprime el valor actual
        printf("%d ", i);
    }
    printf("\n\n");
}

// ============================================================================
// EJERCICIO 10: Verificar si un número es primo (while)
// ============================================================================
// EXPLICACIÓN: Verifica si un número es primo probando divisores hasta su raíz cuadrada
// PSEUDOCÓDIGO:
// LEER numero
// SI numero <= 1 ENTONCES
//     NO ES PRIMO
// SINO
//     divisor ← 2
//     esPrimo ← VERDADERO
//     MIENTRAS divisor * divisor <= numero Y esPrimo HACER
//         SI numero MOD divisor = 0 ENTONCES
//             esPrimo ← FALSO
//         FIN SI
//         divisor ← divisor + 1
//     FIN MIENTRAS
// FIN SI

void ejercicio10() {
    printf("=== EJERCICIO 10: Verificar si un número es primo ===\n");
    
    int numero;
    // Variable bandera para determinar si es primo
    int esPrimo = 1; // 1 = verdadero, 0 = falso
    
    // Solicita el número al usuario
    printf("Ingrese un número para verificar si es primo: ");
    scanf("%d", &numero);
    
    // Casos especiales: números <= 1 no son primos
    if (numero <= 1) {
        esPrimo = 0;
    } else if (numero == 2) {
        // 2 es el único número par primo
        esPrimo = 1;
    } else {
        // Verifica divisores desde 2 hasta la raíz cuadrada del número
        int divisor = 2;
        
        // Bucle while para buscar divisores
        while (divisor * divisor <= numero && esPrimo) {
            // Si encuentra un divisor, no es primo
            if (numero % divisor == 0) {
                esPrimo = 0;
                printf("Divisor encontrado: %d\n", divisor);
            }
            // Incrementa el divisor para probar el siguiente
            divisor++;
        }
    }
    
    // Muestra el resultado
    if (esPrimo) {
        printf("El número %d ES PRIMO\n\n", numero);
    } else {
        printf("El número %d NO ES PRIMO\n\n", numero);
    }
}

// ============================================================================
// FUNCIÓN PRINCIPAL - MENÚ DE EJERCICIOS
// ============================================================================
// EXPLICACIÓN: Presenta un menú para que el usuario elija qué ejercicio ejecutar
// PSEUDOCÓDIGO:
// REPETIR
//     MOSTRAR MENÚ
//     LEER opcion
//     SEGÚN opcion HACER
//         CASO 1: ejercicio1()
//         CASO 2: ejercicio2()
//         ...
//         CASO 0: SALIR
//     FIN SEGÚN
// HASTA QUE opcion = 0

int main() {
    int opcion;
    
    do {
        // Muestra el menú de opciones
        printf("\n========================================\n");
        printf("         MENÚ DE EJERCICIOS CON BUCLES\n");
        printf("========================================\n");
        printf("1.  Números del 1 al 10 (for)\n");
        printf("2.  Números pares del 2 al 20 (while)\n");
        printf("3.  Suma primeros 10 números (for)\n");
        printf("4.  Pedir números hasta 0 (do-while)\n");
        printf("5.  Calcular factorial (for)\n");
        printf("6.  Contar positivos (while)\n");
        printf("7.  Tabla de multiplicar (for)\n");
        printf("8.  Sumar hasta negativo (do-while)\n");
        printf("9.  Números 10 al 1 descendente (for)\n");
        printf("10. Verificar número primo (while)\n");
        printf("0.  SALIR\n");
        printf("========================================\n");
        printf("Seleccione una opción: ");
        
        // Lee la opción del usuario
        scanf("%d", &opcion);
        
        // Switch para ejecutar el ejercicio seleccionado
        switch (opcion) {
            case 1:
                ejercicio1();
                break;
            case 2:
                ejercicio2();
                break;
            case 3:
                ejercicio3();
                break;
            case 4:
                ejercicio4();
                break;
            case 5:
                ejercicio5();
                break;
            case 6:
                ejercicio6();
                break;
            case 7:
                ejercicio7();
                break;
            case 8:
                ejercicio8();
                break;
            case 9:
                ejercicio9();
                break;
            case 10:
                ejercicio10();
                break;
            case 0:
                printf("¡Gracias por usar el programa!\n");
                break;
            default:
                printf("Opción inválida. Intente nuevamente.\n");
        }
        
        // Pausa para que el usuario pueda ver los resultados
        if (opcion != 0) {
            printf("Presione Enter para continuar...");
            getchar(); // Consume el \n del scanf anterior
            getchar(); // Espera que el usuario presione Enter
        }
        
    } while (opcion != 0); // Continúa hasta que el usuario elija salir
    
    return 0;
}
