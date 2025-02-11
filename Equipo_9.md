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
