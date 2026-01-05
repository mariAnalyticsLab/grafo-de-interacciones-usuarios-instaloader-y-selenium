# grafo-de-interacciones-usuarios-instaloader-y-selenium

## Web Scraping de Instagram y Grafo de Interacciones
#### Selenium · Undetected Chromedriver · Instaloader · NetworkX

## 📌 Descripción del algoritmo
Este proyecto implementa un flujo de recolección y análisis de interacciones en Instagram mediante técnicas de web scraping y análisis de redes.
A partir de una cuenta objetivo, el algoritmo extrae información pública de publicaciones, comentarios, menciones y usuarios etiquetados, para finalmente construir un grafo de interacciones reales entre usuarios.
El objetivo principal es modelar las relaciones sociales visibles en una cuenta de Instagram utilizando grafos, lo que permite analizar patrones de interacción, centralidad y conexiones entre usuarios.

## ⚙️ Funcionamiento básico
El algoritmo se divide en varias etapas:
1. Acceso y navegación en Instagram
- Inicio de sesión automatizado usando Selenium con Undetected Chromedriver.
- Búsqueda de la cuenta objetivo.
- Scroll automático para obtener enlaces de publicaciones (posts y reels).
2. Extracción de información
Para cada publicación:
- Usuarios que comentaron.
- Usuarios que comentaron.
- Menciones (@usuario) en comentarios y descripciones.
- Usuarios etiquetados en la publicación.
- Se utilizan conjuntos (set) para evitar duplicados y asegurar datos únicos.
3. Limpieza y procesamiento de datos
- Normalización de nombres de usuario.
- Eliminación de emojis en menciones.
- Separación de usuarios comentadores, mencionados y etiquetados.
4. Construcción del grafo de interacciones
- Creación de un grafo usando NetworkX.
- Cada nodo representa un usuario real de Instagram.
- Cada arista representa una interacción (comentario, mención o etiquetado).
- Visualización del grafo con Matplotlib.

## 📊 Resultados y aprendizajes obtenidos
- Representación visual de comunidades e interacciones reales.
- Identificación de usuarios con mayor nivel de interacción.
Comprensión práctica de:
- Web scraping dinámico.
- Manejo de contenido cargado dinámicamente.
- Modelado de redes sociales mediante grafos.
- Integración de scraping + análisis de datos + visualización.

## 🛠️ Herramientas y tecnologías utilizadas
- Python
- selenium
- Undetected Chromedriver
- instaloader
- BeautifulSoup
- pandas
- networkX
- matplotlib
- regex
- emoji

## 📁 Datos y archivos importantes
- Grafo_de_interacciones_usuarios_Instaloader_y_Selenium.ipynb
Notebook principal con todo el flujo:
- Scraping
- Procesamiento
- Construcción del grafo
- Visualización
⚠️ Los datos generados dependen de contenido público y del estado de la cuenta analizada al momento de la ejecución.

## ⚠️ Limitaciones
- El scraping depende de la estructura cambiante de Instagram.
- Riesgo de bloqueos temporales si se ejecuta con alta frecuencia.
- No se analizan cuentas privadas.
- El grafo refleja interacciones visibles, no relaciones reales fuera de la plataforma.
- El uso de nombres de usuario reales implica responsabilidad ética.

## ⚖️ Consideraciones éticas y legales
- Este proyecto tiene fines educativos y académicos.
Se recomienda:
- Analizar solo cuentas propias o con consentimiento.
- No redistribuir datos sensibles.
- Respetar los términos de servicio de Instagram.

## 📄 Licencia
Este proyecto se distribuye bajo la licencia MIT, permitiendo su uso, modificación y distribución con fines académicos y de aprendizaje, siempre que se mantenga el aviso de copyright.
