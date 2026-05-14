# 🐲 Bakugan Data Expert 🐉 - 🧾eConsulting: Gs & More

Un agente de IA personalizado (Gem) impulsado por el modelo de Gemini, diseñado específicamente para actuar como la enciclopedia técnica y definitiva de la franquicia Bakugan. 

Este proyecto nació de la necesidad de extraer, limpiar y estructurar miles de datos dispersos sobre el poder G (G-Power) del juego físico y el anime, convirtiéndolos en una base de conocimiento consultable mediante lenguaje natural.

[![Google Badge](https://img.shields.io/badge/Google-Gems-blue?style=flat&logo=google)](https://gemini.google.com/gem/16PXYJfSoG9dfOJaEcexz4MLqSqY3GlFz?usp=sharing)

## ✨ Características Principales (Features)

* **Extracción Precisa de G-Power:** Proporciona tablas detalladas de poder separadas por Atributos (Pyrus, Aquos, Subterra, Haos, Darkus, Ventus, Clear), incluyendo ediciones especiales exclusivas (Translucent, Japan releases, BakuEvolutions).
* **Fidelidad de Datos (Cero Alucinaciones):** El agente está programado bajo una estricta directiva de consultar primero la base de datos local (Extraída vía Web Scraping de la Bakugan Wiki). Si un dato no existe, el bot informa al usuario con total transparencia y realiza un _fallback_ automático buscando en la web.
* **Integración de Battle Gears & Evoluciones:** Identifica y vincula automáticamente los Battle Gears, BakuNanos y Mechtogans asociados a cada Bakugan.
* **Diseño UI/UX para Móviles:** Las variaciones y evoluciones de los Bakugan se renderizan utilizando etiquetas `<u>` de HTML, lo que facilita aislar el texto para "Copiar y Pegar" rápidamente desde dispositivos móviles.
* **Agente Interactivo:** No solo entrega datos, sino que guía la conversación. El bot pregunta proactivamente si el usuario desea desglosar el poder de los Battle Gears por tratamientos de metal (Gold, Silver, Copper) o si requiere la extracción directa del *Thumbnail* (imagen principal) desde la Wiki.

## 🛠️ Stack & Herramientas

* **Python & Pandas:** Limpieza y estructuración del archivo maestro en formato `.xlsx` separado por temporadas (S1 a S4).
* **BeautifulSoup & Requests (Web Scraping):** Automatización de extracción de Infoboxes desde Fandom/Wikia.
* **Google Gemini (Gems):** Motor de Procesamiento de Lenguaje Natural y razonamiento lógico para cruzar los datos.

## 🚀 Cómo funciona

Al preguntarle al Agente por un Bakugan (Ej. *"Alpha Hydranoid"*), este procesa el archivo maestro y devuelve instantáneamente una tabla cruzando los G-Powers físicos vs. los datos canónicos del anime, ofreciendo rutas interactivas para expandir el conocimiento del usuario.
