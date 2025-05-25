# MINERIA DE TEXTO
# Análisis Comparativo de Textos: Rexixtenxia Norte vs. Operación Bin Laden

## Descripción General del Proyecto

Este proyecto de análisis textual tuvo como objetivo aplicar técnicas de *minería de texto* y *procesamiento de lenguaje natural (PLN)* a dos documentos con temáticas y estilos narrativos completamente diferentes:

1. *"Rexixtenxia Norte"*: un comunicado emocional de la barra brava del Independiente Medellín previo a un clásico futbolero.
2. *"Operación Bin Laden"*: un texto informativo que describe el operativo militar estadounidense que resultó en la muerte de Osama bin Laden.

El propósito fue extraer patrones lingüísticos, estructuras gramaticales y relaciones semánticas que revelaran diferencias en tono, estilo, propósito comunicativo y temas tratados.

---

##  Etapas del Proyecto

### 1.Recolección de los textos
Los textos fueron obtenidos en formato .txt y cargados al entorno de trabajo. Cada archivo contenía múltiples repeticiones del contenido base, lo que permitió trabajar con un corpus uniforme de 1000 palabras por texto.

### 2. Normalización del texto
Se aplicó una función normalize() para limpiar los textos:
- Eliminación de etiquetas HTML.
- Remoción de URLs.
- Supresión de emojis y caracteres no ASCII.
- Reemplazo de guiones especiales por espacios.
- Conversión a minúsculas.
- Eliminación de signos de puntuación y espacios redundantes.

Este paso aseguró una base de datos textual homogénea para el análisis posterior.

### 3. Estadísticas básicas del contenido
Se analizaron:
- Número de párrafos.
- Número de frases.
- Total de palabras.

Este análisis estructural permitió comparar la longitud y complejidad de los textos de forma inicial.

### 4.Tokenización, lematización y eliminación de stopwords (con spaCy)
Usando spaCy, se aplicaron las siguientes transformaciones:
- *Tokenización*: división del texto en unidades léxicas (palabras).
- *Lematización*: conversión de palabras a su forma base.
- *Remoción de stopwords*: eliminación de palabras funcionales sin valor semántico fuerte (como "el", "de", "la", etc.).

Esto permitió obtener las palabras más significativas y representativas de cada documento.

### 5. Análisis de frecuencia léxica
Se contaron las palabras más frecuentes después del procesamiento lingüístico. Se identificaron las *top 30* por frecuencia y se analizaron las *top 5* para cada texto, revelando los temas centrales de cada uno:

- *Rexixtenxia Norte*: barra, equipo, clásico, hinchada, jugadores.
- *Operación Bin Laden*: bin, laden, operación, fuerzas, estadounidenses.

### 6. Visualización mediante nubes de palabras
Se generaron *nubes de palabras globales* y *nubes por categoría gramatical* (sustantivos, verbos y adjetivos). Estas visualizaciones facilitaron una comprensión intuitiva del contenido y del enfoque temático de cada documento.

### 7.  Etiquetado gramatical (POS Tagging)
Se aplicó análisis gramatical para clasificar las palabras por su categoría:
- *Sustantivos*: revelan los temas clave.
- *Verbos*: muestran las acciones más importantes.
- *Adjetivos*: indican descripciones y tono emocional o técnico.

Este análisis mostró que el texto de Rexixtenxia se centra en exigencias emocionales y colectivas, mientras que el de Bin Laden presenta un enfoque narrativo técnico y descriptivo.

### 8. Extracción de tripletas SVO (Sujeto–Verbo–Objeto)
Se identificaron estructuras SVO representativas de cada texto:

- *Rexixtenxia Norte*: (“barra”, “concluyó”, “jugadores”) → una construcción que refleja autoridad y presión emocional.
- *Operación Bin Laden*: (“operativo”, “anunció”, “kilómetros”) → una estructura técnica, asociada a datos objetivos.

Esto permitió revelar cómo se construyen las relaciones entre actores, acciones y objetos en cada narrativa.

---

## Conclusiones Finales

- La *minería de texto* permitió identificar *temas, actores y estructuras discursivas* dominantes sin necesidad de leer manualmente cada línea.
- Se evidenciaron *diferencias claras de tono y propósito*: uno emocional y colectivo, el otro técnico e institucional.
- El uso de *spaCy* y técnicas de PLN demostró ser eficaz para convertir datos textuales complejos en *información estructurada y visualmente comprensible*.
- La combinación de métodos cuantitativos y lingüísticos permitió realizar un análisis profundo y comparativo que va más allá del contenido superficial de los textos

--------------------------------------

## Archivos involucrados
- REXIXTENXIA NORTE.txt
- OPERATIVO.txt
-----------------------------------------

## ✍️ Autor
Juan Esteban Sierra  
Proyecto de análisis de texto con enfoque en minería de datos CIENCIA DE DATOS 1. UNIVERSIDAD AUTONOMA LATINOAMERICANA
