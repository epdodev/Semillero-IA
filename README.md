# 🚀 Semillero de Inteligencia Artificial

Repositorio oficial para las prácticas y talleres del Semillero de IA.

---

## 📌 Contenido del Repositorio

| Práctica | Nombre del Taller | Descripción | Archivo |
| :--- | :--- | :--- | :--- |
| **Práctica 1** | Introducción a los LLMs | Primeros pasos con modelos de lenguaje y entornos de ejecución. | `practica_1.ipynb` |
| **Práctica 2** | Expedición Lunar: Cartas desde la Luna | Experimentación y control de hiperparámetros de generación con Ollama y `gemma:2b`. | `practica_2.ipynb` |
| **Práctica 3** | Clínica Psiquiátrica IA: Técnicas de Prompt Engineering | Aplicación y comparación de técnicas clave de prompting (Zero-shot, Few-shot, Chain of Thought y Role Prompting) en simulación clínica. | `practica_3.ipynb` |

---

## 🧪 Práctica 2: Expedición Lunar — Cartas desde la Luna con LLMs

Esta práctica tuvo como objetivo evaluar el impacto práctico de los hiperparámetros de generación de texto ejecutando un modelo localmente mediante **Ollama** (`gemma:2b`).

### ⚙️ Hiperparámetros Evaluados

* **`temperature`**: Controla el grado de aleatoriedad o creatividad del modelo. Valores bajos (ej. `0.1`) generan respuestas deterministas y rígidas; valores altos (ej. `0.85`) producen salidas más fluidas, poéticas y descriptivas.
* **`top_p` (Nucleus Sampling)**: Define el umbral probabilístico para la selección de tokens. Un `top_p` reducido (ej. `0.2`) limita severamente el vocabulario a palabras comunes, mientras que valores altos (ej. `0.95`) introducen diversidad léxica.
* **`num_predict`**: Delimita el número máximo de tokens generados, evitando la interrupción prematura o la extensión excesiva de la carta.
* **`repeat_penalty`**: Penaliza la repetición contigua de frases o estructuras oracionales. Un valor elevado (ej. `1.35`) fuerza al modelo a utilizar sinónimos y variar la redacción.

---

## 🧠 Práctica 3: Clínica Psiquiátrica IA — Técnicas de Prompt Engineering

Esta práctica aborda la formulación estratégica de instrucciones para modelos de lenguaje a través de la simulación de casos en una clínica psiquiátrica. Se analiza cómo la estructura y la técnica de prompting determinan la calidad, precisión y profundidad de las respuestas del modelo.

### 🛠️ Técnicas de Prompting Exploradas

* **Zero-Shot**: Se instruye al modelo sin proporcionarle ejemplos previos, evaluando su capacidad intrínseca para reestructurar notas informales y redactar informes clínicos profesionales.
* **Few-Shot**: Se suministran casos de referencia previos (síntomas, diagnóstico y recomendación) para que el modelo aprenda el patrón y estandarice las respuestas siguiendo el formato clínico requerido.
* **Chain of Thought (CoT)**: Se fuerza al modelo a descomponer el razonamiento paso a paso (preguntas clínicas clave, análisis diferencial, evaluación preliminar y próximos pasos) antes de emitir una conclusión diagnóstica.
* **Role Prompting**: Se asignan perfiles profesionales diferenciados (Psicólogo Cognitivo-Conductual, Psiquiatra y Coach de Vida/Oratoria) para evaluar un mismo caso desde diversas perspectivas disciplinares.
* **Combinación de Técnicas & Caso Personalizado**: Integración sinérgica de múltiples técnicas (Role Prompting + Chain of Thought + formato estructurado) para la resolución de casos clínicos complejos y el análisis de adicciones tecnológicas.

---

## 💻 Requisitos del Entorno

* **Python 3.x**
* **Ollama** con los modelos instalados localmente:
  * `gemma:2b` (`ollama pull gemma:2b`)
  * `gemma2:2b` (`ollama pull gemma2:2b`)
* **Librerías de Python**:
  * `ollama`
  * `openai` *(opcional para ejecución en la nube mediante Google Gemini API)*
  * `ipython`
