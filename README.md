# 🚀 Semillero de Inteligencia Artificial

Repositorio oficial para las prácticas y talleres del Semillero de IA.

---

## 📌 Contenido del Repositorio

| Práctica | Nombre del Taller | Descripción | Archivo |
| :--- | :--- | :--- | :--- |
| **Práctica 1** | Introducción a los LLMs | Primeros pasos con modelos de lenguaje y entornos de ejecución. | `practica_1.ipynb` |
| **Práctica 2** | Expedición Lunar: Cartas desde la Luna | Experimentación y control de hiperparámetros de generación con Ollama y `gemma:2b`. | `practica_2.ipynb` |

---

## 🧪 Práctica 2: Expedición Lunar — Cartas desde la Luna con LLMs

Esta práctica tuvo como objetivo evaluar el impacto práctico de los hiperparámetros de generación de texto ejecutando un modelo localmente mediante **Ollama** (`gemma:2b`).

### ⚙️ Hiperparámetros Evaluados

* **`temperature`**: Controla el grado de aleatoriedad o creatividad del modelo. Valores bajos (ej. `0.1`) generan respuestas deterministas y rígidas; valores altos (ej. `0.85`) producen salidas más fluidas, poéticas y descriptivas.
* **`top_p` (Nucleus Sampling)**: Define el umbral probabilístico para la selección de tokens. Un `top_p` reducido (ej. `0.2`) limita severamente el vocabulario a palabras comunes, mientras que valores altos (ej. `0.95`) introducen diversidad léxica.
* **`num_predict`**: Delimita el número máximo de tokens generados, evitando la interrupción prematura o la extensión excesiva de la carta.
* **`repeat_penalty`**: Penaliza la repetición contigua de frases o estructuras oracionales. Un valor elevado (ej. `1.35`) fuerza al modelo a utilizar sinónimos y variar la redacción.

---

## 💻 Requisitos del Entorno

* **Python 3.x**
* **Ollama** con el modelo `gemma:2b` instalado localmente (`ollama pull gemma:2b`)
* Librerías de Python: `ollama`
