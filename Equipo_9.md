Grupo compuesto por : 

[Leonardo David Arenas López](mailto:ldalopez@lasalleinstitucion.es)

[Jonathan Javier Cumbajin Vaca](mailto:jjcvaca@lasalleinstitucion.es)

[Jonatan Andrés Benítez Narváez](mailto:jabnarvaez@lasalleinstitucion.es)

Título del Proyecto: 

**"Implementación de un Servidor Inteligente para la Gestión de Redes”**

El proyecto consiste en crear un servidor inteligente para la gestión de redes que integre herramientas como Redis para almacenamiento en caché, phpMyAdmin para gestionar la base de datos, y un sistema de firewall con proxy para mejorar la seguridad. Además, se incorporará Inteligencia Artificial (IA) para el análisis de tráfico, optimización de servicios como DHCP y DNS, y la detección de posibles amenazas. Este servidor proporcionará servicios críticos para una red empresarial, mejorando tanto el rendimiento como la seguridad.

### **Esquema del Proyecto:**

* **Servidor Principal:**  
  - **Servicios de Red:**  
    * **DHCP:** Asigna dinámicamente direcciones IP a los dispositivos conectados.  
    * **DNS:** Resuelve nombres de dominio a direcciones IP.  
    * **Redis:** Almacenamiento en caché para optimizar el rendimiento de las consultas DNS y asignaciones DHCP.  
    * **Base de Datos (MySQL/MariaDB):** Almacena logs y estadísticas de tráfico.  
* **Inteligencia Artificial:**  
  - **Monitoreo de tráfico:** Analiza el comportamiento de la red en tiempo real.  
  - **Optimización:** Mejora la asignación de direcciones IP y la resolución DNS.  
  - **Detección de amenazas:** Identifica patrones sospechosos y genera alertas.  
* **Base de Datos con phpMyAdmin:**  
  - **phpMyAdmin:** Herramienta para gestionar la base de datos visualmente.  
  - **Almacenamiento de datos:** Logs de tráfico, usuarios conectados, configuraciones de red, etc.  
* **Seguridad:**  
  - **Firewall:**  
    * **iptables / ufw:** Filtra el tráfico no autorizado, protege puertos sensibles.  
  - **Proxy (Squid):**  
    * Filtra y enruta el tráfico web, bloqueando accesos no deseados y actuando como caché.  
* **Integración:**  
  - **Redis**: Mejora la eficiencia mediante la caché de peticiones frecuentes (DNS, DHCP).  
  - **phpMyAdmin**: Facilita la gestión de bases de datos con una interfaz web.  
  - **Firewall \+ Proxy**: Proporciona seguridad controlando el acceso a la red y filtrando tráfico.
 
# Servicio de Página Web con IA (Chat GPT y Análisis de Datos)

## Objetivo:
Crear un servicio web donde los usuarios interactúan con una inteligencia artificial (GPT) que tiene capacidades constructivas, análisis de datos y una serie de funcionalidades relacionadas con redes complejas.

## Requerimientos Técnicos:

### Infraestructura de Red Compleja:
- **DHCP**: Proporcionar direcciones IP dinámicas a las máquinas en la red.
- **DNS**: Configuración de un servidor DNS interno para resolver nombres dentro de la red y un servidor DNS público para el sitio web.
- **Firewalls**: Implementar un firewall robusto para proteger el servidor web y los datos de los usuarios, asegurando que solo el tráfico legítimo llegue a los servicios.
- **Proxy**: Configurar un servidor proxy para asegurar que las conexiones salientes y entrantes sean filtradas correctamente, protegiendo la red interna de accesos no deseados.
- **VPN**: Establecer una VPN para permitir el acceso seguro de administradores y usuarios remotos al sistema.

### Seguridad en la Web:
- **SSL/TLS**: Asegurarse de que la comunicación entre el servidor web y los usuarios sea cifrada usando HTTPS.
- **Autenticación y autorización**: Implementar autenticación multifactor para proteger el acceso a la página web, especialmente en la parte administrativa.
- **Análisis de Seguridad**: Realizar auditorías de seguridad utilizando herramientas de escaneo de vulnerabilidades como OpenVAS y configurar alertas para posibles amenazas.

### Servicio Web:
- Crear la página web con frameworks modernos como React o Angular para la interfaz del usuario, donde los usuarios pueden interactuar con el chat de IA.
- Implementar un API RESTful para la comunicación con el servidor backend, que puede estar construido en Node.js o Python (Flask/Django).
- La IA se puede implementar usando un modelo GPT preentrenado de OpenAI o similar, y se pueden integrar capacidades adicionales de análisis de datos utilizando Python (Pandas, NumPy, SciPy).

### Implementación de IA:
- La IA debe ser capaz de realizar análisis de datos sobre las interacciones de los usuarios, como identificar patrones de comportamiento sospechosos o necesidades comunes para mejorar la experiencia.
- Incorporar capacidades para realizar consultas de red básicas a través de la IA (por ejemplo, preguntar sobre el estado de un servicio como DNS o DHCP).

### Estructura de Servicios en Red:
- **Gestión de Logs**: Implementar un servicio de Centralización de Logs usando herramientas como ELK Stack (Elasticsearch, Logstash y Kibana) para almacenar y analizar eventos de seguridad y operativos.
- **Balanceo de Carga**: Si esperas una carga considerable de tráfico, deberías considerar un sistema de balanceo de carga como HAProxy o NGINX.

---

# Segunda Idea: IA Operativa para Redes de Empresa (Administración Automática de Redes)

## Objetivo:
Crear una IA que gestione la red interna de una empresa, permitiendo a los administradores dar órdenes a través de un chat para modificar la configuración de servicios clave (DHCP, DNS, Proxy, Firewall, VPN) y realizar análisis de seguridad.

## Requerimientos Técnicos:

### Redes y Servicios Administrados por la IA:
- **DHCP**: Implementar un sistema donde la IA pueda interactuar con el servidor DHCP para modificar configuraciones de direcciones IP, rangos, y reservas.
- **DNS**: La IA debe ser capaz de agregar o modificar registros DNS, así como identificar y solucionar problemas de resolución de nombres.
- **Proxy**: Configurar el proxy de manera dinámica, permitiendo que la IA gestione las reglas de acceso, cache y filtrado.
- **Firewall**: La IA debe poder configurar reglas de firewall para permitir o bloquear tráfico, integrando herramientas como iptables o pfSense.
- **VPN**: La IA puede gestionar conexiones VPN, configurando accesos y monitoreando su rendimiento.

### Chat con IA:
- Implementar un chatbot que se integre con sistemas de gestión de red, donde los administradores o usuarios autorizados pueden interactuar con la IA para realizar tareas como modificar configuraciones, analizar el estado de los servicios y recibir recomendaciones.
- Utilizar un framework de chatbot como Rasa o Dialogflow, combinado con un modelo de lenguaje GPT para dar respuestas naturales y efectivas.

### Análisis de Seguridad:
- **Análisis de Vulnerabilidades**: La IA puede analizar la red en busca de vulnerabilidades conocidas usando herramientas como Nessus o OpenVAS, proporcionando informes automáticos.
- **Detección de Anomalías**: Implementar sistemas de detección de intrusiones (IDS) como Snort o Suricata para monitorizar el tráfico y detectar patrones inusuales.

### Interfaz Web Administrativa:
- Crear un panel de administración con React o Angular, donde los administradores puedan supervisar el estado de la red, ver alertas y resultados de análisis de seguridad, y gestionar servicios como DHCP, DNS, Proxy, etc.
- Asegurarse de que este panel esté protegido mediante autenticación robusta y autorización de roles.

### Monitorización y Gestión Proactiva:
- Integrar herramientas de monitorización en tiempo real como Prometheus y Grafana para hacer un seguimiento de la salud de los servicios de red y la seguridad.
- Implementar alertas automáticas en caso de problemas con la red o la seguridad, y permitir que la IA proponga soluciones o cambios.

### Infraestructura en la Nube:
- Si el proyecto se enfoca en un entorno más global, podrías considerar la posibilidad de implementar algunos servicios en la nube utilizando plataformas como AWS, Azure o Google Cloud.
- Estos servicios pueden incluir bases de datos (como Amazon RDS para MySQL o PostgreSQL) y almacenamiento en la nube (como Amazon S3).

---

# Recomendaciones para Implementaciones de Red y Seguridad:

## Seguridad y Protección:
- Implementa Cifrado de extremo a extremo (TLS) para todas las comunicaciones en la red.
- Usa Redes Privadas Virtuales (VPN) para asegurar la comunicación entre los diferentes servicios de red y permitir accesos remotos seguros para administradores.
- Configura Autenticación multifactor para los accesos a la plataforma administrativa.

## Automatización y Orquestación:
- Para mejorar la eficiencia, podrías usar herramientas como Ansible o Terraform para automatizar la configuración y mantenimiento de los servicios en tus máquinas virtuales.

## Pruebas y Simulación:
- Realiza pruebas de seguridad continuas y simulaciones de ataques (como penetration testing), utilizando herramientas como Kali Linux o Metasploit, para asegurar que la infraestructura esté bien protegida contra posibles amenazas.

## Escalabilidad:
- Considera la posibilidad de que tu servicio crezca con el tiempo. Usa Docker y Kubernetes para crear contenedores y gestionar la escalabilidad de tu servicio.

