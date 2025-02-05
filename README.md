# Análisis estadistico de señales Biomédicas 
Este laboratorio tiene como objetivo analizar estadisticamente las señales biomédicas, sus estadisticas descriptivas y evaluar la relación señal-ruido (SNR) bajo diferentes tipos de ruido. El código esta implentado en Python y utiliza bibliotecas como `wfdb`, `numpy`,`matplotlib` y `scipy`.

## Tabla de Contenidos 
1.[Introducción](#introducción)
2.[Requisitos](#requisitos)
3.[Uso](#uso)
4.[Explicación del Código](#explicación-del-código)
5.[Resultados y Gráficas](#resultados-y-gráficas)

##Introducción 

Las señales biomédicas son las señales generadas por el cuerpo humano, como lo son los electrocardiogramas (ECG), electroencefalogramas (EEG) y lo que analizaremos en este labpratorio es una señal de electromiografia (EMG). Estas señales contienen información relevante, como amplitud y frecuencia, pero también están contaminadas por ruido, lo que dificulta su análisis. En este laboratorio se realiza lo siguiente: 

1. **Lectura de una señal fisiológica** desde archivos `.dat` y `.hea` que son descargados desde las base de datos como [PhysioNet`](https://physionet.org/).
2. **Cálculo de estadísticas descriptivas**(media,desviación estándar, coeficiente de variación, histograma y función de probabilidad).
3. **Evaluación de la relación señal-ruido (SNR)** Bajo diferentes tipos de ruido (gaussiano,impulso y artefacto).

## Requisitos 

- **Phyton** Instalado en tu sistema 
- **Spyder** (Puedes instalarlo como parte de [Anaconda](https://www.anaconda.com/)).
- **Bibliotecas de Python:** `numpy`,`matplotlib`,`scipy`,`wfdb`
- **Una señal fisiológica en formato `.dat` y `.hea` (Se puede descargala de [Physionet](https://physionet.org/)).

## Descargar una señal fisiologica y Guardar los datos en el código 
1. Entrar a Physionet y descargar una señal en formato .dat y .hea, en este caso de una señal EMG
2. Guardar los archivos descargados en la misma carpeta donde se guardo el archivo del código.
3. Verificar que todas las librerias esten instaldas: Poner en la terminal ejem:!pip install wfdb 

   
## Explicación del Código  

1. **Lectura de la señal**: Se utiliza la biblioteca wfdb para leer la señal fisiológica desde los archivos .dat y .hea
![image](https://github.com/user-attachments/assets/a6ebaa49-53fc-48ba-b1fd-f9ea67d60226)
2.**Cálculos de estadistica**:Se calculan estadísticas descriptivas como la media,desviación estándar y coeficiente de variación.Estas se calculan de dos maneras:Programando las fórmulas desde cero y utilizando funciones predefinidas de python. 
