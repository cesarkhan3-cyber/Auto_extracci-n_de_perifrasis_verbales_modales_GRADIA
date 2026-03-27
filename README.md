# Auto_extraccion_de_perifrasis_verbales_modales_GRADIA
Este repositorio ofrece un script de python que ayuda a llevar a cabo una extracción automática de 6 perífrasis verbales modales (PPVV) ("deber + INF", "deber de + INF", "tener de + INF", "tener que + INF", "haber que + INF" y "haber de + INF") desde archivos de textos planos (.txt). Se calcula la frecuencia de las perífrasis verbales elegidas con concordancia de dichas PPVV para que se vuelva a revisar los resultados. También ofrece un análisis colostruccional (Collexeme Analysis) con el fin de mostrar la atracción/repulsión entre los verbos infinitivos y las PPVV. Este script todavía está desarrollando, en el futuro apoyará una elección más amplia de otras perífrasis verbales. Está desarrollado por el Equipo GRADIA.

# Requisitos previos
Para que funcione el script, hay que preparar una carpeta que se llama "raw_txt_clean" en el mismo directorio del script. Debería guardar los archivos que se van a procesar en esta carpeta. 

*En teoría también hay que preparar archivo de diccionario (en este script es "hsms.src"). Pero este diccionario no está cargado al repositorio. Así que si no lo tiene, durante el procesamiento aparecerá una alerta sobre la precisión. El "hsms.src" está basado de Freeling. Por eso, si es necesario, también puede compilar un propio y luego cambiar un poquito el contenido del script. 

# Instalar las dependencias de Python
pip install -r requirements.txt
python -m spacy download es_core_news_md

# Manejo y uso
Cualquier herramienta que apoya al entorno de Python. Corre el script:
python auto_extraccion v1.py
Se corre automáticamente todo el procesamiento y al final nos salen 3 archivos de .xslx, son (i) frecuencias de las PPVV con concordancias, (ii) los verbos infinitivos detectados y filtrados del corpus y (iii) resultados del análisis colostruccional.  

