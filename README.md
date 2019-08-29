# mod-deep-learning

El objetivo de esta práctica es obtener un modelos de subtitular imagenes. Para ello se diseña un modelo encoder-decoder y se entrena. A partir de un modelo básico, se van realizando distintas modificaciones en el mismo para ver como afectan los distintos cambios en el modelo.

Cuando se encuentra un modelo 'aceptable' se entrena la red con más datos y más iteraciones.

La practica está realizada en un cuaderno de Google Colab ([enlace](https://colab.research.google.com/drive/1aVOG3RO36p1Crynzv4yUncDd2M4SlZEk))

Además, se incluye en el repositorio distintos archivos que se generan durante la ejecución del cuaderno:

| Archivo | Descripción |
| --- | ---|
| `Practica_Mod_Deep_Learning_Final.ipynb` | Copia del cuaderno |
| `README.md` | Este archivo |
| `demo_image.jpg` | Ejemplo de imagen de entrada |
| `demo_image.desc.txt` | Ejemplo de descripción de la imagen |
| `descriptions.txt` | Archivo con todas las descripciones extraídas de todas las imagenes|
| `baseline1.csv` | Resultados del modelo base |
| `size_sm_fixed_vec_model.csv` | Resultados de disminuir el tamaño de la red de entrada al LSTM decodificador |
| `size_lg_fixed_vec_model.csv` | Resultados de aumentar ek tamaño de la red de entrada al LSTM del decodificador |
| `size_sm_seq_model.csv` | Resultados de disminuir la memoria del LSTM del secuenciador |
| `size_lg_seq_model.csv` | Resultados de aumentar la memoria al LSTM del secuenciador |
| `size_em_seq_model.csv` | Resultados de cambiar la capacidad de vocabulario del secuenciador |
| `size_sm_lang_model.csv` | Resultados de disminuir la memoria del modelo de lenguaje |
| `size_lg_lang_model.csv` | Resultados de aumentar la memoria en el modelo de lenguaje |
| `fe_avg_pool.csv` | Resultados de cambiar el metodo de pooling del extractor de características |
| `fe_flat.csv` | Resultados de eliminar el metodo de pooling del extractor de características |
| `final_result.csv` | Resultados finales. Un sólo entrenamiento con más épocas y más datos |
| `train-test-val-set.txt`| Lista con las mil imagenes que usamos para entrenar el modelo  |
| `models-sumamry.csv` | CSV con las medias de todos los experimentos realizados agrupados |
| `models-results.csv` | CSV con todos los experimentos realizados|
| `features.pkl` | Archivo con todas las características extraídas de las imagenes. *(Como el archivo es de 2.97G, no se incluye en el repositorio. **Para obtenerlo hay que ejecutar hasta la sección Modelo - Extracción de características**)* |
