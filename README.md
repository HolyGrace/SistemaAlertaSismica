<p align=center><img src=https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png><p>

# <h1 align="center">**Sistema de Alertas Sísmicas**</h1>

<p align="center">
<img src="https://imgmedia.larepublica.pe/640x377/larepublica/migration/images/MGQ4EMJTTNGWPIKNXLCXXHNPSU.webp"> 
</p>

<center>
  
###### *Terremoto de Pisco, Perú - Agosto de 2007. Devastador sismo de magnitud 8.0 que impactó la región de Pisco, considerado uno de los más destructivos en la historia de Perú*

</center>

### Integrantes:
- Pedro Cornejo Mori
  
  pe.cor.12345@gmail.com
  
  [Linkedin](https://www.linkedin.com/in/pedro-cornejo-mori)
- Juan Sebastian Arias Ayala - Data Engineer
  
  juansebastianarias1@gmail.com
  
  [Linkedin](https://www.linkedin.com/in/juan-sebastian-arias-ayala)
- Jerson Brayan Gimenes Beltrán - Data Scientist
  
  jerson.gimenesbeltran@gmail.com
  
  [Linkedin](https://www.linkedin.com/in/jerson-gimenes-beltran/)
- Pablo Alberto Duque Marín
  
  pabdus3000@gmail.com
  
  [Linkedin](https://www.linkedin.com/in/pablo-alberto-duque-marin-426334155)

# Introducción

El Perú es un país altamente sísmico debido a su ubicación en el Cinturón de Fuego del Pacífico, una región donde se libera gran parte de la energía acumulada en la Tierra. La actividad sísmica en el país está relacionada con los procesos de convergencia de placas, especialmente entre la placa de Nazca y la placa Sudamericana, lo que provoca una intensa actividad sísmica, volcánica y otros efectos asociados. Por ejemplo, el terremoto de Pisco en el año 2007 causó la muerte de aproximadamente 595 personas y dejó más de 2,800 heridos. Además, los costos materiales asociados con este terremoto ascendieron a alrededor de 3 mil millones de dólares.

El Instituto Geofísico del Perú (IGP) ha registrado sismos durante más de 60 años y ha identificado importantes fuentes sismogénicas. Los sismos se clasifican según su profundidad en sismos de foco superficial (menor a 60 km), de foco intermedio (entre 61 y 300 km) y de foco profundo (mayor a 351 km). Estos sismos han afectado diversas áreas urbanas en el pasado, tanto en la costa como en la cordillera y en regiones como San Martín, Áncash, Junín, Ayacucho, Cusco y Arequipa.

Este repositorio contiene el proyecto de Sismos, el cual tiene como objetivo la recolección, almacenamiento y análisis de datos sísmicos para mejorar la monitorización y prevención de sismos de gran magnitud. Se utilizan diversas tecnologías de AWS, incluyendo un datalake, una API, el servicio S3 de AWS y el servicio Lambda de AWS para procesar los datos y mostrarlos en un dashboard de PowerBI.

### Causas:
Los sismos son causados por la liberación repentina de energía acumulada en la corteza terrestre. Esto puede ocurrir debido a la actividad de placas tectónicas, el movimiento de fallas geológicas, la actividad volcánica y la acción humana. Cuando la tensión en las rocas supera su resistencia, se produce una ruptura brusca, generando ondas sísmicas. Estas ondas se propagan por la Tierra, provocando un sismo. Las causas de los sismos varían según la ubicación y las características geológicas de cada región.

### Medición:
Los sismos se miden utilizando la escala de magnitud de momento, conocida como escala de Richter. Esta escala asigna un número que indica la cantidad de energía liberada durante un sismo. Los valores en la escala de Richter van desde menos de 2.0 para sismos microscópicos hasta más de 9.0 para sismos extremadamente fuertes. Cada aumento de un punto en la escala de Richter representa un aumento de aproximadamente 32 veces en la energía liberada. Además, los sismos también se pueden medir en términos de intensidad, que describe los efectos observados en la superficie. La escala de intensidad más utilizada es la escala de Mercalli, que va desde I (no se siente) hasta XII (total destrucción).

### Glosario de términos:
- **Sismo:** es un fenómeno natural que ocurre cuando se libera energía acumulada en la corteza terrestre, generando vibraciones o movimientos bruscos en la tierra. También se le conoce como terremoto.
- **Magnitud:** se refiere a la medida de la energía liberada durante el sismo. Se determina utilizando la escala de magnitud de momento, como la escala de Richter, que asigna un número para representar la fuerza del sismo. Valores más altos en la escala indican sismos más fuertes.
- **Profundidad:** se refiere a la distancia vertical desde la superficie terrestre hasta el punto donde se origina el sismo. Puede variar desde sismos superficiales, que ocurren cerca de la superficie, hasta sismos de mayor profundidad que se originan en las capas más internas de la Tierra.
- **Epicentro:** es el punto en la superficie de la Tierra directamente sobre el lugar donde se origina el sismo. Es el punto donde los efectos del sismo son más intensos y donde se registra la magnitud y localización inicialmente.
- **Hipocentro:** también conocido como foco sísmico, es el lugar en el interior de la Tierra donde se origina el sismo. Es el punto exacto donde se libera la energía acumulada y se inician las vibraciones sísmicas. La profundidad y ubicación del hipocentro son datos importantes para comprender la distribución de los sismos.

## Contexto de la propuesta: 
Se enfoca en la necesidad de detectar y comunicar de manera efectiva los eventos sísmicos en Perú, país reconocido por su alta actividad sísmica en la región latinoamericana. Es esencial contar con un sistema de alerta sísmica confiable que proporcione información oportuna y precisa a la comunidad civil. Además, como parte de una alianza tri-nacional con Estados Unidos (USGS) y Japón (JMA), se busca establecer estándares internacionales para la recolección y clasificación de datos sísmicos, así como desarrollar mecanismos de comunicación que sean comprensibles para la población, garantizando la protección de la salud, seguridad y bienestar de las personas ante los eventos sísmicos.

## Objetivos
- Identificar los criterios y parámetros necesarios para la clasificación de eventos sísmicos y la generación de alertas, tomando en cuenta la calidad de los datos recopilados. 
- Establecer los procedimientos y protocolos para la clasificación y alerta adecuados, considerando las características de cada país y las necesidades de la comunidad.
- Identificar zonas con mayor cantidad sísmica de cada país
- Realizar un análisis exhaustivo de la problemática sísmica en Perú, el país más sísmico de Latinoamérica, incluyendo el estudio de los datos históricos de sismos, sus características y los efectos en la población y en las estructuras.
- Realizar un análisis comparativo de la problemática sísmica en Perú, Estados Unidos y Japón, considerando el estudio de los datos históricos de sismos, sus características y los efectos en la población y en las estructuras, a fin de identificar similitudes, diferencias y lecciones aprendidas entre los tres países.

## ¿A quién estará dirigido el proyecto?
El proyecto estará dirigido al Instituto Nacional de Defensa Civil (INDECI). El INDECI es el organismo encargado de la gestión integral de riesgos de desastres en el país. Como ente rector, su función principal es coordinar y promover políticas, estrategias y acciones en la prevención, respuesta y rehabilitación frente a situaciones de emergencia. El proyecto busca colaborar con el INDECI en sus esfuerzos por fortalecer la capacidad de respuesta del país, reducir los riesgos asociados a los desastres y garantizar la protección de la población y las estructuras ante eventos sísmicos. Además, se busca establecer una coordinación estrecha con los diversos sectores, entidades gubernamentales y la sociedad civil, con el fin de lograr una gestión integral y efectiva de los riesgos sísmicos.

## Producto final
Este proyecto tiene como finalidad desarrollar un sistema de alertas sísmicas basado en un modelo de clasificación no supervisada. El sistema permitirá clasificar los sismos según patrones de peligrosidad (media/alta/baja) utilizando características como la magnitud, profundidad, latitud y longitud. Este proyecto forma parte de una colaboración tri-nacional entre Perú, Estados Unidos (USGS) y Japón (JMA) para estandarizar las redes sismológicas y mejorar la comunicación efectiva con la comunidad civil. También para facilitar la comprensión y la toma de decisiones informadas, el proyecto incluirá visualizaciones y mapas interactivos que mostrarán de manera clara y concisa la distribución geográfica de los sismos clasificados. El potencial cliente de este proyecto es el Instituto Nacional de Defensa Civil (INDECI) de Perú. 
Beneficios para la población en general y para las autoridades encargadas de la gestión de desastres en Perú:
- **Mayor seguridad:** El sistema de alertas sísmicas permitiría una respuesta más rápida y  eficiente ante sismos, lo que podría salvar vidas y reducir el impacto de los desastres naturales en la población.
- **Conciencia y preparación:** Las alertas tempranas ayudarían a crear conciencia sobre la peligrosidad de los sismos y fomentarán la preparación de la población, promoviendo la adopción de medidas de seguridad y mitigación de riesgos.
- **Mejora de la gestión de desastres:** El proyecto contribuiría a fortalecer las capacidades del INDECI en la gestión de desastres, brindando herramientas basadas en datos para una toma de decisiones más precisa y efectiva.
- **Colaboración internacional:** La colaboración tri-nacional con Estados Unidos y Japón permitiría establecer estándares de calidad en las redes sismológicas y promover la comunicación efectiva a nivel global, fortaleciendo el posicionamiento del INDECI en el ámbito internacional.

## Alcance
El alcance del proyecto consistirá en definir y desarrollar un modelo de predicción de sismos basado en datos históricos y proyecciones futuras, con el objetivo de evaluar las posibles consecuencias de los sismos y su impacto en una realidad hipotética. Se abordarán diferentes aspectos relacionados con la gestión de desastres, como la recopilación y análisis de datos sísmicos, la identificación de áreas de riesgo, la estimación de posibles daños y víctimas, así como la planificación de medidas preventivas.

## Diagrama ER
El diagrama ER representa la estructura de la base de datos utilizada para almacenar los datos sísmicos. Se ha considerado la adición de una tabla "Calendar" para facilitar el seguimiento y análisis de los eventos sísmicos en función de la fecha y el tiempo.

<p align="center">
<img src="https://github.com/HolyGrace/SistemaAlertaSismica/blob/master/img/ERD.jpg"> 
</p>

## Diccionario de Datos

A continuación se muestra el diccionario de datos para la base de datos de Sismos:

- **time:** Indica la fecha en formato UTC en la que ocurrió el sismo.  -
- **latitude:** Representa la latitud geográfica del epicentro del sismo.  
- **longitude:** Representa la longitud geográfica del epicentro del sismo.  
- **depth:** Indica la profundidad en kilómetros desde la superficie terrestre a la que se produjo el sismo.  
- **mag:** Es la magnitud del sismo, medida cuantitativa de la energía liberada durante el evento sísmico. Se encuentra en magnitud momento (Mw).  
- **updated:** Indica la fecha y hora de la última actualización de la información del sismo en el dataset.  
- **place:** Proporciona la ubicación geográfica general donde ocurrió el sismo, como el nombre del país, estado o ciudad.  
- **horizontalError:** Indica el error estimado en la ubicación horizontal del epicentro del sismo.  
- **id_country:** Contiene los identificadores únicos de los países donde ocurrieron los sismos.  

## Workflow

<p align="center">
<img src="https://github.com/pabdus/SistemaAlertaSismica/blob/master/img/aws.jpeg"> 
</p>

El siguiente es el flujo de trabajo utilizado para procesar los datos sísmicos:

### Recolección de datos:
- **a.** Se recopilan datos sísmicos de diversas fuentes, incluyendo sensores sísmicos en todo el mundo y datos históricos de sismos.-
- **b.** Se realiza una extracción de datos de las APIs de las páginas del USGS y del IGP. Se descarga la información mundial de sismos de los últimos 10 años, filtrando solo los países Japón, USA y Perú, y se guarda en formato CSV.
- **c.** Se crea un ETL para subir la información al cloud y realizar las pruebas correspondientes.

### Configuración inicial:
- **a.** Se crea una cuenta en AWS y se configura el cliente de terminal de AWS para levantar la infraestructura en la región OHIO-us-east-

- **b.** Almacenamiento de los datos en un datalake de AWS.

- **c.** Uso de una API para acceder a los datos almacenados en el datalake.

- **d.** Procesamiento de los datos utilizando el servicio Lambda de AWS.

- **e.** Almacenamiento de los datos procesados en el servicio S3 de AWS, que es el principal servicio de almacenamiento de archivos en AWS.

- **f.** Visualización de los datos en un dashboard de PowerBI.

## KPIs (Indicadores Clave de Rendimiento)
- **Reducción Anual del Número de Personas Afectadas por Sismos en Perú en un 30% en Comparación al Año Anterior.**

  Su funcionalidad radica en medir la efectividad de las estrategias implementadas para proteger a la población y disminuir los impactos de los sismos, buscando reducir significativamente el número de personas afectadas en comparación con el año anterior. Este KPI permite monitorear y evaluar el progreso en la reducción de los riesgos sísmicos, impulsando así la mejora continua de las políticas y acciones de protección civil en Perú.

- **Reducción Anual del Número de Personas Damnificadas por Sismos en Perú en un 20% en Comparación al Año Anterior.**

  Este indicador busca demostrar la disminución progresiva de personas afectadas por desastres naturales de sismos, promoviendo así la seguridad y el bienestar de la población peruana. Al reducir en un 20% el número de damnificados en comparación con el año anterior, se evidencia una mejora significativa en la capacidad de respuesta, prevención y protección ante eventos sísmicos, lo que refleja la eficacia de las políticas y acciones implementadas en este ámbito.

- **Reducción Anual del Número Total de Perdidas Materiales por Sismos en Perú en un 35% en Comparación al Año Anterior.**

  El objetivo de este kpi es lograr una disminución del 35% en las pérdidas materiales causadas por los terremotos en comparación con el año anterior. Este indicador permite evaluar el éxito de las estrategias implementadas para fortalecer la resiliencia y la capacidad de respuesta ante desastres naturales, proporcionando una medida cuantitativa de la mejora en la protección de los recursos y la infraestructura en el Perú.

- **Aumentar la Cantidad de Usuarios del Sistema de Alerta Sísmica en 2500 usuarios para el Próximo Mes.**

  Este KPI proporciona una medida cuantitativa de crecimiento, permitiendo evaluar el desempeño y la eficacia de las acciones tomadas para atraer nuevos usuarios. Al alcanzar este objetivo de aumentar la cantidad de usuarios en 2500, se logra fortalecer la cobertura del sistema de alerta sísmica y contribuir a la seguridad y protección de una mayor cantidad de personas ante posibles eventos sísmicos.
  
## AWS Cloud Stack
- **AWS:** Plataforma de nube de Amazon que proporciona una amplia gama de servicios, incluyendo almacenamiento, procesamiento en streaming, internet de las cosas, entre otros.  
- **AWS Datalake:** Utilizado para almacenar los datos sísmicos. Es un repositorio centralizado diseñado para almacenar, procesar y proteger grandes cantidades de datos.  
- **AWS Lambda:** Utilizado para procesar los datos sísmicos y almacenarlos en el servicio S3 de AWS. Es un servicio informático sin servidor que permite ejecutar código sin necesidad de aprovisionar o administrar servidores.  
- **AWS S3:** Utilizado para almacenar los datos procesados. Es el principal servicio de almacenamiento de archivos en AWS, que ofrece rentabilidad, seguridad y diversas configuraciones y gestiones del ciclo de vida de los archivos.

## Sistema de Alertas Pro (SAP)

Sistema de Alertas Pro (SAP)
El Sistema de Alertas Pro (SAP) es una plataforma que tiene como objetivo informar a la población sobre eventos sísmicos recientes. Utiliza la tecnología de mensajes de texto (SMS) y la plataforma de Whatsapp para enviar alertas en tiempo real.

Características principales:

Monitoreo sísmico en tiempo real: SAP se conecta a fuentes de datos sísmicos confiables para obtener información actualizada sobre eventos sísmicos.

Envío de alertas vía SMS: Cuando se detecta un sismo significativo, SAP envía mensajes de texto (SMS) a los usuarios registrados con detalles sobre el evento, como fecha, hora, ubicación y magnitud.

Notificaciones a través de Whatsapp: Además de los mensajes de texto, SAP también envía notificaciones a través de la plataforma de Whatsapp para llegar a un mayor número de personas y facilitar la visualización de la información.

El objetivo de SAP es brindar a la población una herramienta efectiva para estar informados sobre eventos sísmicos y tomar medidas preventivas en caso de ser necesario. La plataforma se esfuerza por garantizar la precisión y la rapidez en la entrega de alertas para aumentar la seguridad y la conciencia de la comunidad ante situaciones de riesgo.

## Stack Tecnológico General
[![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white&labelColor=101010)](https://code.visualstudio.com/docs)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)](https://docs.python.org/3/) 
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white&labelColor=101010)](https://aws.amazon.com/es/free/?gclid=Cj0KCQjw_O2lBhCFARIsAB0E8B9Hkiiw-3Bn1fREwAKYGhcurWpAF8I0UZohtrB0sH_C0-iqzrrzLHcaAmSnEALw_wcB&trk=1b5e0cad-6939-407d-b265-d513ac796285&sc_channel=ps&ef_id=Cj0KCQjw_O2lBhCFARIsAB0E8B9Hkiiw-3Bn1fREwAKYGhcurWpAF8I0UZohtrB0sH_C0-iqzrrzLHcaAmSnEALw_wcB:G:s&s_kwcid=AL!4422!3!647999789244!p!!g!!aws!19685311604!143348651942)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=white&labelColor=101010)](https://learn.microsoft.com/en-us/power-bi/) 
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white&labelColor=101010)](https://dev.mysql.com/doc/) 

[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white&labelColor=101010)](https://docs.streamlit.io/) 
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white&labelColor=101010)](https://git-scm.com/doc)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://docs.github.com/en)

## [Link de los datasets](https://drive.google.com/drive/folders/1ujrPcokGmVWx-feOcKnkvmp1UN86B12Q)
En el transcurso del proyecto, se han utilizado datasets extraídos de las APIs de la USGS, de la IGP y de la INDECI. El enlace proporcionado conduce a estos datasets, incluidos aquellos a los que se les aplicó un proceso de Extracción, Transformación y Carga (ETL) y aquellos que no fueron sometidos a este proceso.

## ***[Link del Producto Final del Proyecto](https://jersonbgb-projectfinal-group12-ml-sismos.streamlit.app/)***

## Bibliografía:
- https://earthquake.usgs.gov/fdsnws/event/1/
- https://ultimosismo.igp.gob.pe/datos-sismicos
- https://portal.indeci.gob.pe/direccion-politicas-y-planes/base-de-datos-de-emergencia-y-danos/
- https://www.sgp.org.pe/alerta-peru-un-pais-altamente-sismico/
- https://es.statista.com/estadisticas/1379060/indice-de-riesgo-sismico-de-lo-spaises-de-america-latina-y-el-caribe/#:~:text=Seg%C3%BAn%20el%20%C3%ADndice%20de%20riesgo,%2C%20con%20un%209%2C8.
