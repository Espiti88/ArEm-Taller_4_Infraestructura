# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
Taller-04-infraestructura-AREM

## 👥 Integrantes del equipo

- Edwin Alejandro Gutierrez Rodriguez
- Samuel Espitia Cruz
- Nicolas Stiven Ortiz Cortes

## 🧠 Descripción general del trabajo

Este trabajo presenta la documentación y representación gráfica de la infraestructura tecnológica del área de adquisiciones. A partir de la información suministrada por el área responsable, se identificaron los principales sistemas en uso (ERP PeopleSoft y portal de servicios en Oracle Cloud, así como recursos locales como SharePoint y bases de datos). Además, se registraron los mecanismos de autenticación mediante Active Directory y las limitaciones de acceso establecidas. Finalmente, la infraestructura fue plasmada en un diagrama elaborado en draw.io, que permite visualizar de forma clara la organización y funcionamiento de los componentes tecnológicos.

## 🔧 Proceso de desarrollo
Para la elaboración del mapa de infraestructura del sector de adquisiciones, se inició con una serie de preguntas dirigidas al área responsable. El objetivo fue obtener información concreta acerca de la arquitectura tecnológica que utilizan actualmente. Se indagó principalmente sobre:

- Arquitectura utilizada: cuáles son los componentes de red y sistemas que conforman su infraestructura. En este apartado se encontró que usan un ERP proporcionado por Oracle Cloud, el cual es People Soft, que es usado como Siga Financiero, además de un portal de servicios que tambien es parte de Oracle. De manera local se encunetran archivos en un SharePoint para tener un control interno. 

- Método de autenticación: cómo los usuarios acceden a los diferentes servicios y archivos, en la cual unicamente se usa el Active Directory que propociona la universidad

- Limitaciones existentes: qué restricciones de acceso o barreras de seguridad aplican dentro del entorno. En la cual se encontró que para acceder al protal de servicios se requiere estar en la red del campus.


Con la información recopilada, se procedió a representar gráficamente la infraestructura utilizando la herramienta draw.io. En el diagrama se incluyeron los distintos componentes de red, servidores y sistemas clave, mostrando la interacción entre ellos (por ejemplo, conexión con SharePoint, bases de datos locales, ERP y portal de servicios en la nube).

El resultado fue un mapa visual de la infraestructura de adquisiciones, que facilita la comprensión de cómo se encuentran organizados los servicios y las restricciones de seguridad aplicadas.

## 🧩 Análisis del modelo propuesto
- **Cómo se estructura el modelo entregado:**
El modelo elaborado se presenta de manera jerárquica, distinguiendo entre los recursos en la nube y los recursos locales. En la capa superior se encuentran los servicios alojados en Oracle Cloud, dentro de los cuales destacan el ERP PeopleSoft, empleado como sistema financiero institucional, y el portal de servicios que complementa los procesos del área de adquisiciones. Estos servicios se vinculan con los usuarios a través de la red institucional, que se encuentra protegida por un firewall que únicamente permite el acceso desde el campus universitario.
En la capa local se integraron elementos como SharePoint y las bases de datos internas, que funcionan como mecanismos de control y seguimiento de las solicitudes. Todo el conjunto se articula mediante el uso de Active Directory, que centraliza los procesos de autenticación y otorga coherencia a la administración de usuarios.

- **Cómo representa las necesidades del cliente:**
El diagrama responde a las principales necesidades del área de adquisiciones al reflejar su esquema actual de trabajo. En primer lugar, asegura la representación de los sistemas financieros críticos (ERP) y del portal de servicios como herramientas esenciales para la gestión de procesos. En segundo lugar, visibiliza la existencia de repositorios locales (SharePoint y bases de datos) que permiten mantener un control interno complementario. Finalmente, destaca la importancia del mecanismo de autenticación basado en Active Directory, que constituye un requisito institucional para la gestión unificada de accesos y permisos.

- **Qué supuestos se tomaron:**
En el proceso de construcción del modelo se asumió que la información proporcionada por el área de adquisiciones es completa y refleja fielmente la infraestructura utilizada en la actualidad. Se consideró además que las restricciones de acceso identificadas, como la necesidad de conexión desde la red del campus para ingresar al portal de servicios, aplican de manera generalizada a todos los usuarios. Asimismo, se asumió que el uso de Oracle Cloud como proveedor de servicios es una decisión institucional consolidada, que orienta y condiciona la estructura tecnológica del área de adquisiciones.

## 📈 Diagrama final entregado

### Vista de infraestructura

![mapa-final](mapa-final.png)


## 🔍 Investigación complementaria
### Tema investigado:  Buenas prácticas de arquitectura de infraestructura (cloud, on-premise, híbrida).

•  Definir claramente los objetivos del negocio y criterios para decidir qué cargas de trabajo deben estar en la nube, cuáles on-premises o híbridas. Esto incluye aspectos como latencia, cumplimiento regulatorio, seguridad y costos. 
•  Establecer una gobernanza unificada: políticas, roles y procedimientos que se apliquen tanto en entornos locales como en la nube, para mantener consistencia en seguridad, cumplimiento y gestión. 
•  Utilizar herramientas y procesos comunes o compatibles en ambos entornos (on-premise y cloud) para administración, monitorización, autenticación y despliegue. Esto facilita interoperabilidad, despliegue uniforme y reduce errores. 
•  Seguridad integral: aplicar controles como cifrado de datos en tránsito y en reposo, un modelo de identidad único (IAM), principio de privilegio mínimo, monitoreo continuo, auditorías regulares. 
•  Alta disponibilidad, resiliencia y recuperación ante desastres: asegúrate de que la arquitectura soporte fallos, con redundancia, backups y procedimientos de recuperación probados. 
•  Optimización de costos: monitorear uso de recursos, evitar sobre-aprovisionamiento, usar tarifas reservadas o instancias según demanda, apagar recursos inactivos, etc. 
•  Planificación de red y conectividad: establecer conexiones seguras, de bajo latencia entre la red local y la nube (VPN, líneas dedicadas, etc.), definir redes virtuales, segmentación, etc. 
•  Hacer pruebas constantes: no solo al inicio, sino testeos de rendimiento, pruebas de recuperación, validación de seguridad, simulaciones de fallos. Esto ayuda a detectar puntos débiles anticipadamente.


### Resumen:
En la investigación realizada sobre buenas prácticas de arquitectura de infraestructura en entornos cloud, on-premise e híbridos, se identificó que un aspecto fundamental es alinear la tecnología con los objetivos del negocio. Para ello, se recomienda definir criterios claros que determinen qué cargas de trabajo se ejecutan en la nube, cuáles permanecen en servidores locales y cuáles se gestionan bajo un modelo híbrido. Otro elemento central es la gobernanza unificada, que implica establecer políticas, roles y procedimientos consistentes para la gestión de recursos, la seguridad y el cumplimiento normativo, sin importar el entorno donde se ubiquen los sistemas.

Asimismo, la literatura consultada enfatiza la importancia de contar con controles de seguridad integrales, como el cifrado de datos, la gestión centralizada de identidades y accesos (IAM), la aplicación del principio de privilegio mínimo y el monitoreo continuo. Se destaca también la necesidad de planificar adecuadamente la conectividad entre la nube y los sistemas locales, garantizando baja latencia y comunicación segura mediante redes virtuales, VPN o enlaces dedicados.

Finalmente, se recomienda implementar prácticas que aseguren la resiliencia y la optimización de costos. Esto incluye la creación de arquitecturas con alta disponibilidad, planes de recuperación ante desastres, pruebas constantes de rendimiento y seguridad, así como mecanismos de control para evitar sobre-aprovisionamiento y gastos innecesarios en recursos. Estas prácticas constituyen un marco de referencia sólido para el diseño y gestión eficiente de infraestructuras modernas.

La revisión de buenas prácticas en arquitecturas de infraestructura resulta pertinente al trabajo realizado, ya que permite contrastar el modelo actual del área de adquisiciones con lineamientos ampliamente aceptados en el ámbito tecnológico. El diagrama elaborado refleja una infraestructura que combina servicios en la nube (Oracle Cloud) y recursos locales (SharePoint y bases de datos), lo cual se alinea con un enfoque híbrido. En este sentido, prácticas como la gobernanza unificada, la seguridad integral y la planificación de conectividad ofrecen un marco de referencia que puede guiar futuras mejoras, garantizando que la arquitectura no solo cumpla con las necesidades operativas actuales, sino que también evolucione hacia estándares de mayor resiliencia, seguridad y eficiencia.

## 📚 Referencias
- [1] New Relic. Hybrid Cloud Deployment Models and Examples. 2023. Disponible en: https://newrelic.com/de/blog/best-practices/hybrid-cloud-deployment-models-examples

- [2] Cloudian. Hybrid Cloud Infrastructure: 6 Components and How to Put Them Together. 2024. Disponible en: https://cloudian.com/guides/hybrid-cloud/hybrid-cloud-infrastructure-6-components-putting-them-together

- [3] Cyscale. Hybrid Cloud Best Practices: Security, Compliance and Cost Management. 2023. Disponible en: https://cyscale.com/blog/hybrid-cloud-best-practices

- [4] Amazon Web Services (AWS). Hybrid Cloud Best Practices – Prescriptive Guidance. 2024. Disponible en: https://docs.aws.amazon.com/prescriptive-guidance/latest/hybrid-cloud-best-practices/introduction.html

- [5] Aptum. Hybrid Cloud: Best Practices for Modern Enterprises. 2022. Disponible en: https://aptum.com/knowledge-center/hybrid-cloud

---

_Este documento hace parte de la entrega del taller Taller-04-infraestructura-AREM del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
