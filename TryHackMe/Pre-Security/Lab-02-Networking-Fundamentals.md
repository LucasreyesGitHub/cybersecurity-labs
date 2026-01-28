# Lab 02 – Networking Fundamentals (TryHackMe)

## Objetivo
Comprender los fundamentos de redes necesarios para ciberseguridad, incluyendo
modelos de red, comunicación entre dispositivos, encapsulación de datos y
segmentación de redes.

Estos conceptos son esenciales para roles de SOC, Blue Team y Pentesting.

---

## ¿Qué es una red?
Una red es un conjunto de dispositivos conectados entre sí para intercambiar datos.
Estos dispositivos pueden ser computadoras, servidores, routers, switches o firewalls.

En ciberseguridad, entender cómo viaja la información es clave para detectar ataques,
analizar tráfico y responder a incidentes.

---

## Modelo OSI
El modelo OSI divide la comunicación en 7 capas:

1. Física – Transmisión de bits (cables, señales)
2. Enlace de Datos – Frames y direcciones MAC
3. Red – Direccionamiento IP y ruteo
4. Transporte – Comunicación confiable (TCP / UDP)
5. Sesión – Gestión de sesiones
6. Presentación – Formato y cifrado de datos
7. Aplicación – Servicios al usuario (HTTP, FTP, SMTP)

Este modelo ayuda a identificar en qué capa ocurre un problema o ataque.

---

## LAN (Local Area Network)
Una LAN conecta dispositivos dentro de un área limitada, como una casa u oficina.
Utiliza switches y routers para permitir la comunicación interna y con Internet.

Los atacantes suelen comenzar explotando debilidades dentro de la LAN.

---

## Paquetes y Frames
Los datos se dividen en paquetes para ser transmitidos.
Cada paquete se encapsula en diferentes capas según el modelo OSI.

Comprender paquetes y frames permite:
- Analizar tráfico de red
- Detectar ataques como sniffing o spoofing
- Investigar incidentes de seguridad

---

## Extensión de Redes
Las redes pueden ampliarse mediante:
- Routers
- Subredes
- NAT
- VPNs

Esto es fundamental para entender infraestructuras empresariales y entornos SOC.

---

## Importancia para Ciberseguridad
Networking Fundamentals es la base para:
- Análisis de tráfico
- Detección de intrusiones
- Monitoreo de logs
- Investigación de incidentes
- Pentesting y Red Team

---

## Conclusión
Este laboratorio proporciona las bases necesarias para comprender cómo fluye la
información en una red y cómo puede ser protegida o atacada.
