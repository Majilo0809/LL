## Eliminación de recursividad por la izquierda
La única producción con recursividad por la izquierda es:
- B → B cuatro C cinco | ε

Aplicando la transformación:

A -> A α | β
-> A -> β A'
-> A' -> α A' | ε

## Cálculo de Primeros, Siguientes y conjuntos de prediccion
<img width="731" height="775" alt="image" src="https://github.com/user-attachments/assets/34423b23-2800-4c30-9b39-0dc8496ca762" />

## Verificación LL(1)
Se comparan las producciones de un mismo no terminal:
S → A B C → { dos, cuatro, seis }
S → D E → { uno, cuatro }
Existe intersección en “cuatro”.
Por lo tanto, la gramática no es LL(1).
## ASDR
<img width="803" height="45" alt="image" src="https://github.com/user-attachments/assets/0076aaf5-dc35-4724-9ec1-ae52f7c66f9b" />

El ASDR implementado permite validar cadenas de entrada siguiendo la estructura de la gramática transformada. Sin embargo, debido a que la gramática no es LL(1), pueden existir ambigüedades en la selección de producciones, por lo que el analizador puede no comportarse de manera determinista en todos los casos
