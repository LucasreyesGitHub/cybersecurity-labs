# Entorno de Laboratorio SOC – Setup

Este documento describe la configuración del entorno de laboratorio
utilizado para el aprendizaje y práctica como Analista SOC (Blue Team).

El objetivo es contar con un entorno reproducible, controlado y alineado
a escenarios reales de monitoreo, detección y análisis.

---

## 🖥️ Máquina de Análisis

### Sistema Operativo
- Kali Linux (rolling / versión estable)

### Rol
- Analista SOC
- Análisis de logs, eventos y alertas
- Investigación de comportamientos sospechosos

### Usuario
- Usuario por defecto: `kali`
- Uso exclusivo para análisis (no productivo)

---

## 💿 Virtualización

- Software: VirtualBox o VMware
- CPU: 2 cores
- Memoria RAM: 4 GB
- Disco: 40 GB

Esta configuración es suficiente para tareas de análisis SOC iniciales.

---

## 🌐 Configuración de Red

- Tipo de red: NAT / Host-only
- Comunicación controlada entre máquinas virtuales
- Sin exposición directa a Internet desde servicios internos

Ejemplo de rango utilizado:
- 192.168.56.0/24 (referencial)

---

## 📁 Directorios relevantes

- `/var/log`  
  Directorio principal de logs del sistema Linux.

- `/etc`  
  Archivos de configuración del sistema.

Estos directorios son clave para tareas de monitoreo y análisis.

---

## 🔐 Consideraciones de Seguridad

- No se utilizan credenciales reales
- No se exponen IPs productivas
- Todos los datos son generados en entorno de laboratorio
- Uso estrictamente educativo

---

## 🎯 Objetivo del Setup

Proveer una base sólida para:
- Aprender fundamentos de SOC
- Analizar logs y eventos
- Simular escenarios de detección
- Documentar procesos de análisis

Las herramientas pueden cambiar, la metodología permanece.
