# Intro to LAN (Local Area Network) — Consolidated Technical Documentation

## Overview

Este documento consolida los conceptos fundamentales del módulo **Intro to LAN** de TryHackMe, integrando teoría de redes, funcionamiento interno y fundamentos de seguridad.

La comprensión sólida de una LAN es esencial para cualquier profesional de ciberseguridad, ya que la mayoría de los ataques comienzan o se expanden dentro de redes internas.

---

# 1. ¿Qué es una LAN?

Una **LAN (Local Area Network)** es una red que interconecta dispositivos dentro de un área geográfica limitada (hogar, oficina, campus).

Permite:

- Compartición de recursos
- Comunicación interna de baja latencia
- Administración centralizada
- Control de seguridad perimetral

Las LAN modernas utilizan principalmente Ethernet (cableado) y Wi-Fi (inalámbrico).

---

# 2. Componentes Fundamentales de una LAN

## 2.1 Hosts (End Devices)

Dispositivos finales que generan o consumen datos:

- PCs
- Servidores
- Dispositivos móviles
- IoT

Cada host posee:

- Dirección MAC (capa 2)
- Dirección IP (capa 3)

---

## 2.2 Switch (Layer 2 Device)

Dispositivo que opera en la **capa de enlace de datos**.

Funciones:

- Mantiene una tabla MAC (CAM Table)
- Reenvía tramas según dirección MAC destino
- Reduce dominios de colisión
- Mejora eficiencia frente a hubs

---

## 2.3 Router (Layer 3 Device)

Opera en la **capa de red**.

Funciones:

- Conecta múltiples redes
- Mantiene tabla de enrutamiento
- Determina la mejor ruta para paquetes
- Actúa como gateway predeterminado

En entornos domésticos suele integrar:

- NAT
- Firewall básico
- DHCP

---

## 2.4 Access Point (AP)

Permite conexión inalámbrica:

- Opera en 2.4 GHz y 5 GHz
- Autentica dispositivos Wi-Fi
- Integra dispositivos inalámbricos a la LAN cableada

---

## 2.5 Firewall

Controla tráfico:

- Entrante
- Saliente
- Interno

Aplica reglas basadas en:

- IP
- Puerto
- Protocolo

---

# 3. Direccionamiento en LAN

## 3.1 MAC Address

- Identificador físico único
- 48 bits
- Representación hexadecimal
- Utilizado en capa 2

Ejemplo: 00:1A:2B:3C:4D:5E


---

## 3.2 IP Address

Dirección lógica utilizada para identificar dispositivos en una red.

### IPv4

- 32 bits
- Ejemplo: 192.168.1.10

### IPv6

- 128 bits
- Mayor espacio de direccionamiento

---

## 3.3 DHCP (Dynamic Host Configuration Protocol)

Asigna automáticamente:

- Dirección IP
- Máscara de subred
- Gateway
- DNS

Reduce errores de configuración manual.

---

# 4. Subnetting y Segmentación

## 4.1 Subnetting

Proceso de dividir una red en subredes más pequeñas.

Ejemplo: 192.168.1.0/24 → 254 hosts utilizables


Beneficios:

- Mejor organización
- Mejor rendimiento
- Control granular

---

## 4.2 VLAN (Virtual LAN)

Segmentación lógica dentro de un switch físico.

Permite:

- Separar departamentos
- Aislar tráfico
- Aplicar políticas específicas

Reduce propagación lateral de amenazas.

---

# 5. Modelos de Red

## 5.1 Modelo OSI

7 capas:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

Permite diagnosticar problemas por capa.

---

## 5.2 Modelo TCP/IP

Modelo práctico usado en Internet:

1. Link
2. Internet
3. Transport
4. Application

---

# 6. Protocolos Fundamentales

## 6.1 ARP (Address Resolution Protocol)

Resuelve: IP → MAC


Esencial en comunicación interna.

Vulnerabilidad común:

- ARP Spoofing

---

## 6.2 TCP

- Orientado a conexión
- Confiable
- 3-way handshake
- Control de flujo y congestión

---

## 6.3 UDP

- No orientado a conexión
- Baja latencia
- Sin garantía de entrega

Usado en:

- DNS
- Streaming
- VoIP

---

# 7. Flujo de Comunicación en una LAN

Cuando un host A quiere comunicarse con host B:

1. Verifica si está en la misma subred.
2. Si es local:
   - Envía broadcast ARP.
   - Obtiene MAC destino.
   - Envía trama al switch.
3. El switch reenvía la trama al puerto correcto.
4. Si es externo:
   - Envía paquete al gateway (router).

---

# 8. Conceptos Clave de Dominio

## 8.1 Broadcast Domain

Conjunto de dispositivos que reciben mensajes broadcast.

- Routers separan broadcast domains.

---

## 8.2 Collision Domain

Segmento donde pueden ocurrir colisiones.

- Switches reducen collision domains.
- Hubs no.

---

# 9. Seguridad en LAN

Una LAN mal segmentada es un entorno ideal para:

- Movimiento lateral
- Escaneo interno
- ARP spoofing
- Man-in-the-middle

Buenas prácticas:

- Implementar VLANs
- Aplicar ACLs
- Monitorear tráfico interno
- Utilizar IDS/IPS
- Aplicar principio de mínimo privilegio

---

# 10. Relevancia en Ciberseguridad

Comprender LAN permite:

- Analizar tráfico en Wireshark
- Detectar anomalías internas
- Entender cómo se mueve un atacante
- Diseñar segmentaciones defensivas
- Implementar Zero Trust

---

# Conclusión

La LAN es la base estructural de cualquier infraestructura moderna.

Antes de abordar:

- SOC
- Pentesting
- Threat Hunting
- Arquitectura defensiva

Es obligatorio comprender profundamente:

- Direccionamiento
- Segmentación
- Protocolos
- Flujo de tráfico

Networking no es opcional en ciberseguridad.  
Es la base sobre la cual se construye todo lo demás.

---


