# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller X - Taller-04-infraestructura-AREM

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

### Vista de contexto

![Mapa de infraestrutura](mapa-final.png)


## 🔍 Investigación complementaria
### Tema investigado:
(Ej: Buenas prácticas BPMN, comparación TOGAF vs C4, principios de seguridad STRIDE, etc.)

### Resumen:
Describa en 2–3 párrafos lo investigado, citando fuentes cuando sea necesario. Incluya cómo se relaciona con el taller.

## 📚 Referencias
- [1] Apellido, Nombre. *Título*. Año. URL o DOI.
- [2] Fuente oficial BPMN: https://www.omg.org/spec/BPMN/

---

_Este documento hace parte de la entrega del taller X del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
