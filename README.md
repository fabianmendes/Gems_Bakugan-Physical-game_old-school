# 🐲 Bakugan Data Expert🐉 🧾eConsulting: Gs & More

Un agente de IA personalizado (Gem) impulsado por el modelo de Gemini, diseñado específicamente para actuar como la enciclopedia técnica y definitiva de la franquicia Bakugan. 

Este proyecto nació de la necesidad de extraer, limpiar y estructurar miles de datos dispersos sobre el poder G (G-Power) del juego físico y el anime, convirtiéndolos en una base de conocimiento consultable mediante lenguaje natural.

[![Google Badge](https://img.shields.io/badge/Google-Gems-blue?style=flat&logo=google)](https://gemini.google.com/gem/16PXYJfSoG9dfOJaEcexz4MLqSqY3GlFz?usp=sharing)

## ✨ Características Principales (Features)

* **Extracción Precisa de G-Power:** Proporciona tablas detalladas de poder separadas por Atributos (Pyrus, Aquos, Subterra, Haos, Darkus, Ventus, Clear), incluyendo ediciones especiales exclusivas (Translucent, Japan releases, BakuEvolutions).
* **Fidelidad de Datos e Ingesta Extrema (Absorción Total Quad-Core):** El agente opera bajo la directiva de consultar primero la base de datos local. En caso de requerir un *fallback* o búsqueda externa, ejecuta una **Búsqueda Multifuente en 4 ejes estratégicos de forma simultánea**:
  1. `bakugan.fandom.com/wiki/` (Canon occidental y extracción obligatoria del nombre original en Japonés).
  2. `bakugan.wiki/wiki/` (Registro de lanzamientos físicos en América y Europa).
  3. `bakugan.fandom.com/es/wiki/` (Wiki en español, vital para rescatar ediciones omitidas en inglés).
  4. `bakucolle.com` (El archivo definitivo de coleccionismo en Japón, usando el término en japonés extraído).
  
  *Sin visión de túnel:* El bot escanea de forma agresiva **la totalidad de cada página web** (artículos principales, infoboxes, galerías de imágenes, pies de foto y notas de trivia) para capturar lanzamientos ultra-raros u ocultos (como la versión *Pearl* de Clayf).
* **Integración de Battle Gears & Evoluciones:** Identifica y vincula automáticamente los Battle Gears, BakuNanos y Mechtogans asociados a cada Bakugan.
* **Diseño UI/UX Optimizado:** Las variaciones y evoluciones de los Bakugan se renderizan utilizando formato de **código en línea** (acentos graves `` ` ``), eliminando las antiguas etiquetas HTML. Esto facilita aislar el texto para dar doble toque y "Copiar y Pastear" rápidamente desde cualquier dispositivo móvil o de escritorio.
* **Agente Interactivo:** No solo entrega datos, sino que guía la conversación. El bot pregunta proactivamente si el usuario desea desglosar el poder de los Battle Gears por tratamientos de metal (Gold, Silver, Copper) o si requiere la extracción/generación directa del *Thumbnail* (imagen oficial) desde la Wiki.

## 🛠️ Stack & Herramientas

* **Python & Pandas:** Limpieza y estructuración del archivo maestro en formato `.csv` separado por temporadas (S1 a S4). Con una pestaña principal de archivo maestro para poder ser procesado por el Gemini desde el `gSheets`.
* **BeautifulSoup & Requests (Web Scraping):** Automatización de extracción de Infoboxes desde Fandom/Wikia.
* **Google Gemini (Gems):** Motor de Procesamiento de Lenguaje Natural y razonamiento lógico para cruzar los datos.

[![gColabs Badge](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://colab.research.google.com/drive/1Rj9r4xzLbDmMww4n8XbGruGe2fqn6hZ6?usp=sharing)
[![gSheets Badge](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)](https://docs.google.com/spreadsheets/d/1g8TjyF7CRJYDMCVDxPnjEMgLlBZ3dO8bOfS_tF7NLYA/edit?usp=sharing)
[![gGemini Badge](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://gemini.google.com/gem/16PXYJfSoG9dfOJaEcexz4MLqSqY3GlFz?usp=sharing)
![gGemini Badge](https://img.shields.io/badge/Wiki%20js-1976D2?style=for-the-badge&logo=Wikidotjs&logoColor=white)

![by-sa](https://licensebuttons.net/l/by-sa/3.0/88x31.png)

## 🚀 Cómo funciona

Al preguntarle al Agente por un Bakugan (Ej. *"Clayf"*), este procesa el archivo maestro y ejecuta en tiempo real su **Protocolo de Extracción Quad-Core de Absorción Total (v1.2.1)**. Cruza instantáneamente los textos, las tablas globales y los repositorios fotográficos para estructurar un veredicto definitivo sin importar en qué rincón de la red estuviese oculta la variante física.
