# Practicas_Curriculares

# Del comentario a la conversación: análisis de YouTube con Python y NLP

**Proyecto de Ciencia de Datos | Python · NLP · Machine Learning · Estadística**

Este proyecto desarrolla un análisis exploratorio de conversaciones en YouTube mediante técnicas de extracción automatizada de datos, procesamiento del lenguaje natural (NLP), Machine Learning y estadística.

El objetivo es estudiar **de qué hablan los usuarios, cómo expresan sus opiniones y qué características están relacionadas con la participación**, prestando especial atención a las diferencias entre comentarios principales y respuestas.

## Datos analizados

El estudio consta de dos fases:

| Fase | Datos | Finalidad |
|---|---|---|
| Estudio piloto | 1.179 comentarios | Exploración metodológica y comparación de modelos de IA |
| Análisis ampliado | 5.531 comentarios de seis vídeos | Análisis temático, emocional, conversacional y estadístico |

En el análisis ampliado se identificaron 3.792 comentarios principales y 1.739 respuestas.

## Metodología

1. **Extracción y preparación:** recopilación de comentarios y metadatos mediante `yt-dlp`, limpieza con `pandas` y reconstrucción de conversaciones.
2. **Análisis temático:** aplicación de TF-IDF y NMF para identificar patrones de palabras y agrupar comentarios por temas.
3. **Procesamiento del lenguaje:** clasificación de sentimiento y estimación de hostilidad mediante `pysentimiento`, con uso complementario de Gemini y Qwen.
4. **Análisis de participación:** estudio de likes, respuestas e interacciones entre usuarios.
5. **Análisis estadístico:** regresiones logísticas, comparaciones ajustadas y comprobaciones de incertidumbre mediante bootstrap.
6. **Visualización:** elaboración de tablas y gráficos para comunicar los resultados.

## Principales resultados

- El **73,51 %** de los comentarios del análisis ampliado fue clasificado con sentimiento negativo.
- El tema predominante, relacionado con la seguridad y los fallos ferroviarios, agrupó aproximadamente el **48,83 %** de los comentarios.
- El **53,48 %** de las respuestas presentó una puntuación de agresividad superior a la del comentario al que contestaba, aunque el incremento medio fue pequeño (+0,015).
- Después de considerar el vídeo, el tema y la longitud del comentario, no se encontró evidencia estadística suficiente de que los comentarios negativos recibieran más respuestas.
- Se identificaron **783 comentarios con signos de interrogación**, cuya interpretación requiere distinguir preguntas informativas de preguntas retóricas.

Los resultados representan asociaciones observadas en los vídeos estudiados, no relaciones causales.

## Tecnologías utilizadas

**Python · pandas · NumPy · scikit-learn · pysentimiento · statsmodels · yt-dlp · Gemini · Qwen · Matplotlib · Seaborn · Jupyter Notebook**

## Limitaciones

El estudio se basa en un número limitado de vídeos. Las clasificaciones realizadas por modelos de inteligencia artificial pueden contener errores, especialmente ante ironía, ambigüedad o expresiones que requieren contexto.

Las puntuaciones de agresividad son estimaciones automáticas y no equivalen directamente a la presencia de amenazas o violencia.

Como futuras mejoras se plantea ampliar el conjunto de datos, realizar validaciones humanas y desarrollar análisis temporales de las conversaciones.

## Estado del proyecto

**Análisis exploratorio completado**, con posibles ampliaciones metodológicas y validaciones pendientes.




