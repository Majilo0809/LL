En este ejercicio se trabajó con una gramática que inicialmente presentaba recursividad por la izquierda en el no terminal S. Para poder aplicar correctamente los algoritmos de análisis sintáctico predictivo, se eliminó dicha recursividad utilizando la transformación estándar, introduciendo un nuevo no terminal S'. Esto permitió obtener una gramática equivalente pero adecuada para el análisis.

Los resultados obtenidos muestran que, aunque la recursividad por la izquierda fue eliminada y los conjuntos de primeros y siguiees fueron calculados, la gramática no es LL1. Esto se debe a que existen intersecciones en los conjuntos de predicción, particularmente en el no terminal B, lo que genera ambigüedad al momento de seleccionar una producción con un solo símbolo de entrada. Por lo tanto, no es posible construir un analizador sintáctico predictivo determinista para esta gramática sin realizar transformaciones adicionales.

<img width="758" height="624" alt="image" src="https://github.com/user-attachments/assets/f3445ce5-f7a8-43fb-8d0f-41b6421d63cd" />

## ASDR
<img width="800" height="64" alt="image" src="https://github.com/user-attachments/assets/e3d60be7-c332-4a4d-b504-9bb9e29718e7" />
- Tokens = ["dos", "cuatro", "tres", "uno", "$"]
El analizador descendente recursivo implementado refleja correctamente la estructura de la gramática sin recursividad por la izquierda y permite validar cadenas de entrada. Sin embargo, debido a la existencia de conflictos en los conjuntos de predicción, la gramática no es LL(1), lo que puede generar ambigüedades durante el análisis y afectar la determinación de la producción correcta en ciertos casos.
