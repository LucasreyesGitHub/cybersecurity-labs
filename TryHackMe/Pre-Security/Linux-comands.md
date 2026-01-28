# ==============================
# Navegación del sistema de archivos
# ==============================

pwd                         # Muestra el directorio actual de trabajo
ls -l                       # Lista archivos con permisos, propietario y tamaño
cd /var/log                 # Accede al directorio donde se almacenan logs del sistema

# ==============================
# Usuarios y permisos
# ==============================

whoami                      # Muestra el usuario actual
ls -l archivo.txt           # Verifica permisos de un archivo
chmod 644 archivo.txt       # Asigna permisos seguros (rw-r--r--)
sudo comando                # Ejecuta un comando con privilegios elevados

# ==============================
# Acceso remoto
# ==============================

ssh usuario@192.168.1.10    # Conexión remota segura a un servidor Linux mediante SSH

# ==============================
# Gestión de procesos
# ==============================

ps aux                      # Lista todos los procesos en ejecución
top                         # Monitorea procesos y consumo de recursos en tiempo real
kill 1234                   # Finaliza un proceso usando su PID

# ==============================
# Logs del sistema
# ==============================

cat /var/log/auth.log       # Muestra intentos de login y uso de sudo
cat /var/log/syslog         # Muestra eventos generales del sistema

# ==============================
# Gestión de paquetes
# ==============================

sudo apt update             # Actualiza la lista de paquetes disponibles
sudo apt install nmap       # Instala una herramienta común en ciberseguridad

# ==============================
# Automatización
# ==============================

crontab -e                  # Edita tareas programadas (cron jobs)

# ==============================
# Descarga y transferencia de archivos
# ==============================

wget https://example.com/archivo     # Descarga archivos desde Internet
scp archivo.txt usuario@192.168.1.10:/ruta/destino  # Copia archivos de forma segura vía SSH

# ==============================
# Editores de texto
# ==============================

nano archivo.txt            # Editor de texto simple en terminal
vim archivo.txt             # Editor de texto avanzado usado en servidores
