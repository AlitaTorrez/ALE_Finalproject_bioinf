Final project Alejandra Torrez
1. Introduction
1.1 My database
My proyecto abarca el analisis de secuencias de muestras clínicas (heces) principalmente positivas para Rotavirus o RVA (hay muy pocas para otros patógenos ya que el objetivo era caracterizar las cepas de RVA). A partir de un set de aproximadamente 300 muestras diarreicas de niños menores a 5 años recolectadas durante el 2023, se extrajo el TNA con un protocolo homemade. El TNA de las muestras posteriormente fue analizado por qPCR para diferentes patógenos entéricos virales y bacterianos. Se seleccionó un set de extractos positivos para RVA y algunos otros patógenos para realizar la preparación de librerías a partir de RNA. Las librerías individuales se unieron en diferentes pooles y fueron cargadas en diferentes ocasiones en cartuchos de una plataforma de Illumina (iSeq100). Las corridas fueron almacenadas en Base Space y luego cargadas a CZ-ID (una plataforma gratuita que ya incluye un pipeline para analizar datos metagenómicos) donde gracias al pipeline se pueden ver directamente los reads y contigs asignados a diferentes patógenos.

En un análisis previo las secuencias de RVA obtenidas del CZ-ID fueron utilizadas para caracterizar el genoma de diferentes cepas circulantes. Sin embargo, solo se evaluó RVA y no los demás patógenos. Aunque la mayor parte de las muestras seleccionadas corresponden a RVA, hay algunas que corresponden a otros patógenos.

Por esta razón el objetivo general es:

Analizar los datos metagenómicos de las muestras diarrecias secuenciadas y comparar con los resultados de qPCR.
Y los objetivos específicos son:

Realizar el QC de algunas muestras secuenciadas, evaluar la calidad y realizar el filtrado de ser necesario. Con esto obtener un gráfico de la diversidad de patógenos y comparar con los gráficos obtenidos en el CZ-ID (esto con fines solo de comparacion).
Obtener gráficas de reads totales para virus, bacterias y cada uno de los patógenos detectados usando librerías de Python.
(Si da tiempo) Comparar las gráficas obtenidas en Python y CZ-ID para comparar con los datos de qPCR (tanto a nivel general como por muestra).


Clona este repositorio:

git clone https://github.com/AlitaTorrez/ALE_Finalproject_bioinf.git

cd ALE_Finalproject_bioinf

Crea y activa el entorno conda:

conda env create -f ale_env_bioinfo.yml -n ale_env_bioinfo

conda activate ale_env_bioinfo
