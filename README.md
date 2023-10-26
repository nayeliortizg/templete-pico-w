# templete-picow
Para trabajos de microcontroladores

# Ver el directorio de /code/ para como documentar un programa con sus pantallas, etc.

```C
/*
 * Nombre del Archivo: main.c
 * Autor:   Ortiz Garcia Nayeli
 * Correo:  l21210406@tectijuana.edu.mx
 * Fecha:   25/10/2023
 * Curso:   Lenguajes de Interfaz, TECNM Campus ITT
 * 
 * Objetivo:
 * Imprimir la tabla de multiplicar hasta 12 x 12.
 *
 * Historial de Revisiones:
 * 25/10/2023       Ortiz Garcia Nayeli - Creado
 * 25/10/2023       Ortiz Garcia Nayeli - Actualizado para añadir [característica/corrección]
 *
 */

#include <stdio.h>
#include "pico/stdlib.h"

int main()
{
    stdio_init_all();

    for (int i = 1; i <= 12; i++) {
        for (int j = 1; j <= 12; j++) {
            int resultado = i * j;
            printf("%d x %d = %d\n", i, j, resultado);
        }
        printf("\n"); // Línea en blanco entre tablas de multiplicar
    }

    while (true) {
        sleep_ms(5000); // Esperar 5 segundos antes de imprimir de nuevo
    }

    return 0;
}

```
