# Detector de malezas en monocultivos (Soja/Maíz)

## Descripción

En la Argentina, el problema de las malezas crece de manera sostenida y acelerada favorecido por el uso rutinario y repetido de las mismas herramientas de control, que consisten en uno o unos pocos herbicidas como única y exclusiva herramienta. Al competir por el agua y los nutrientes del suelo, las malezas generan pérdidas económicas e interfieren durante la cosecha. En este proyecto buscamos crear un detector de malezas que permita al productor tomar decisiones que se ajusten a la realidad del cultivo, que permitan la detección de focos y minimicen las consecuencias negativas de las malezas. Además, esto reduciría el número de aplicaciones de fitosanitarios (tales como insecticidas, bactericidas, fungicidas y plaguicidas). Esta herramienta permitirá el monitoreo de lotes de forma remota y la toma de decisiones conociendo la distribución de malezas en su cultivo (cantidad y distribución espacial)
<div><img src="https://mundoagro.cl/wp-content/uploads/2024/01/3.jpg" border="5px solid red" height="300" caption="Detecciones de malezas y cultivos mediante el uso del modelo Yolo-V4" ><img src="https://avgust.com.co/wp-content/uploads/2020/02/dji-4204801_1280-1080x675.jpg" border="5px solid red" height="300" caption="Detecciones de malezas y cultivos mediante el uso del modelo Yolo-V4" ></div>






## Requerimientos

Se utilizan las herramientas **GDAL** y [Orfeo Toolbox](https://www.orfeo-toolbox.org/) en la primera etapa del pre-procesamiento de los datos. Luego, se emplean nuestros paquetes [satproc](https://github.com/dymaxionlabs/satproc) y [unetseg](https://github.com/dymaxionlabs/satproc) para la generación del dataset y modelo de ML respectivamente.

## Notebooks

Este repositorio contiene un conjunto de notebooks de Jupyter, que describen los pasos necesarios:

1. [Pre-procesamiento](notebooks/1_Preprocesamiento.ipynb): Se procesan las imágenes satelitales y la verdad de campo para generar el dataset de entrenamiento y de predicción del modelo.
2. [Entrenamiento](notebooks/2_Entrenamiento.ipynb): Entrenamiento y evaluación del modelo.
3. [Predicción](notebooks/3_Prediccion.ipynb): Predicción sobre la región de interés.
4. [Post Procesamiento](notebooks/4_Post-procesamiento.ipynb): Procesamiento de los resultados de la predicción.

## :handshake: Contribuciones

Reportes de bugs y *pull requests* pueden ser reportados en la [página de issues](https://github.com/dymaxionlabs/basurales) de este repositorio. Este proyecto está destinado a ser un espacio seguro y acogedor para la colaboración, y se espera que los contribuyentes se adhieran al código de conducta [Contributor
Covenant](http://contributor-covenant.org).

## :page_facing_up: Licencia

El código está licenciado bajo Apache 2.0. Refiérase a [LICENSE.txt](LICENSE.txt).
