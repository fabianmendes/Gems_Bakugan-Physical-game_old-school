# 🐲 Bakugan Data Expert🐉 🧾eConsulting: Gs & More

Un agente de IA personalizado (Gem) impulsado por el modelo de Gemini, diseñado específicamente para actuar como la enciclopedia técnica y definitiva de la franquicia Bakugan. 

Este proyecto nació de la necesidad de extraer, limpiar y estructurar miles de datos dispersos sobre el poder G (G-Power) del juego físico y el anime, convirtiéndolos en una base de conocimiento consultable mediante lenguaje natural.

[![Google Badge](https://img.shields.io/badge/Google-Gems-blue?style=flat&logo=google)](https://gemini.google.com/gem/16PXYJfSoG9dfOJaEcexz4MLqSqY3GlFz?usp=sharing)

## ✨ Características Principales (Features)

* **Extracción Precisa de G-Power:** Proporciona tablas detalladas de poder separadas por Atributos (Pyrus, Aquos, Subterra, Haos, Darkus, Ventus, Clear), incluyendo ediciones especiales exclusivas (Translucent, Japan releases, BakuEvolutions).
* **Fidelidad de Datos (Extracción Cruzada):** El agente está programado bajo una estricta directiva de consultar primero la base de datos local. Si un dato no existe, el bot informa al usuario con total transparencia y realiza un _fallback_ automático de **Búsqueda Dual**, cruzando datos entre `bakugan.fandom.com` (canon del anime) y `bakugan.wiki` (juego físico) para entregar la lista más exhaustiva.
* **Integración de Battle Gears & Evoluciones:** Identifica y vincula automáticamente los Battle Gears, BakuNanos y Mechtogans asociados a cada Bakugan.
* **Diseño UI/UX Optimizado:** Las variaciones y evoluciones de los Bakugan se renderizan utilizando formato de **código en línea** (acentos graves `` ` ``), eliminando las antiguas etiquetas HTML. Esto facilita aislar el texto para dar doble toque y "Copiar y Pegar" rápidamente desde cualquier dispositivo.
* **Agente Interactivo:** No solo entrega datos, sino que guía la conversación. El bot pregunta proactivamente si el usuario desea desglosar el poder de los Battle Gears por tratamientos de metal (Gold, Silver, Copper) o si requiere la extracción/generación directa del *Thumbnail* (imagen oficial) desde la Wiki.

## 🛠️ Stack & Herramientas

* **Python & Pandas:** Limpieza y estructuración del archivo maestro en formato `.csv` separado por temporadas (S1 a S4). Con una pestana principal de archivo maestro para poder ser procesado por el Gemini desde el `gSheets` 

* **BeautifulSoup & Requests (Web Scraping):** Automatización de extracción de Infoboxes desde Fandom/Wikia.
* **Google Gemini (Gems):** Motor de Procesamiento de Lenguaje Natural y razonamiento lógico para cruzar los datos.


[![gColabs Badge](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252)](https://colab.research.google.com/drive/1Rj9r4xzLbDmMww4n8XbGruGe2fqn6hZ6?usp=sharing)
[![gSheets Badge](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)](https://docs.google.com/spreadsheets/d/1g8TjyF7CRJYDMCVDxPnjEMgLlBZ3dO8bOfS_tF7NLYA/edit?usp=sharing)
[![gGemini Badge](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://gemini.google.com/gem/16PXYJfSoG9dfOJaEcexz4MLqSqY3GlFz?usp=sharing)
![gGemini Badge](https://img.shields.io/badge/Wiki%20js-1976D2?style=for-the-badge&logo=Wikidotjs&logoColor=white)

![by-sa](https://licensebuttons.net/l/by-sa/3.0/88x31.png)

## 🚀 Cómo funciona

Al preguntarle al Agente por un Bakugan (Ej. *"Alpha Hydranoid"*), este procesa el archivo maestro y devuelve instantáneamente una tabla cruzando los G-Powers físicos vs. los datos canónicos del anime, ofreciendo rutas interactivas para expandir el conocimiento del usuario.


Protocolo de Extracción Cruzada de Datos (v1.1.2)!
