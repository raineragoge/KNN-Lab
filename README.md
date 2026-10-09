# KNN Lab 4.0 — Laboratorio interactivo de Machine Learning

**Proyecto educativo en HTML, CSS y JavaScript para comprender el algoritmo K-Nearest Neighbors (KNN) de forma visual e interactiva.**

En lugar de limitarse a una definición teórica, la página permite **modificar ejemplos, elegir K, consultar vecinos, mover puntos y comprobar el resultado inmediatamente**. Incluye una situación cotidiana con datos simulados: la elección entre **bicicleta y autobús** según la distancia y la probabilidad de lluvia.

## 🚀 Cómo ejecutarlo

1. Descarga o clona este repositorio.
2. Abre **[`index.html`](index.html)** con tu navegador (Chrome, Firefox, Edge, etc.).
3. No tienes que instalar paquetes, servidor, compiladores ni bibliotecas externas.

```bash
git clone https://github.com/raineragoge/KNN-Lab.git
cd KNN-Lab
```

## 🎯 ¿Qué se aprende?

**KNN** es un algoritmo de aprendizaje supervisado. Para clasificar un dato desconocido:

1. Parte de ejemplos que ya tienen una clase asignada.
2. Calcula la distancia del dato nuevo a esos ejemplos.
3. Escoge los **K ejemplos más cercanos**.
4. Predice la clase más frecuente entre esos vecinos.

La interfaz muestra la predicción y cómo votan los vecinos, para entender el efecto de cambiar los datos, el valor de K y la forma de medir la distancia.

## 🧪 Funciones de la versión 4.0

| Función | Qué puedes hacer |
|---|---|
| **Laboratorio de clasificación** | Ver clases A/B en un plano con características X e Y. |
| **Control de K** | Probar valores impares de K entre 1 y 19 en el laboratorio genérico. |
| **Distancia** | Alternar entre distancia euclídea y Manhattan. |
| **Fronteras de decisión** | Mostrar u ocultar las zonas que KNN clasificaría como A o B. |
| **Datos editables** | Elegir el número de puntos conocidos A y B. |
| **Puntos aleatorios** | Seleccionar la cantidad de nuevos puntos y si serán A, B o una mezcla. |
| **Clic y arrastre** | Colocar, desplazar y editar puntos visualmente, también desde dispositivos táctiles. |
| **Predicciones fijadas** | Hacer clic en una zona libre para clasificarla y dejar marcado el punto; las predicciones **no pasan automáticamente a ser datos de entrenamiento**. |
| **Explicación paso a paso** | Inspeccionar las fases de cálculo de distancias, selección de vecinos y votación. |
| **Modo desafío** | Adivinar qué clase elegirá KNN; consultar aciertos, rondas y rachas. |
| **Ejemplo de la vida real** | Simular si alguien elegiría bicicleta o autobús con distancia y probabilidad de lluvia. |
| **Música instrumental** | Reproducir y pausar una melodía sintetizada de estilo clásico y regular el volumen (sin reproducción automática). |
| **Historial de prompts** | Consultar dentro de la web las peticiones originales y sus versiones mejor redactadas. |

> **Importante:** el ejemplo de bicicleta/autobús trabaja con datos **ficticios**; la predicción estima qué eligieron ejemplos similares, no determina cuál es el medio de transporte objetivamente mejor. Las variables se normalizan antes de calcular la distancia.

## 📱 Vista en móvil

La interfaz se adapta a pantallas pequeñas y permite interactuar con los puntos mediante controles táctiles.

## 🛠️ Evolución del proyecto

| Versión | Mejoras realizadas |
|---|---|
| **v1 — Idea inicial** | Explicación general de KNN, laboratorio visual, predicción por vecinos y ejemplo cotidiano de movilidad. Historial de peticiones. |
| **v2 — Más interactividad** | Fronteras de decisión, modo desafío y comparación de K = 1, 5 y 15. Historial ampliado. |
| **v3 — Claridad visual** | Paneles más compactos, fases de clasificación explicadas y cabeceras de tablas más claras. |
| **v4 — Interfaz y edición** | Eliminación de la sección independiente de comparación de K, reducción de espacios vacíos, recuento A/B editable, generación aleatoria configurable, puntos arrastrables, predicciones permanentes, música instrumental y prompt unificado. |

**Decisión de diseño:** la comparación de tres mapas de K presente en v2 se retiró expresamente en v4. Sigue siendo posible comparar distintos valores de K cambiándolos en el laboratorio y en el ejemplo práctico.

## 💬 Prompts utilizados durante la creación

El proyecto se desarrolló iterativamente con ayuda de ChatGPT. Los siguientes prompts son **versiones mejor redactadas** de las solicitudes efectuadas; su formulación original se conserva en [PROMPTS.md](PROMPTS.md) y también puede consultarse en el historial incluido en `index.html`.

### PROMPT 01 — Idea inicial

> Crea una página HTML interactiva para explicar y visualizar cómo funciona el algoritmo KNN (k vecinos más cercanos). Haz que se pueda experimentar con los datos de forma intuitiva e interesante.

### PROMPT 02 — Estructura

> Organiza la página en dos partes: primero, una explicación general y sencilla de KNN; después, un caso práctico que muestre cómo se aplica a una situación de la vida real.

### PROMPT 03 — Petición unificada

> Desarrolla una página HTML educativa e interactiva sobre KNN. Comienza con una explicación de sus fundamentos y continúa con una simulación aplicada a un problema real.

### PROMPT 04 — Transparencia

> Incluye dentro de la propia página un apartado donde aparezcan los prompts utilizados durante su creación, para que el proceso de desarrollo quede documentado.

### PROMPT 05 — Propuestas de mejora

> Propón mejoras que hagan KNN Lab más visual, interactivo y útil para aprender, manteniendo la explicación y el ejemplo práctico existentes.

### PROMPT 06 — Nuevas funciones

> Actualiza KNN Lab con cuatro funciones: visualización de fronteras de decisión, modo desafío para adivinar predicciones, comparación simultánea de distintos valores de K y un historial ampliado de prompts. Conserva todas las funciones anteriores y el ejemplo de movilidad.

### PROMPT 07 — Rediseño de resultados

> Mejora la presentación de los paneles «Resultado de KNN» y «Modo desafío». Reduce los espacios vacíos, agrupa mejor la información, explica qué hace cada fase del algoritmo e identifica las columnas de las tablas de vecinos: número, clase, posición y distancia. Mantén todas las interacciones y añade esta solicitud al historial con una redacción clara, sin perder el mensaje original.

### PROMPT 08 — Últimas peticiones unificadas

> Actualiza KNN Lab con un diseño más compacto y sin grandes espacios vacíos, especialmente bajo los gráficos del laboratorio y del ejemplo de transporte. Elimina la sección independiente de comparación de K (los tres mapas simultáneos), pero conserva el resto de funciones: explicación, KNN paso a paso, fronteras de decisión, desafío y ejemplo real de bicicleta/autobús. Añade controles para ajustar por separado el número de puntos conocidos de las clases A y B y un generador de puntos aleatorios cuya cantidad y clase se puedan elegir. Permite arrastrar y reposicionar los puntos existentes. Al pulsar en una zona libre, clasifica esa posición y deja una marca permanente con el color de la clase predicha; diferencia esas predicciones de los datos de entrenamiento. Incorpora música instrumental de estilo clásico con botones para reproducir/pausar y controlar el volumen, sin reproducción automática. Finalmente, agrupa estas últimas solicitudes en un único prompt, redáctalo con claridad e inclúyelo en el historial de la propia página. Asegúrate de que el diseño sea cómodo también en móvil y de que todo siga funcionando sin conexión.

## 📂 Estructura del repositorio

```text
KNN-Lab/
├── index.html                 # Página completa: HTML + CSS + JavaScript
├── README.md                  # Documentación y resumen de prompts
└── PROMPTS.md                 # Historial de mensajes originales y mejorados
```

## 🌍 Publicar la página con GitHub Pages

Cuando los archivos estén subidos:

1. Entra en el repositorio de GitHub.
2. Abre **Settings → Pages**.
3. En **Build and deployment**, elige **Deploy from a branch**.
4. Selecciona `main` y la carpeta `/ (root)`; pulsa **Save**.
5. Espera a que GitHub muestre la URL publicada en la sección Pages.

La URL habitual, **si el repositorio se llama `KNN-Lab`**, sería `https://raineragoge.github.io/KNN-Lab/`, pero **no debe considerarse activa hasta que GitHub Pages confirme su publicación**.

## 🧰 Tecnologías

- **HTML5** para estructura y accesibilidad.
- **CSS3** para estilos, diseño responsive e interfaz compacta.
- **JavaScript** para KNN, visualización, interacciones y sonido sintetizado.
- **SVG y Canvas** para gráficos y fronteras de decisión.

No depende de servicios externos y puede ejecutarse sin conexión.

---

Proyecto educativo creado para experimentar con KNN y documentar el proceso iterativo de diseño con IA. **Versión documentada: 4.0 (9 de octubre de 2026).**