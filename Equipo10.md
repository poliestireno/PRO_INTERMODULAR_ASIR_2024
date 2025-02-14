# **Boceto del Proyecto TFG: Plataforma Web de Análisis de Logs de Seguridad con Apache Cassandra**

**Emily Almudena Morillo Montachana**

**Álvaro Barras Taracena**

**Leonardo Rafael Rodríguez Solano** 

## **1\. Título del Proyecto**

**Plataforma Web de Análisis de Logs de Seguridad con Apache Cassandra**

## **2\. Contexto y Justificación**

En un entorno digital donde la ciberseguridad es un pilar fundamental, las empresas y administradores de sistemas necesitan herramientas eficientes para la **detección y gestión de eventos de seguridad**. Cada día, los servidores, aplicaciones web y dispositivos de red generan **grandes volúmenes de logs**, los cuales contienen información crítica sobre intentos de acceso, actividad de usuarios y posibles ataques informáticos.

Sin una solución adecuada para **almacenar, analizar y visualizar** estos eventos, es difícil identificar amenazas en tiempo real y reaccionar ante incidentes de seguridad.

Este proyecto propone el desarrollo de una **plataforma web centralizada** que permita a los administradores visualizar, filtrar y analizar logs de seguridad en una **base de datos distribuida con Apache Cassandra**. Cassandra se elige por su **escalabilidad, tolerancia a fallos y capacidad para manejar grandes volúmenes de datos en entornos distribuidos**.

Además, el sistema **facilitará la detección de accesos sospechosos y patrones de comportamiento malicioso**, utilizando herramientas de procesamiento en tiempo real y alertas automatizadas.

## **3\. Objetivo del Proyecto**

El propósito del proyecto es proporcionar una solución escalable y eficiente para la **gestión y análisis de logs de seguridad** en infraestructuras de red y servidores.

### **Objetivos específicos:**

* Implementar **Apache Cassandra** como base de datos para almacenar logs de seguridad.  
* Diseñar un sistema capaz de **detectar accesos sospechosos** y registrar eventos relevantes.  
* Desarrollar una **interfaz web** que permita la consulta, filtrado y análisis de logs.  
* Garantizar la **escalabilidad y disponibilidad** de la solución mediante una arquitectura distribuida.  
* Integrar herramientas de **monitorización y generación de alertas** para mejorar la respuesta ante incidentes de seguridad.

## **4\. Tecnologías a Utilizar**

El sistema se desarrollará con herramientas especializadas para garantizar **eficiencia en el almacenamiento, procesamiento y visualización de datos**.

| Componente | Tecnología Seleccionada |
| ----- | ----- |
| **Base de Datos** | Apache Cassandra |
| **Backend** | Flask o Django (Python) |
| **Frontend** | React.js o Bootstrap con HTML/CSS |
| **Procesamiento** | Apache Spark |
| **Monitorización** | Grafana, Prometheus o Elastic (además de una web propia) |
| **Seguridad** | Cifrado TLS/SSL \+ Autenticación |

## **5\. Funcionamiento del Sistema**

El sistema opera en tres fases principales para capturar, analizar y visualizar eventos de seguridad.

### **1\. Captura y almacenamiento de eventos de seguridad**

* Se recopilan **logs generados por servidores SSH, Apache/Nginx y firewalls**.  
* Los registros se almacenan en **Apache Cassandra**, garantizando alta disponibilidad y rapidez en las consultas.

### **2\. Procesamiento y detección de anomalías**

* Se analizan **patrones de actividad sospechosa**, como intentos reiterados de acceso o tráfico anómalo.  
* Se procesan los datos en **Apache Spark** para identificar **comportamientos inusuales**.  
* Se generan **alertas automáticas** cuando se detectan posibles amenazas.

### **3\. Visualización y consulta de logs**

* Los administradores acceden a una **interfaz web** donde pueden visualizar los registros almacenados.  
* Se permite el **filtrado de eventos** por **fecha, dirección IP y tipo de alerta** para facilitar el análisis.  
* Se integra **Grafana o Prometheus** para generar **gráficos y reportes de seguridad**.

## **6\. Arquitectura del Sistema**

El sistema sigue una estructura modular y distribuida para garantizar **eficiencia y escalabilidad**.

`+--------------------+       +--------------------+       +--------------------+`  
`|   Captura de Logs  |       |   Apache Cassandra |       |   Aplicación Web   |`  
`| (SSH, Apache, etc.)|-----> |  (Base de Datos)   |-----> | (Consulta y Alertas) |`  
`+--------------------+       +--------------------+       +--------------------+`

* **Captura de Logs:** Servidores y firewalls generan registros de actividad.  
* **Almacenamiento:** Apache Cassandra permite gestionar y consultar grandes volúmenes de datos de manera eficiente.  
* **Procesamiento:** Apache Spark ayuda a analizar patrones y detectar actividad anómala.  
* **Visualización:** La interfaz web facilita la consulta de logs, mientras que herramientas como Grafana o Prometheus permiten monitorizar tendencias y generar reportes.
