# Proyecto-final-GDGC
## Entrega de proyecto final de la materia gestion de datos geocientificos, presentado por Erluan Zabaleta, Ezequiel Ferro y Diego Navarro.
Este proyecto integra conocimientos de ArcGis, programacion en Python y indicios de gestion de riesgo de desastres geolgicos.

**Objetivo:** El objetivo es crear una herramienta SIG en ArcGis para la identificacion automatica de cuencas torrenciales usando un modelo de elevacion de la zona de interes.

**¿Por que es necesario?:** El primer problema es la delimitacion automatica de cuencas, muchas veces no se tienen delimitadas estas en informacion secundaria y su delimitacion si el area de trabajo es muy grande suele ser tedioso y demora, con este programa se realiza de manera automatica, por otro lado definir la torrencialidad de manera remota sirve como un filtro para el estudio de avenidas torrenciales (fenomeno geologico de alta capacidad destructiva en las zonas montañosas del pais) para su posterior estudio de campo e hidrogeologico. 

**¿Que variables y programas se usaron?** Como variables se tiene que el unico insumo necesario es un modelo de elevacion de cualquier escala y area o si es querido se puede agregar los puntos de interseccion de las cuencas de interes particular. Los programas utilizados fueron ArcMap para la visualizacion y tratamiento de datos geoespaciales asi como la utilizacion de herramientas de analisis espacial, para el analisis de base de datos generadas en ArcMap se utilizo Python con el programa Jupyter Notebook.

**¿Como se hizo?:** Se utilizaron una serie de herramientas de analisis espacial en el software ArcMap, como resultado se genera un shp con todas las cuencas delimitadas segun unos ordenes de jerarquia definidos, posterior este shp y DEM se utilizan para el calculo de parametros morfometricos 50 en total, estos parametros tienen diferentes usos pero para este caso usaremos aquellos que definen la torrencialidad de la cuenca, este codigo genera un csv que puede ser utilizado para hacer join con el shp y darle la caracteristica de torrencialidad a cada cuenca calculada, esto se hace gracias a un parametro en comun, el GRIDCODE. 

Para su mejor visualizacion todo el contenido se encuentra en el siguiente link de Drive: https://drive.google.com/drive/folders/1rLoFFI6YFiJPWLGtxV7LU6gl_aFdfQd1?usp=drive_link 

![Logo](LOGO.png)
