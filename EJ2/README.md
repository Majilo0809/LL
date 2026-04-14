
Los resultados obtenidos muestran que los conjuntos Primeros y Siguientes fueron calculados correctamente considerando que hay varias producciones con ε, lo que genera una alta propagación entre los conjuntos.
Al analizar los conjuntos de predicción, se identificaron intersecciones entre producciones del mismo no terminal, especialmente en el caso de S, lo que indica ambigüedad en la selección de reglas. 
Por esta razón, se concluye que la gramática no es LL(1), ya que no permite tomar decisiones determinísticas con un solo símbolo de entrada.

<img width="740" height="595" alt="image" src="https://github.com/user-attachments/assets/87baabc7-668d-4072-ae32-58d80c683cfd" />

## ASDR
<img width="800" height="64" alt="image" src="https://github.com/user-attachments/assets/ce36be19-21d5-4a6e-9987-c44d22f6529e" />
tokens = ["dos", "siete", "cinco", "seis", "uno", "$"]

El ASDR permite simular el análisis de cadenas de acuerdo con la gramática dada, consumiendo tokens de forma secuencial. No obstante, al no ser una gramática LL(1), pueden presentarse conflictos en la elección de producciones, lo que limita la capacidad del analizador para tomar decisiones únicas en todos los casos.
