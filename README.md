# Análisis estadistico de señales Biomédicas 
Este laboratorio tiene como objetivo analizar estadisticamente las señales biomédicas, sus estadisticas descriptivas y evaluar la relación señal-ruido (SNR) bajo diferentes tipos de ruido. El código esta implentado en Python y utiliza bibliotecas como `wfdb`, `numpy`,`matplotlib` y `scipy`.

## Tabla de Contenidos 
1.[Introducción](#introducción)
2.[Requisitos](#requisitos)
3.[Uso](#uso)
4.[Explicación del Código](#explicación-del-código)
5.[Resultados y Gráficas](#resultados-y-gráficas)

## Introducción 

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

### 1. **Lectura de la señal**: Se utiliza la biblioteca wfdb para leer la señal fisiológica desde los archivos .dat y .hea
![image](https://github.com/user-attachments/assets/a6ebaa49-53fc-48ba-b1fd-f9ea67d60226)
### 2.**Cálculos de estadistica**:Se calculan estadísticas descriptivas como la media,desviación estándar y coeficiente de variación.Estas se calculan de dos maneras:Programando las fórmulas desde cero y utilizando funciones predefinidas de python.
![image](https://github.com/user-attachments/assets/b68de891-4309-46ec-a174-4868bfe7f217)
### 3.**Visualización de la señal**: La señal se grafica en el dominio del tiempo para su inspección visual.
![image](https://github.com/user-attachments/assets/b1c01518-2b65-49e8-b334-3fd0a559c2a2)
4.**Histograma y Función de Probabilidad** : Se grafica un Histograma de señal junto con su función de Probabilidad.
5.**Calculo de SNR por potencia y por forma estadistica**: se añade diferentes tipos de ruido ( gaussiano,impulso y artefacto) a la señal y se calcula el SNR para cada caso.
## Resultados y Gráficas
### 1. Señal Original 
![image](https://github.com/user-attachments/assets/84311f68-7927-4cf1-a1c1-b36373a3caac)
## *Figura 1: Representación de la señal en el dominio del tiempo.*
### 2. Histograma y Función de probabilidad desde cero y predefinida.
![image](https://github.com/user-attachments/assets/2ca58720-5063-41b6-9135-99094ab103c0)
## *Figura 2: Histograma y Función de probabilidad.*
### 3. Señal con Ruido Gaussioano
![image](https://github.com/user-attachments/assets/973746dd-5009-4ae3-9935-1d7cc58f56f3)
## *Figura 3: Señal del Ruido Gaussiano.*
### 4. Señal con Ruido de impulso
![image](https://github.com/user-attachments/assets/58cedf77-3965-448c-9a4d-b41e8d36dff2)
## *Figura 4: Señal con ruido de impulso.*
### 5. Señal con ruido de artefacto
![image](https://github.com/user-attachments/assets/0b2a7d67-163c-4e77-b8e4-be06733b02f5)
## *Figura 5: Señal de Ruido de artefacto.*
### 6. Calculos estadisticos
![image](https://github.com/user-attachments/assets/a66b0eef-3b9e-4428-b55e-387434106013)
## *Figura 6: Calculos estadisticos.*
### 7.Calculos de SNR
![image](https://github.com/user-attachments/assets/bdb2fbd4-d642-43cb-9b18-9d9900204696)
## *Figura 7: Calculos SNR.*






