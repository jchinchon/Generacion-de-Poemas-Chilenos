# Generación de Poemas Chilenos con SP-GPT2

¡Bienvenido al proyecto de Generación de Poemas Chilenos! Aquí utilizamos SP-GPT2 (Poema Semántico GPT-2) para generar poesía tradicional chilena. Este proyecto se basa en GPT-2, un potente modelo generativo desarrollado por OpenAI.

## Resumen

El objetivo de este proyecto es explorar las capacidades de SP-GPT2 en la generación de poesía que capture la esencia y estructura de los poemas chilenos tradicionales. El modelo se mejora mediante la incorporación de una función de pérdida personalizada, y su rendimiento se evalúa en un conjunto de datos que incluye poemas de poetas reconocidos como Gabriela Mistral y Pablo Neruda.

## Instrucciones de Uso:

**Nota:** Puedes acceder y ejecutar el notebook de Google Colab asociado a este proyecto aquí [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Vv6yyFw7e_mImcadHitl3oscesPK8F4u?usp=sharing)

1. **Instalación y Configuración:**
   - Ejecutar las secciones 1 a 3 para instalar los requisitos, importar las bibliotecas necesarias y crear funciones relativas a la arquitectura LSTM.

2. **Carga del Dataset:**
   - En la sección 4, por defecto, se importa el dataset con todos los poemas. Sin embargo, puedes cambiarlo para utilizar solo poemas de Pablo Neruda o Gabriela Mistral, archivos que se encuentran en la carpeta `Datasets/`.

3. **Elección del Tokenizador:**
   - En la sección 5, elige el tokenizador que prefieras. Se recomienda sólo la ejecución de la sección 5.2 para utilizar el tokenizador pre-entrenado. En caso de optar por Tiktoken, sólo ejecuta la sección 5.1.

4. **Funciones de Entrenamiento y Evaluación:**
   - Ejecuta la sección 6, que contiene la creación de funciones relacionadas con el entrenamiento, la evaluación del modelo, y el score de creatividad.

4. **Selección y Entrenamiento del Modelo:**
   - Para elegir el modelo que deseas entrenar, ejecuta la sección correspondiente:
      - **Opción A:** Para entrenar un modelo SP-GPT2 pequeño desde cero (sin pre-entrenamiento), ejecuta la sección 7.A.
      - **Opción B:** Si prefieres realizar fine-tuning en el modelo SP-(GPT2 pre-entrenado para español), disponible en Hugging Face [aquí](https://huggingface.co/DeepESP/gpt2-spanish), ejecuta la sección 7.B (se recomienda esta opción).
      - **Opción C:** Para examinar únicamente el modelo GPT2 clásico pre-entrenado, ejecuta la sección 7.C.


6. **Generación de Poemas:**
   - Para modificar los parámetros de generación de poemas, consulta las subsecciones "Generación de Poemas" dentro de cada sección 7.

Siguiendo estos pasos, podrás configurar, entrenar y generar poemas con el modelo según tus preferencias.

## Estructura del Proyecto

- `Datasets/`: Contiene el conjunto de datos de poemas chilenos.
- `Notebooks/`: Cuaderno Google Colab para el entrenamiento del modelo y generación.
- `Resultados/`: Contiene el conjunto de poemas generados del modelo.

## Reconocimientos

Este proyecto utiliza el modelo SP-GPT2, inspirado en el trabajo presentado en el artículo [T. Nguyen and P. Nguyen](https://doi.org/10.48550/arXiv.2110.15723) - *SP-GPT2: Semantics improvement in vietnamese poetry generation*, 2021.; y en el trabajo base realizado en los laboratorios del curso Modelos Generativos Avanzados, por Camilo Carvajal y Cristóbal Alcázar.

## Contribuciones

¡Se aceptan contribuciones a este proyecto! Si encuentras problemas o tienes ideas para mejorar, no dudes en abrir un problema o enviar una solicitud de extracción.

## Licencia

Este proyecto está bajo la [Licencia MIT](LICENSE).


