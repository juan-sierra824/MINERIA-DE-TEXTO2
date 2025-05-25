# Análisis Comparativo de Textos: Rexixtenxia Norte vs. Operación Bin Laden

## Descripción General del Proyecto

Este proyecto de análisis textual tuvo como objetivo aplicar técnicas de minería de texto y procesamiento de lenguaje natural (PLN) a dos documentos con temáticas y estilos narrativos completamente diferentes:

1. "Rexixtenxia Norte": un comunicado emocional de la barra brava del Independiente Medellín previo a un clásico futbolero.
2. "Operación Bin Laden": un texto informativo que describe el operativo militar estadounidense que resultó en la muerte de Osama bin Laden.

El propósito fue extraer patrones lingüísticos, estructuras gramaticales y relaciones semánticas que revelaran diferencias en tono, estilo, propósito comunicativo y temas tratados.

## Etapas del Proyecto
----------------------------------------
### 1. Recolección de los textos

Los textos fueron obtenidos en formato `.txt` y cargados al entorno de trabajo. Cada archivo contenía múltiples repeticiones del contenido base, lo que permitió trabajar con un corpus uniforme de 1000 palabras por texto.
-------------------------------------
### 2. Normalización del texto

Se aplicó una función `normalize()` para limpiar los textos:
- Eliminación de etiquetas HTML.
- Remoción de URLs.
- Supresión de emojis y caracteres no ASCII.
- Reemplazo de guiones especiales por espacios.
- Conversión a minúsculas.
- Eliminación de signos de puntuación y espacios redundantes.
-------------------------------------------
### 3. Estadísticas básicas del contenido

Se analizaron:
- Número de párrafos.
- Número de frases.
- Total de palabras.

Este análisis estructural permitió comparar la longitud y complejidad de los textos de forma inicial.

### 4. Tokenización, lematización y eliminación de stopwords (con spaCy)

Se aplicaron:
- Tokenización: división del texto en unidades léxicas.
- Lematización: transformación de palabras a su forma base.
- Remoción de stopwords: eliminación de palabras comunes sin valor semántico.
---------------------------------------------------
### 5. Análisis de frecuencia léxica

Se identificaron las palabras más frecuentes en ambos textos para comprender los conceptos clave:

- Rexixtenxia Norte: barra, equipo, clásico, hinchada, jugadores.
- Operación Bin Laden: bin, laden, operación, fuerzas, estadounidenses.

### 6. Visualización mediante nubes de palabras
---------------------------------------
Se generaron nubes de palabras globales y también por categoría gramatical (sustantivos, verbos, adjetivos), lo que permitió detectar de forma visual los temas y enfoques de cada texto.

### 7. Etiquetado gramatical (POS Tagging)

Se clasificaron palabras por tipo:
- Sustantivos: temas y actores.
- Verbos: acciones dominantes.
- Adjetivos: tono y estilo narrativo.
-------------------
### 8. Extracción de tripletas SVO (Sujeto–Verbo–Objeto)

Se analizaron estructuras como:
- Rexixtenxia: ("barra", "concluyó", "jugadores") → tono crítico y emocional.
- Bin Laden: ("operativo", "anunció", "kilómetros") → enfoque técnico y objetivo.
------------------------------------------------------------
## Hallazgos más importantes

### 1. Tonalidad contrastante

- **Rexixtenxia Norte**: El texto adopta un tono emocional, exigente y colectivo. Se percibe un lenguaje apelativo dirigido a los jugadores, con expresiones de orgullo y compromiso por parte de la hinchada. La reiteración de frases como “esto no es solo un juego” refuerza la carga simbólica del mensaje.
  
- **Operación Bin Laden**: El tono es formal, descriptivo y objetivo. Se prioriza la claridad informativa sobre los hechos, destacando la participación de actores institucionales y detalles operativos. No hay juicios emocionales, sino una intención de relatar hechos de forma cronológica.

### 2. Temas y actores centrales

- **Rexixtenxia Norte**: Los actores principales son la barra, los hinchas y el equipo. Se construye una relación simbiótica entre estos, donde la hinchada tiene la autoridad moral para exigir entrega y respeto. El texto gira en torno al clásico paisa y su significado como evento de identidad local.
- **Operación Bin Laden**: Los protagonistas son las fuerzas especiales estadounidenses, Barack Obama y Osama Bin Laden. El enfoque está puesto en el operativo como culminación de una estrategia militar. También aparecen actores secundarios como el gobierno pakistaní y la Casa Blanca.

### 3. Verbos y acciones

- **Rexixtenxia Norte**: Los verbos más frecuentes tienen un carácter exhortativo: exigir, apoyar, convocar, manifestar. Reflejan acciones de la hinchada hacia el equipo, demostrando un rol participativo y activo dentro del relato.
- **Operación Bin Laden**: Se destacan verbos técnicos y narrativos como ejecutar, anunciar, localizar, abatir. Estos verbos relatan el desarrollo de un operativo real, con acciones planificadas y comunicadas oficialmente.

### 4. Estilo narrativo

- **Rexixtenxia Norte**: Estilo discursivo informal, directo y con repeticiones que refuerzan la idea de presión emocional. Se nota una fuerte carga valorativa que busca conmover o movilizar.
- **Operación Bin Laden**: Estilo expositivo, objetivo y lineal. El texto está estructurado para informar de manera clara, sin subjetividades, ideal para un entorno periodístico o académico.

### 5. Relaciones SVO (Sujeto–Verbo–Objeto)

- **Rexixtenxia Norte**: Las tripletas extraídas (como “la barra concluyó jugadores”) evidencian un sujeto colectivo que ejerce juicio sobre otros. Esto refleja el papel activo de la hinchada como voz de autoridad emocional.
- **Operación Bin Laden**: Tripletas como “el operativo anunció kilómetros” reflejan estructuras informativas, muchas veces impersonales. Se enfoca en la transmisión de hechos logísticos, distanciados de la subjetividad.

### 6. Distribución gramatical por categoría (POS tagging)

- **Rexixtenxia Norte**: Predominan los sustantivos relacionados con fútbol, hinchada y emociones; los verbos expresan exigencia o compromiso; los adjetivos refuerzan la carga emocional del mensaje (ej. “incondicional”, “crucial”).
- **Operación Bin Laden**: Los sustantivos apuntan a conceptos militares y geopolíticos; los verbos están orientados a la acción estratégica; los adjetivos son más técnicos o geográficos (ej. “fortificada”, “militar”, “estadounidense”).

### 7. Frecuencia léxica y temas clave

- **Rexixtenxia Norte**: Palabras más frecuentes como barra, rexixtenxia, equipo, clásico, hinchada indican un enfoque centrado en el fútbol, la identidad barrista y la exigencia de compromiso.
- **Operación Bin Laden**: Términos como bin, laden, operación, fuerzas, estadounidense muestran un texto técnico, basado en hechos históricos y militares.

### 8. Visualización y comprensión rápida

- Las **nubes de palabras** facilitaron la interpretación del contenido sin necesidad de leer línea por línea.
- En Rexixtenxia, las nubes mostraron un entorno semántico afectivo y simbólico; en Bin Laden, un contexto operacional y noticioso.


--------------------------------------------------------------------------

## Conclusiones Finales

- La minería de texto permitió identificar temas, actores y estructuras discursivas sin leer todo manualmente.
- Las técnicas de PLN aplicadas facilitaron una lectura profunda y comparativa.
- El análisis sintáctico y las visualizaciones aportaron una comprensión más rica de cada documento.
- Las diferencias entre textos no solo radican en el tema, sino en cómo están construidos lingüísticamente.
---------------------------------------
## Archivos involucrados

- `REXIXTENXIA NORTE.txt`
- `OPERATIVO.txt`
-------------------------------

## ✍️ Autor
Juan Esteban Sierra  
Proyecto de análisis de texto con enfoque en minería de datos CIENCIA DE DATOS 1. UNIVERSIDAD AUTONOMA LATINOAMERICANA
