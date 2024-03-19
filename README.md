# Detector de malezas en monocultivos

## Descripción

Las malezas son un gran problema en la agricultura, generan pérdidas económicas y desequilibrios ambientales.
Para resolverlo, necesitamos nuevas tecnologías que reduzcan el uso de herbicidas y maximicen la producción. 
Aunque existen sistemas automatizados para controlar las malezas, aún tienen dificultades para reconocerlas en diferentes condiciones. 
Es crucial mejorar la capacidad de reconocimiento y desarrollar bases de datos específicas para entrenar modelos de IA que funcionen bien en cualquier situación de campo.<br><br>
Queremos crear un sistema de detección de malezas que identifique y clasifique las plantas entre maleza y cultivo para realizar un control selectivo. 
Este sistema ayudará a los agricultores a gestionar sus cultivos de manera eficiente y sostenible. 
Podrá implementarse en maquinaria agrícola, drones o robots para realizar un control selectivo utilizando herbicidas, vapor de agua o láser


<div><img src='images\imagenReadme.jpg' border=5px solid red height=300 caption="Detecciones de malezas y cultivos mediante el uso del modelo Yolo-V4" ></div>

## Funcionalidades

Clasificación y detección de malezas y cultivo en imágenes provistas por el usuario a traves de la app.

## Demo
Link a la aplicación [WeedCropDetector](https://weedcropdetector.streamlit.app/)

## Fuente de datos

Imágenes de cultivos de [Crop/Weed](https://drive.google.com/drive/folders/1zpyWs7rDUHFCtOCNAvH5RueEvUVxL6OZ?usp=sharing)

## Notebooks

Este repositorio contiene un conjunto de notebooks de Jupyter, que describen los pasos necesarios:

1. [EDA](notebooks/EDA.ipynb): Se realiza una analisis exploratorio de las imágenes para comprender mejor el set de datos.
2. [Entrenamiento- Validacion -Test ](notebooks/Weed_crop_60epoc.ipynb): Entrenamiento y evaluación del modelo.


## Autores
- [@sasalyamila](https://github.com/yamilasasal)
- [@miguebalderrama](https://github.com/miguebalderrama)
## :page_facing_up: Licencia

El código está licenciado bajo Apache 2.0. Refiérase a [LICENSE.txt](LICENSE.txt).
