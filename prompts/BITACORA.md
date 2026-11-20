# Bitacora de prompts

Laboratorio 06: Fundamentos de Ingenieria de Prompts.

Herramienta de IA usada: GPT

## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. | 34| 7|
| The students program in Java. | 29| 6|
| desafortunadamente | 28| 4|

La IA necesita informacion o contexto de la cual obtener informacion y generar una respuesta.

## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100%| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3%| BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 1 | 44.5%| LibroYa, PrestaLibro, BiblioTec, BiblioTec, BiblioTec|
| 1.8 | 32.2%| BiblioTec, LibroYa, BiblioTec, BiblioTec, PrestaLibro |

Con el ajuste de la temperatura a 1.8 las probabilidades se ditribuyen en las demas palabras.

## Ejercicio 4: Prompt vago vs estructurado

| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema | Si| Si|
| Menciona a los usuarios principales | No| Si|
| Tiene exactamente 3 funcionalidades | No| Si|
| Esta en 3 parrafos | No| Si|
| Lo usaria en un informe real | No| Si|


## Ejercicio 5: Anatomia de un prompt

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Crea un programa en Java.|
| Instruccion | Actua como desarrollador Java. Crea un programa en Java.|
| Contexto | Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda.|
| Ejemplo | Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto con los atributos codigo, nombre, precio y stock.|
| Formato | Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto con los atributos codigo, nombre, precio y stock. Explica primero la estructura de la clase y luego presenta el codigo Java.|
| Estilo | Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto con los atributos codigo, nombre, precio y stock. Explica primero la estructura de la clase y luego presenta el codigo Java. Usa este estilo para los metodos: getPrecio(), setPrecio(double precio).|

