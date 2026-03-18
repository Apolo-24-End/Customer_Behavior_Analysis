Análisis de Comportamiento de Compra del Cliente 🛒📊
Descripción del Proyecto
Este proyecto realiza un análisis end-to-end (E2E) sobre el comportamiento de compra de 3,900 clientes. El objetivo fue transformar datos brutos en información accionable para identificar patrones de consumo, segmentar clientes y evaluar la efectividad de los programas de suscripción y descuentos.

Tecnologías Utilizadas
Python: Limpieza de datos y feature engineering (Pandas, Numpy).

SQL Server: Almacenamiento de datos y consultas analíticas complejas.

Power BI: Creación de dashboard interactivo y visualización de KPIs.

Pipeline del Proyecto
1. Extracción y Preprocesamiento (Python) 🐍
Se trabajó con un dataset de 3,900 filas y 18 columnas (customer_shopping_behavior.csv). Las acciones principales fueron:

Tratamiento de Nulos: Se imputaron 37 valores ausentes en review_rating utilizando la media agrupada por categoría para mantener la consistencia estadística.

Feature Engineering: * Creación de age_group: Segmentación en 'Young Adult', 'Adult', 'Middle aged' y 'Senior'.

Creación de frequency_of_purchases: Derivada de los días entre compras.

Optimización de Columnas: Eliminación de promo_code_sed tras validar una correlación del 100% con discount_applied (evitando redundancia).

2. Análisis de Datos (SQL Server) 🗄️
Tras cargar los datos limpios en SQL Server, se realizaron consultas para extraer los siguientes hallazgos clave:

Género y Ganancias: Los hombres generaron ganancias de 157,890, mientras que las mujeres 75,191.

Clientes VIP: 839 clientes gastan por encima del promedio y poseen suscripción activa.

Ranking de Productos: Identificación del Top 5 de productos con mejor calificación (reviews).

Impacto de Suscripción: Aunque los suscriptores gastan lo mismo en promedio que los no suscritos, el grupo de no suscritos genera 100,000 más en ganancias totales debido al volumen de población.

Estrategia de Descuentos: Top 5 de productos más vendidos bajo promociones.

Fidelización: Segmentación de clientes (Nuevos, Recurrentes, Leales). Se identificaron 3,116 clientes leales.

Categorización: Ranking de productos estrella por cada categoría.

Retención: Se encontró que la mayoría de los clientes que repiten compra (2,518) no están suscritos, lo que representa una oportunidad de conversión.

3. Visualización y Reporte (Power BI) 📈
Se conectó SQL Server con Power BI para diseñar un dashboard dinámico que incluye:

KPIs Principales: Ganancia promedio por compra, Rating promedio, Total de clientes y Clientes suscritos.

Análisis Financiero: Utilidad y ventas desglosadas por categoría de producto.

Análisis Demográfico: Ventas y utilidad distribuidas por grupo de edad (age_group).

Conclusiones
El análisis sugiere que existe una base sólida de clientes leales que aún no se han convertido al modelo de suscripción. Además, la diferencia de ingresos por género indica que hay espacio para optimizar las campañas de marketing dirigidas al segmento femenino para equilibrar la balanza de ingresos.
