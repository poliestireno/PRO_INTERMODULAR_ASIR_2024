# Monitorización Completa en Tiempo Real de una Red Securizada

## 1️⃣ Introducción  
Este proyecto implementa una **red local securizada y monitorizada en tiempo real**. La infraestructura consta de:  

- Un **router**.  
- Un **firewall** para la seguridad de la red.  
- Un **servidor con Redis** para recopilar datos de los clientes mediante scripts sistemas de recopilacion de informacion.  
- Un **servidor web (Apache)** para la gestión y administracion de los datos vía interfaz web.  
- Un **servidor con servicios básicos** como **DNS, DHCP, CORREO**.  

## 2️⃣ Objetivo  
El objetivo principal es gestionar **en tiempo real** todos los datos y eventos de la red mediante un **entorno gráfico (página web)** que permitirá:  

- **Implementar sistemas de seguridad**
- **Visualizar** la información recopilada.  
- **Modificar** o actualizar datos en la base de datos.  
- **Eliminar** información cuando sea necesario.  

## 3️⃣ Base de Datos: Redis  
Para almacenar los datos se utilizará **Redis**, una base de datos **NoSQL**, debido a los siguientes beneficios:  

✅ **Alta velocidad de acceso** para gestionar grandes volúmenes de datos en tiempo real.  
✅ **Evita conflictos** con los scripts de recopilación de datos, problema observado en pruebas con MySQL.  

### 🔍 Información recopilada  
La base de datos almacenará múltiples tipos de información, incluyendo:  

- **Datos del sistema** de cada cliente.  
- **Direcciones IP** asignadas.  
- **Registros de auditoría** de la red.  
- **Historial de páginas web visitadas**.  
- **Solicitudes de red** procesadas.
- **Estado de los servicios**

## 4️⃣ Seguridad y Reglas de Firewall  
La red de clientes estará protegida por un **firewall** con reglas específicas, tales como:  

- 🔒 **Enmascaramiento de IP**.  
- 🚫 **Bloqueo de acceso** a ciertos contenidos web.  
- 📊 **Filtrado de tráfico** según necesidades de la red.  

## 5️⃣ Función del Servidor DNS/DHCP  
El servidor que contiene **DNS, DHCP y CORREO INTERNO** tendrá un rol clave en la red:  

📜 **Distribución de scripts** a los clientes para la recopilación de información.  
📡 **Gestión de direcciones IP dinámicas** mediante DHCP.  
🔗 **Resolución de nombres de dominio** con DNS.  
✉️ **Envio de correos entre los clientes** de la red local
## 6️⃣ Conclusión  
Este sistema permitirá un control **eficiente, seguro y en tiempo real** sobre la infraestructura de red, ofreciendo una interfaz web intuitiva para la monitorización y gestión de datos.  

🚀 **Tecnologías Clave**: Redis, Apache, Firewall, DNS, DHCP, CORREO.  

## 7️⃣Esquema logico

![image](https://github.com/user-attachments/assets/f9f5c543-0e03-458e-97d7-605f458196f8)


