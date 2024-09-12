# analysis-food-product-app
Proyecto realizado para una start-up que vende productos alimenticios a través de su aplicación móvil. 

### Descripción del proyecto

El objetivo fue analizar el comportamiento de los usuarios en el embudo de ventas y evaluar los resultados de un experimento A/A/B. El equipo de diseño está considerando cambiar las fuentes de la aplicación, y se llevó a cabo el test para determinar si el nuevo diseño afecta de manera negativa o positiva la experiencia del usuario.

### Objetivos del Análisis
1. **Análisis del embudo de ventas**: Evaluar cómo los usuarios navegan a través de las distintas etapas del embudo de ventas, identificando los puntos de mayor abandono.
2. **Evaluación del experimento A/A/B**: Comparar el comportamiento de los usuarios entre dos grupos de control con las fuentes antiguas y un grupo de prueba con las fuentes nuevas, para determinar si los cambios en el diseño tienen un impacto significativo.

### Datos Utilizados
El dataset incluye información sobre los eventos registrados en la aplicación:

* **EventName**: Tipo de evento (acción realizada por el usuario).
* **DeviceIDHash**: Identificador único del dispositivo del usuario.
* **EventTimestamp**: Marca temporal del evento.
* **ExpId**: Número del grupo experimental (246 y 247 para los grupos de control, 248 para el grupo de prueba).

### Análisis Realizado
1. Preparación de los datos:
   - Limpieza de los datos, conversión de tipos de datos y manejo de valores faltantes.
   - Creación de nuevas columnas de fecha y hora para un análisis temporal más preciso.
2. Análisis del embudo de ventas:
   - Identificación de eventos clave dentro de la aplicación y su frecuencia.
   - Construcción del embudo de ventas para analizar la proporción de usuarios que avanzan de una etapa a otra.
   - Identificación de las etapas donde se produce la mayor pérdida de usuarios y cálculo del porcentaje de usuarios que completan el viaje hasta la compra.

3. Análisis del test A/A/B:
   - Comparación estadística entre los dos grupos de control (246 y 247) para validar la consistencia del experimento.
   - Comparación del grupo de prueba (248) con los grupos de control para identificar diferencias significativas en el comportamiento de los usuarios.
   - Evaluación de eventos clave, como la acción más popular, y análisis de la proporción de usuarios que la realizaron en cada grupo.
4. Prueba de hipótesis:
   - Aplicación de pruebas estadísticas para verificar la significancia de los resultados y determinar si las diferencias observadas son relevantes.

### Herramientas y Tecnologías
* Python: Para la manipulación y análisis de los datos.
* Pandas y Numpy: Para el procesamiento de datos.
* Matplotlib y Seaborn: Para la visualización de los resultados.
* Jupyter Notebook: Para la presentación del análisis y los resultados.
* Pruebas de hipótesis estadísticas: Para comparar los resultados entre los grupos A/A/B.

### Conclusiones
* Embudo de ventas: Se identificaron las etapas con mayor abandono y el porcentaje de usuarios que completan el proceso de compra.
* Resultados del experimento A/A/B: No se observaron diferencias estadísticamente significativas entre los grupos de control, lo que confirma la validez del experimento. En cuanto al grupo de prueba, se encontraron diferencias menores en la interacción de los usuarios, pero no lo suficiente como para concluir que el cambio en las fuentes afectó negativamente la experiencia del usuario.
* Recomendación: Basado en los resultados, no parece necesario revertir los cambios en las fuentes. Sin embargo, se recomienda realizar más pruebas a largo plazo para evaluar el impacto a medida que los usuarios se acostumbran al nuevo diseño.
