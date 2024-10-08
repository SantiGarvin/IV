# Incertidumbre en la Toma de Decisiones de Venta de Aceitunas

## Contexto

Mis padres son agricultores dedicados al cultivo de olivos en Jaén. Cada año, enfrentan el desafío de decidir el momento óptimo para vender sus aceitunas a las cooperativas. El precio de las aceitunas en el mercado es altamente volátil y depende de múltiples factores, como las condiciones climáticas, la producción nacional e internacional, y las tendencias de consumo. Además, el tipo de aceite de oliva (virgen, virgen extra, lampante, etc.) influye significativamente en el precio y la demanda.

## Problema Específico

La falta de acceso a información actualizada y análisis de tendencias del mercado dificulta la toma de decisiones informadas sobre cuándo vender la cosecha y qué tipo de aceite producir. Esta incertidumbre puede resultar en ventas a precios bajos, afectando significativamente los ingresos familiares y la sostenibilidad de la actividad agrícola.

## Impacto

- **Económico:** Ventas a precios no óptimos reducen los márgenes de ganancia.
- **Operativo:** Dificultades en la planificación de recursos y logística.
- **Calidad del Producto:** La elección del tipo de aceite a producir afecta directamente la calidad y el valor en el mercado.

## Fuentes de Datos

Para abordar este problema, se utilizarán las siguientes fuentes de datos:

1. **Datos del Ministerio de Agricultura, Pesca y Alimentación (MAPA):**
   - **URL:** [Evolución de Precios de Aceitunas Vegetales](https://www.mapa.gob.es/es/agricultura/temas/producciones-agricolas/aceite-oliva-y-aceituna-mesa/Evolucion_precios_AO_vegetales.aspx)
   - **Descripción:** Proporciona información histórica y actualizada sobre los precios de la aceituna y el aceite de oliva, desglosados por tipo (virgen, virgen extra, lampante, etc.).
   - **Método de Acceso:**
     - **Descarga Manual:** Los datos están disponibles para descargar en formatos como Excel y PDF.
     - **Web Scraping:** Si los datos están en tablas HTML, se utilizarán técnicas de scraping para extraer la información.
   - **Formato de Datos:** Excel, CSV, PDF, HTML.

2. **API del Observatorio de Agricultura y Pesca de la Junta de Andalucía:**
   - **URL:** [Últimos Precios de Productos](https://ws142.juntadeandalucia.es/agriculturaypesca/observatorio/servlet/FrontController?action=UltimosPrecios&subsector=33&producto=33000&posicion=2291332)
   - **Descripción:** Proporciona los últimos precios de productos específicos, incluyendo aceitunas, desglosados por tipo.
   - **Método de Acceso:**
     - **Consulta Directa a la API:** Se realizarán solicitudes HTTP GET con los parámetros necesarios para obtener los datos en formato JSON o XML.
     - **Autenticación:** Verificar si es necesaria una clave API o token para acceder a los datos.
   - **Formato de Datos:** JSON, XML, HTML.

## Lógica de Negocio

La aplicación realizará las siguientes funciones clave:

1. **Recopilación de Datos:**
   - Extraer datos meteorológicos en tiempo real.
   - Obtener precios actuales y históricos de mercado desde las fuentes mencionadas, desglosados por tipo de aceite (virgen, virgen extra, lampante, etc.).
   - Recopilar tendencias de consumo y producción nacional e internacional.

2. **Análisis y Predicción:**
   - Utilizar **regresión lineal** para predecir las tendencias de precios futuros basándose en factores como las condiciones climáticas, la producción y el tipo de aceite.
   - Analizar patrones históricos para identificar factores que influyen en la volatilidad de los precios de cada tipo de aceite.

3. **Generación de Recomendaciones:**
   - Sugerir el momento óptimo para vender la cosecha y determinar qué tipo de aceite producir basándose en las predicciones de precios.
   - Proporcionar informes detallados que comparen diferentes escenarios de venta para cada tipo de aceite.

## Algoritmos y Métodos

- **Algoritmos de Predicción:**
  - **Regresión Lineal:** Para identificar la relación entre variables independientes (como clima, producción y tipo de aceite) y los precios de las aceitunas.
  
- **Métodos de Validación:**
  - **Validación Cruzada:** Para evaluar la precisión de los modelos.
  - **Métricas de Rendimiento:** Utilización de RMSE (Root Mean Square Error) y MAE (Mean Absolute Error) para medir la exactitud de las predicciones.

## Referencias

- [OpenWeatherMap API](https://openweathermap.org/api)
- [Evolución de Precios de Aceitunas Vegetales - MAPA](https://www.mapa.gob.es/es/agricultura/temas/producciones-agricolas/aceite-oliva-y-aceituna-mesa/Evolucion_precios_AO_vegetales.aspx)
- [Observatorio de Agricultura y Pesca - Junta de Andalucía](https://ws142.juntadeandalucia.es/agriculturaypesca/observatorio/servlet/FrontController?action=UltimosPrecios&subsector=33&producto=33000&posicion=2291332)

### Configuración del Repositorio

Para detalles sobre la configuración del entorno y del repositorio, consulta [este documento](docs/config.md).

### Lista de Comprobación

- [X] ¿Se trata de un problema real del que se tenga conocimiento personal?
- [X] ¿Se trata de un problema que para solucionar requiera el despliegue de una aplicación en la nube?
- [X] ¿La solución requiere una cierta cantidad de lógica de negocio, en vez de solucionarse sólo almacenando y buscando?
- [X] ¿Se ha incluido la configuración del repositorio y se ha enlazado desde el README?
- [X] ¿Tienes todos los datos necesarios para poder resolver el problema, o vas a requerir que el usuario los introduzca?
- [X] ¿Has seguido la lista de comprobación o estás marcando al buen tuntún todo?

