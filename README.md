## Análisis de Hipermercado ##


Este proyecto pone en práctica habilidades de procesamiento de datos mediante un proceso ETL (Extract, Transform, Load), generando una base de datos que se utiliza para analizar los KPIs en un dashboard desplegado en Power BI.  
El objetivo es proporcionar un material accesible y ágil para utilizar en los briefings y así comprender el comportamiento del negocio e identificar puntos de mejora.  

<img width="1281" height="712" alt="Dashboard" src="https://github.com/user-attachments/assets/d8ac88a9-a368-4d77-bf82-80b9795a84e1" />


📊 Dashboard Interactivo

El dashboard interactivo en Power BI permite explorar diversos aspectos del desempeño del hipermercado.  
A continuación, se destacan algunos de los puntos clave que se pueden analizar:  

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

* El Dashboard cuenta con dos segmentadores para poder analizar en detalle los periodos de tiempo, estos segmentadores nos permiten seleccionar el año y los meses de los cuales disponemos de información en la base de datos.
Pare que estos segmentadores funcionen correctamente despues de transformar los datos, he creado un modelo estrella estableciendo las relaciones con una columna calculada (CodigoPeriodo) que hice utilizando DAX para poder mantener una correcta relación entre las tablas.  
<img width="1150" height="516" alt="modelo" src="https://github.com/user-attachments/assets/9e73459b-f1ea-4ef2-a0d8-dc1bf8a1dff1" />

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


* Contamos con una barra con los KPI's que se actualizaran al utilizar los segmentadores, estos nos aportan información muy importante sobre el negocio como el total de la venta, la productividad, total de la merma, cantidad de tickets y la media de los mismos.
<img width="978" height="192" alt="kpi" src="https://github.com/user-attachments/assets/ae7c5dac-5402-47f2-ae5a-1a3a53b44c37" />

ç-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

+ Los gráficos con los que contamos son los siguientes: 


1. 📈 Ventas por Día

Visualización: Gráfico de líneas que muestra las ventas totales por periodo.

Análisis: Identificar tendencias de ventas, comparar periodos y detectar picos o caídas significativas.

2. 🛒 Porcentaje de ventas por Categoría

Visualización: Muestra la participación que tiene cada categoría sobre la venta total.

Análisis: Determinar qué categorías generan más ingresos y evaluar su rotación.

3. 📉 Mermas por Día

Visualización: Gráfico de líneas que muestra las mermas por periodo.

Análisis: Identificar patrones en las mermas y evaluar su impacto en las ventas.

4. 📉 Merma por Categorías

Visualización: Se ve el porcentaje de cada categoría sobre la merma total.

Análisis: Identificar las categorías con mayor merma para tomar medidas correctivas.

5. 💬 NPS (Net Promoter Score)

Visualización: Indicador que muestra el NPS actual.

Análisis: Evaluar la satisfacción del cliente y su disposición a recomendar el hipermercado.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


🛠️ Tecnologías Utilizadas

Plataforma de análisis y visualización: Power BI

Procesamiento de datos: Transformaciones y limpieza de datos directamente en Power BI (Power Query y DAX)

Control de versiones: Git, GitHub


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


📂 Estructura del Repositorio
├── Análisis Hipermercado.pbix   # Archivo de Power BI con el dashboard
├── Mermas.csv                   # Datos de mermas
├── NPS.csv                      # Datos de NPS
├── Ventas.csv                   # Datos de ventas
└── README.md                    # Este archivo


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
🚀 Cómo Ejecutar el Proyecto

Clona el repositorio:

git clone https://github.com/JaviDoria/Analisis-Hipermercado.git


Abre el archivo Análisis Hipermercado.pbix en Power BI.

Carga los archivos CSV (Ventas.csv, Mermas.csv, NPS.csv) en Power BI.

Explora el dashboard interactivo para analizar los KPIs.

* Este proceso requiere la transformación de los CSV ya que todo está ejecutado directamente en el Power BI.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
📌 Objetivos del Proyecto

Aplicar técnicas de procesamiento de datos para la creación de un dashboard interactivo.

Proporcionar una herramienta visual para el análisis del desempeño del hipermercado.

Identificar áreas de mejora basadas en datos concretos.
