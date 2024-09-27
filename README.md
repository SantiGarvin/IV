# Plataforma de Análisis del Mercado Inmobiliario

## Descripción del Proyecto

### Objetivo

Analizar datos del mercado inmobiliario para proporcionar insights sobre tendencias de precios, demanda por ubicación, tipos de propiedades más buscadas, entre otros aspectos relevantes.

### Procesamiento

- **Recolección y limpieza de datos:** Obtener datos de propiedades en venta y alquiler desde APIs de inmobiliarias, portales de anuncios clasificados y datasets abiertos de bienes raíces.
- **Análisis de tendencias de precios:** Identificar patrones y tendencias en los precios de las propiedades a lo largo del tiempo.
- **(Opcional) Predicción de valorización de propiedades:** Implementar modelos de machine learning para predecir el aumento o disminución de los precios de las propiedades en diferentes áreas.

### Despliegue en la Nube

Crear una aplicación web que muestre:

- Mapas interactivos con ubicaciones de propiedades.
- Gráficos de tendencias de precios.
- **(Opcional) Predicciones de precios futuros.**
- **(Opcional) Identificación de áreas emergentes mediante clustering.**

## Cumplimiento de Requisitos

### Problema Real y Conocimiento Personal

El mercado inmobiliario es dinámico y afecta a muchas personas que buscan comprar, vender o alquilar propiedades. Este proyecto proporciona una herramienta que ayuda a los usuarios a tomar decisiones informadas basadas en datos reales y análisis predictivos opcionales.

### Despliegue en la Nube

La aplicación será accesible desde cualquier lugar con conexión a internet. Todos los datos serán procesados y almacenados en la nube, garantizando accesibilidad y escalabilidad.

### Lógica de Negocio

El proyecto incluye:

- Análisis de datos inmobiliarios.
- **(Opcional) Predicción de precios futuros.**
- **(Opcional) Identificación de áreas emergentes mediante clustering.**

### Datos Necesarios

- Acceso a APIs de inmobiliarias como Zillow API y Realtor API.
- Scraping legal de portales inmobiliarios si es necesario.
- Uso de datasets abiertos de bienes raíces disponibles públicamente.

## Características Avanzadas (Opcional)

Para usuarios que deseen funcionalidades adicionales, se pueden implementar las siguientes características avanzadas utilizando técnicas de machine learning:

- **Predicción de Valorización de Propiedades:** Utilizar modelos de machine learning para predecir la valorización futura de las propiedades en diferentes áreas.
- **Clustering de Áreas Emergentes:** Aplicar algoritmos de clustering para identificar zonas con potencial de crecimiento en el mercado inmobiliario.
- **Análisis Predictivo de Demanda:** Predecir la demanda de propiedades en distintas ubicaciones y tipos de inmueble.

Estas características avanzadas requieren conocimientos adicionales en machine learning y pueden ser implementadas como módulos opcionales dentro de la plataforma.

## Configuración del Repositorio

Para detalles sobre la configuración del entorno y del repositorio, consulta [este documento](docs/config.md).

## Lista de Comprobación

Antes de realizar la entrega, asegúrate de que tu proyecto cumple con los siguientes puntos:

- [X] ¿Se trata de un problema real del que se tenga conocimiento personal?
- [X] ¿Se trata de un problema que para solucionar requiera el despliegue de una aplicación en la nube?
- [X] ¿La solución requiere una cierta cantidad de lógica de negocio, en vez de solucionarse sólo almacenando y buscando?
- [ ] ¿Se ha incluido la configuración del repositorio y se ha enlazado desde el README?
- [X] ¿Tienes todos los datos necesarios para poder resolver el problema, o vas a requerir que el usuario los introduzca?
- [X] ¿Has seguido la lista de comprobación o estás marcando al buen tuntún todo?

