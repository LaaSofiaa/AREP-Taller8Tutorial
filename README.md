# AREP Taller 8

## Descripción del Proyecto

Este proyecto implementa un modelo que utiliza un sistema de invocación basado en prompts. 
El objetivo principal es procesar entradas y generar respuestas utilizando un modelo preentrenado.
A continuación, se detalla la arquitectura del proyecto, los componentes principales, las instrucciones de instalación y ejemplos de uso.

---

## Arquitectura del Proyecto

El proyecto está compuesto por los siguientes componentes principales:

1. **Modelo de Invocación (`model.invoke`)**:
   - Este componente se encarga de procesar un `prompt` y generar una respuesta basada en el modelo preentrenado.
   - Es el núcleo del sistema y se utiliza para interactuar con el modelo.

2. **Sistema de Entrada y Salida**:
   - Entrada: El usuario proporciona un `prompt` que describe la tarea o pregunta.
   - Salida: El sistema imprime la respuesta generada por el modelo.

3. **Estructura del Código**:
   - El código principal se encuentra en un archivo Jupyter Notebook (`AREP_TALLER8.ipynb`).
   - Utiliza bibliotecas específicas para la interacción con el modelo.

---

## Instrucciones de Instalación

Instalar las dependencias de LangChain y pip

```bash
  pip install langchain
  pip install -qU "langchain[openai]"
```
Configurar la API Key de OpenAI para poder interactuar con el modelo

```bash
  import os
  import getpass

  if not os.environ.get("OPENAI_API_KEY"):
      os.environ["OPENAI_API_KEY"] = getpass.getpass("Introduce tu API Key de OpenAI: ")
```
## Instrucciones de ejecución del código

1. Abrir el archivo AREP_TALLER8.ipynb en Jupyter Notebook o JupyterLab

```bash
  jupyter notebook AREP_TALLER8.ipynb
```
2. Ejecutar las Celdas: Sigue el orden de las celdas para cargar el modelo, configurar los prompts y realizar invocaciones.

3. Ejemplo de Uso: En el archivo AREP_TALLER8.ipynb, encontrarás un ejemplo como este:

```bash
  response = model.invoke(prompt)
  print(response.content)
```
## Evidencias
![image](https://github.com/user-attachments/assets/1e94f159-9fbb-46dc-8407-219e381cb3ae)

![image](https://github.com/user-attachments/assets/4b60ef95-a471-4158-ba05-c3cec80c6c99)

