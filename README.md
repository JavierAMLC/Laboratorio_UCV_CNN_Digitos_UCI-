# Laboratorio_UCV_CNN_Digitos_UCI-

¿Qué diferencia existe entre una red densa y una CNN? 
La red densa aplana las imágenes perdiendo la geometría local y eleva exponencialmente los parámetros. La CNN mantiene la forma nativa bidimensional usando filtros compartidos para preservar el espacio y ahorrar cómputo.
¿Qué función cumple una capa convolucional? 
Extrae características visuales de forma automática deslizando filtros matemáticos para detectar patrones esenciales como bordes, texturas y esquinas.
¿Qué representa un filtro en una CNN? 
Representa una pequeña matriz de pesos ajustables que busca un patrón geométrico específico; si este coincide con la imagen, genera una activación alta.
¿Qué función cumple MaxPooling? 
Reduce el tamaño de los mapas de características tomando solo el valor máximo de cada región. Esto ahorra memoria computacional y aporta invarianza a pequeñas traslaciones.
¿Por qué normalizamos los valores de píxeles? 
Porque escala los valores originales (0-16) al rango estándar [0, 1]. Esto estandariza las entradas, estabiliza los gradientes y acelera la convergencia del entrenamiento.
¿Por qué usamos softmax en la capa de salida? 
Porque transforma las salidas numéricas crudas en una distribución de probabilidades que suma exactamente 1, definiendo el nivel de confianza para cada dígito.
¿Qué dígitos se confundieron más en la matriz de confusión?
Las mayores confusiones ocurren en dígitos visualmente parecidos debido al trazo, principalmente entre el 1 y el 7 (por la inclinación) o entre el 3, el 8 y el 9 (por curvas abiertas o bucles similares).
¿Por qué algunos dígitos escritos a mano son difíciles de clasificar? 
Debido a la alta variabilidad de la caligrafía humana (estilos e inclinaciones) combinada con la bajísima resolución de este dataset (8x8 píxeles), lo que causa una pixelación extrema que borra los detalles finos.
¿Qué ventajas tendría usar imágenes de mayor resolución?
Más píxeles (como 28x28) aportan nitidez y trazos continuos, permitiendo que los filtros extraigan rasgos mucho más exactos y discriminativos, disminuyendo los errores.
¿Qué limitaciones tiene este laboratorio frente a un sistema OCR real?
En el laboratorio los dígitos ya están perfectamente limpios, aislados, centrados y recortados. Un OCR real debe resolver la segmentación de texto continuo, limpiar ruido de fondo (manchas/sombras), procesar fuentes variadas y entender el contexto semántico.
