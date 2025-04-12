# Proyectos-Deep-Learning
# Clasificación del Estado de los Ojos con Señales EEG usando LSTM

Este proyecto implementa un modelo de red neuronal LSTM para clasificar si los ojos están abiertos o cerrados a partir de señales EEG. Se utiliza el dataset **EEG Eye State** del repositorio de la UCI.  
La clase **0** representa **ojos abiertos** y la clase **1** representa **ojos cerrados**.

---

##  ¿Qué hace este proyecto?

El modelo toma señales EEG registradas por 14 sensores y predice si la persona tenía los ojos abiertos (0) o cerrados (1). El flujo del código incluye:

1. **Carga y análisis de datos**  
   Se exploran las señales EEG, se revisa la distribución de clases y se visualizan correlaciones entre canales.

2. **Preprocesamiento**  
   Se normalizan los datos y se convierten en secuencias de tiempo para poder usar redes neuronales LSTM.

3. **Construcción del modelo**  
   Se diseña una red LSTM con capas `Dropout` y `Dense` para evitar el sobreajuste y mejorar el aprendizaje.

4. **Entrenamiento del modelo**  
   Se usa el optimizador **Adam**, función de pérdida `binary_crossentropy`, validación cruzada y `early stopping`.

5. **Evaluación**  
   Se analiza la precisión del modelo, matriz de confusión y gráficas de entrenamiento (pérdida y precisión).

6. **Visualización de señales EEG**  
   Se generan gráficos que muestran cómo evoluciona el entrenamiento y ejemplos de señales EEG por clase.



