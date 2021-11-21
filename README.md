# aes256

AES-256 pasa por 14 rondas de encriptación, consistente en una serie de procesos que incluyen la sustitución, 
trasposición y mezcla del texto plano de entrada para obtener así el texto encriptado de salida.
    
Expansión de claves y AddRoundKey. 

Esta es la ronda que tiene que ver con las claves, y en cada caso ejecuta una operación lógica XOR con un subconjunto de la clave.
SubBytes. Substituye los bytes de todo el bloque para producir un valor alternativo, de una manera realmente imposible de descifrar mediante computación convencional.

ShiftRows.
Mueve los datos de la matriz.

MixColumns. 

Aplica un XOR bit a bit y una multiplicación de matrices que lleva a un resultado final de 4 filas y 1 columna, por lo que volvemos a datos secuenciales y dejamos de tener la matriz.

Otra cuestión relevante del cálculo es de qué manera se estructura la información, 
pues no se hace de manera secuencial como cabría imaginarse, sino que se organiza en
bloques de matrices de 128 bits con 4 filas y 4 columnas.
