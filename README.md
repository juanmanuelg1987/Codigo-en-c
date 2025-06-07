# Codigo-en-c

#include <stdio.h>

int main() {
    int suma = 0;
    
    // Bucle for para sumar los primeros 10 números naturales
    for (int i = 1; i <= 10; i++) {
        suma += i;
    }
    
    printf("La suma de los primeros 10 números naturales es: %d\n", suma);
    
    return 0;
}



//código en C para sumar los primeros 10 números naturales usando un bucle `for`:
//El programa funciona de la siguiente manera:

//1. Declaramos una variable `suma` inicializada en 0 para almacenar el resultado
//2. El bucle `for` itera desde 1 hasta 10 (inclusive)
//3. En cada iteración, sumamos el valor actual de `i` a la variable `suma`
//4. Al finalizar el bucle, mostramos el resultado

//El resultado será **55**, que es la suma de 1+2+3+4+5+6+7+8+9+10.

//Si quisieras hacer el código más flexible para sumar cualquier cantidad de números naturales, 
//podrías modificar el 10 por una variable o pedirle al usuario que ingrese el número límite.


//# Mostrar números del 1 al 10 usando WHILE

//## Código en C

//#include <stdio.h>

//int main() {
  //  int i = 1;
    
    //printf("Números del 1 al 10:\n");
    
    //while (i <= 10) {
   //     printf("%d ", i);
   //     i++;
   // }
    
   // printf("\n");
   // return 0;
//}


//## Pseudocódigo

//INICIO
 //   i ← 1
  //  ESCRIBIR "Números del 1 al 10:"
    
 //   MIENTRAS i ≤ 10 HACER
 //       ESCRIBIR i
 //       i ← i + 1
//    FIN MIENTRAS
//FIN


//## Explicación detallada

//### ¿Qué es el bucle WHILE?

//El bucle `while` es una estructura de repetición que ejecuta un bloque de código **mientras** una condición sea verdadera. Se evalúa la condición **antes** de cada ejecución.

//### Estructura del bucle WHILE:


//while (condición) {
    // código a repetir
    // actualización de variable de control
//}
//```

//### Análisis paso a paso:

//#### 1. **Inicialización**
//```c
//int i = 1;
//```
//- Declaramos la variable `i` y la inicializamos en 1
//- Esta será nuestra variable de control del bucle

//#### 2. **Condición del bucle**
//```c
//while (i <= 10)
//```
//- **Se evalúa ANTES de cada iteración**
//- Si `i` es menor o igual a 10, ejecuta el bloque
//- Si `i` es mayor a 10, termina el bucle

//#### 3. **Cuerpo del bucle**
//```c
//printf("%d ", i);
//i++;
//```
//- **Impresión**: Muestra el valor actual de `i`
//- **Incremento**: Aumenta `i` en 1 (`i++` es equivalente a `i = i + 1`)

//### Flujo de ejecución:

//| Iteración | Valor de i | ¿i <= 10? | Acción | Nuevo valor de i |
//|-----------|------------|-----------|--------|------------------|
//| 1         | 1          | Sí        | Imprime 1 | 2 |
//| 2         | 2          | Sí        | Imprime 2 | 3 |
//| 3         | 3          | Sí        | Imprime 3 | 4 |
//| ...       | ...        | ...       | ... | ... |
//| 10        | 10         | Sí        | Imprime 10 | 11 |
//| 11        | 11         | No        | Sale del bucle | - |

//### Características importantes del WHILE:

//#### Ventajas:
//- **Flexibilidad**: Ideal cuando no sabes exactamente cuántas iteraciones necesitas
//- **Control preciso**: La condición se evalúa antes de cada ejecución
//- **Legibilidad**: Es fácil de entender y leer

//#### Cuidados importantes:
//- **Variable de control**: Siempre inicializar la variable antes del bucle
//- **Actualización**: No olvidar incrementar/actualizar la variable dentro del bucle
//- **Bucle infinito**: Si no actualizas la variable, el bucle nunca termina

//### Ejemplo de error común:
//```c
// ¡CUIDADO! Bucle infinito
//int i = 1;
//while (i <= 10) {
//    printf("%d ", i);
    // ¡Olvidé incrementar i!
//}
//```

//### Cuándo usar WHILE:
//- Cuando la cantidad de iteraciones depende de una condición
//- Para validar entrada de usuario
//- Para leer archivos hasta el final
//- Para procesar datos hasta encontrar un valor específico

//**Salida del programa**: `1 2 3 4 5 6 7 8 9 10`







#include <stdio.h>

int main() 
{

    
    int contador=2;
    while (contador <= 20)
    {
        printf ("%d\n", contador);
        contador+= 2 ;
    }
    


    return 0;
}
Excelente código! Me parece una implementación muy limpia y eficiente. Analicemos sus fortalezas:
Puntos fuertes de tu código:
✅ Eficiencia óptima

Usa el Método 1 que mostré anteriormente (incrementar de 2 en 2)
Solo 10 iteraciones en lugar de 20
No hace verificaciones innecesarias con el operador módulo

✅ Código limpio y legible

Variable con nombre descriptivo: contador
Lógica clara y directa
Bien estructurado con llaves

✅ Implementación correcta

Inicializa correctamente en 2
Condición adecuada (<= 20)
Incremento correcto (+= 2)



# Mostrar números pares del 2 al 20 usando WHILE

## Código en C

### Método 1: Incrementar de 2 en 2
```c
#include <stdio.h>

int main() {
    int i = 2;
    
    printf("Números pares del 2 al 20 (método 1):\n");
    
    while (i <= 20) {
        printf("%d ", i);
        i += 2;  // Incrementa de 2 en 2
    }
    
    printf("\n");
    return 0;
}
```

### Método 2: Verificar si es par usando módulo
```c
#include <stdio.h>

int main() {
    int i = 2;
    
    printf("Números pares del 2 al 20 (método 2):\n");
    
    while (i <= 20) {
        if (i % 2 == 0) {  // Verifica si es par
            printf("%d ", i);
        }
        i++;  // Incrementa de 1 en 1
    }
    
    printf("\n");
    return 0;
}
```

### Método 3: Empezar desde 1 y verificar paridad
```c
#include <stdio.h>

int main() {
    int i = 1;
    
    printf("Números pares del 2 al 20 (método 3):\n");
    
    while (i <= 20) {
        if (i % 2 == 0) {  // Si es par, lo imprime
            printf("%d ", i);
        }
        i++;
    }
    
    printf("\n");
    return 0;
}
```

## Pseudocódigo

### Método 1: Incrementar de 2 en 2
```
INICIO
    i ← 2
    ESCRIBIR "Números pares del 2 al 20:"
    
    MIENTRAS i ≤ 20 HACER
        ESCRIBIR i
        i ← i + 2
    FIN MIENTRAS
FIN
```

### Método 2: Verificar paridad desde 2
```
INICIO
    i ← 2
    ESCRIBIR "Números pares del 2 al 20:"
    
    MIENTRAS i ≤ 20 HACER
        SI i MOD 2 = 0 ENTONCES
            ESCRIBIR i
        FIN SI
        i ← i + 1
    FIN MIENTRAS
FIN
```

### Método 3: Verificar paridad desde 1
```
INICIO
    i ← 1
    ESCRIBIR "Números pares del 2 al 20:"
    
    MIENTRAS i ≤ 20 HACER
        SI i MOD 2 = 0 ENTONCES
            ESCRIBIR i
        FIN SI
        i ← i + 1
    FIN MIENTRAS
FIN
```

## Explicación detallada

### ¿Qué son los números pares?

Los números pares son aquellos que son divisibles por 2, es decir, al dividirlos entre 2 el **resto es cero**.

**Números pares del 2 al 20**: 2, 4, 6, 8, 10, 12, 14, 16, 18, 20

### Conceptos clave:

#### 1. **Operador módulo (%)**
- Devuelve el **resto** de una división
- `8 % 2 = 0` (8 dividido 2 da resto 0)
- `9 % 2 = 1` (9 dividido 2 da resto 1)
- **Si `número % 2 == 0`**, entonces el número es par

#### 2. **Operador de asignación compuesta (+=)**
- `i += 2` es equivalente a `i = i + 2`
- Permite incrementar de manera más eficiente

### Análisis de cada método:

#### **Método 1: Incrementar de 2 en 2 (MÁS EFICIENTE)**

**Ventajas:**
- Más eficiente: solo visita números pares
- Menos iteraciones (10 vs 19)
- Código más simple y directo

**Flujo de ejecución:**
| Iteración | Valor de i | ¿i <= 20? | Acción | Nuevo valor de i |
|-----------|------------|-----------|--------|------------------|
| 1         | 2          | Sí        | Imprime 2 | 4 |
| 2         | 4          | Sí        | Imprime 4 | 6 |
| 3         | 6          | Sí        | Imprime 6 | 8 |
| ...       | ...        | ...       | ... | ... |
| 10        | 20         | Sí        | Imprime 20 | 22 |
| 11        | 22         | No        | Sale del bucle | - |

#### **Método 2: Verificar paridad desde 2**

**Ventajas:**
- Muestra claramente el concepto de número par
- Útil para enseñar el operador módulo
- Fácil de modificar para otros criterios

**Desventajas:**
- Menos eficiente: verifica todos los números del 2 al 20
- Más iteraciones innecesarias

#### **Método 3: Verificar paridad desde 1**

**Ventajas:**
- Concepto más general (puede adaptarse fácilmente a cualquier rango)
- Muestra el filtrado completo de números

**Desventajas:**
- Menos eficiente: revisa números impares innecesarios
- Una iteración extra (verifica el 1)

### Comparación de eficiencia:

| Método | Iteraciones totales | Números impresos | Verificaciones |
|--------|-------------------|------------------|----------------|
| Método 1 | 10 | 10 | 10 |
| Método 2 | 19 | 10 | 19 |
| Método 3 | 20 | 10 | 20 |

### ¿Cuándo usar cada método?

- **Método 1**: Cuando la eficiencia es importante y el patrón es claro
- **Método 2**: Para enseñar conceptos de paridad y filtrado
- **Método 3**: Cuando necesitas un enfoque más general y flexible

### Conceptos de programación aplicados:

1. **Estructuras de control**: Bucle while
2. **Operadores aritméticos**: %, +=, ++
3. **Estructuras condicionales**: if
4. **Optimización**: Elegir el método más eficiente
5. **Legibilidad vs eficiencia**: Balance entre código claro y rendimiento

**Salida de todos los métodos**: `2 4 6 8 10 12 14 16 18 20`





#include <stdio.h>

int main() {
    int suma = 0;
    
    // Bucle for para sumar los primeros 10 números naturales
    for (int i = 1; i <= 10; i++) {
        suma += i;
    }
    
    printf("La suma de los primeros 10 números naturales es: %d\n", suma);
    
    return 0;
}

//código en C para sumar los primeros 10 números naturales usando un bucle `for`:
//El programa funciona de la siguiente manera:

//1. Declaramos una variable `suma` inicializada en 0 para almacenar el resultado
//2. El bucle `for` itera desde 1 hasta 10 (inclusive)
//3. En cada iteración, sumamos el valor actual de `i` a la variable `suma`
//4. Al finalizar el bucle, mostramos el resultado

//El resultado será **55**, que es la suma de 1+2+3+4+5+6+7+8+9+10.

//Si quisieras hacer el código más flexible para sumar cualquier cantidad de números naturales, 
//podrías modificar el 10 por una variable o pedirle al usuario que ingrese el número límite.

//pseudocodigo iNICIO
 //   suma ← 0
    
 //   PARA i DESDE 1 HASTA 10 HACER
 //       suma ← suma + i
 //   FIN PARA
    
 //   ESCRIBIR "La suma de los primeros 10 números naturales es:", suma
//FIN







//# Pedir números hasta ingresar 0

#include <stdio.h>

int main() {
    int numero;
    int suma = 0;
    int contador = 0;
    
    printf("Ingrese números (0 para terminar):\n");
    
    do {
        printf("Número: ");
        scanf("%d", &numero);
        
        if (numero != 0) {
            suma += numero;
            contador++;
        }
    } while (numero != 0);
    
    printf("\nResultados:\n");
    printf("Cantidad de números ingresados: %d\n", contador);
    printf("Suma total: %d\n", suma);
    
    if (contador > 0) {
        printf("Promedio: %.2f\n", (float)suma / contador);
    }
    
    return 0;
}

//## Pseudocódigo


//INICIO
 //   numero ← 0
 //   suma ← 0
 //   contador ← 0
    
 //   ESCRIBIR "Ingrese números (0 para terminar):"
    
 //   REPETIR
 //       ESCRIBIR "Número: "
 //       LEER numero
        
 //       SI numero ≠ 0 ENTONCES
 //           suma ← suma + numero
 //           contador ← contador + 1
 //       FIN SI
 //   MIENTRAS numero ≠ 0
    
 //   ESCRIBIR "Resultados:"
 //   ESCRIBIR "Cantidad de números ingresados:", contador
 //   ESCRIBIR "Suma total:", suma
    
 //   SI contador > 0 ENTONCES
 //       promedio ← suma / contador
 //       ESCRIBIR "Promedio:", promedio
 //   FIN SI
//FIN


//## Explicación del algoritmo

//### Conceptos clave:

//1. **Bucle do-while / REPETIR-MIENTRAS**: Se ejecuta al menos una vez y continúa mientras la condición sea verdadera.

//2. **Variable centinela**: El valor 0 actúa como señal para terminar el bucle.

//3. **Variables acumuladoras**:
//   - `suma`: Acumula la suma de todos los números ingresados
//   - `contador`: Cuenta cuántos números válidos se ingresaron

//### Flujo de ejecución:

//1. **Inicialización**: Se declaran e inicializan las variables necesarias
//2. **Entrada del bucle**: Se pide el primer número al usuario
//3. **Validación**: Si el número no es 0, se suma al total y se incrementa el contador
//4. **Condición de continuidad**: El bucle continúa mientras el número ingresado no sea 0
//5. **Resultados**: Al salir del bucle, se muestran las estadísticas calculadas

//### Ventajas de usar do-while:

//- Garantiza que se ejecute al menos una iteración
//- La condición se evalúa después de cada ejecución
//- Ideal para menús y validaciones de entrada

//### Posibles mejoras:

//- Validación de entrada para números no válidos
//- Manejo de números negativos según requirements
//- Cálculo de máximo y mínimo valores ingresados







#include <stdio.h>

int main() {
    int numero;
    int factorial = 1;
    
    printf("Ingrese un número para calcular su factorial: ");
    scanf("%d", &numero);
    
    printf("Calculando el factorial de %d:\n", numero);
    
    for (int i = 1; i <= numero; i++) {
        factorial *= i;
    }
    
    printf("El factorial de %d es: %d\n", numero, factorial);
    
    return 0;
}


//##/ Pseudocódigo

//INICIO
 //   ESCRIBIR "Ingrese un número para calcular su factorial:"
 //   LEER numero
 //   factorial ← 1
    
 //   ESCRIBIR "Calculando el factorial de", numero
    
 //   PARA i DESDE 1 HASTA numero HACER
 //       factorial ← factorial × i
 //   FIN PARA
    
 //   ESCRIBIR "El factorial de", numero, "es:", factorial
//FIN
//```

//## Explicación básica

//### ¿Qué es el factorial?

//El factorial de un número es multiplicar ese número por todos los números menores hasta llegar a 1.

//**Ejemplo:** 5! = 5 × 4 × 3 × 2 × 1 = 120

//### ¿Cómo funciona el código?
//  - `scanf("%d", &numero)` lee el número y lo guarda en la variable `numero`
//   - `factorial = 1` (empezamos con 1 porque es el neutro de la multiplicación)

//2. **Bucle FOR**:
//   - Va desde `i = 1` hasta `i = numero` (el número que ingresó el usuario)
//   - En cada vuelta multiplica `factorial` por `i`

//3. **Proceso paso a paso** (ejemplo con 4):
//   - Vuelta 1: `factorial = 1 × 1 = 1`
 //  - Vuelta 2: `factorial = 1 × 2 = 2`
 //  - Vuelta 3: `factorial = 2 × 3 = 6`
 //  - Vuelta 4: `factorial = 6 × 4 = 24`

//4. **Resultado**: Si el usuario ingresa 4, entonces 4! = 24

//### Elementos clave del código:

//-/- **Bucle FOR**: Perfecto para este problema porque sabemos exactamente cuántas veces repetir
//- **Variable acumuladora**: `factorial` guarda el resultado que se va multiplicando

//**Ejemplo de ejecución**: 

//Ingrese un número para calcular su factorial: 4
//Calculando el factorial de 4:
//El factorial de 4 es: 24
