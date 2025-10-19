# backup-linux-azure
# Backup de Linux a Azure Blob Storage

Este proyecto muestra cómo automatizar la copia de seguridad de un sistema Linux y su carga a un contenedor en **Azure Blob Storage**.

Implementado en mi laboratorio personal para practicar integración entre entornos locales y la nube.

## Características
- Genera backups comprimidos de directorios.
- Sube automáticamente los archivos a un contenedor de Azure Blob Storage.
- Permite programar la ejecución mediante cron.

Contenido
- `docs/procedimiento-backup-linux-azure.pdf`: Guía paso a paso.
- `scripts/`: Scripts de respaldo y carga.
- `examples/`: Archivos de ejemplo de configuración.

## Requisitos
- Linux (probado en Ubuntu/Debian)
- azure-cli instalado
- Claves de acceso a Azure Storage

## Uso
1. Configurar las variables en `examples/ejemplo-configuracion.env`
2. Ejecutar el script de respaldo:
   ```bash
   bash scripts/backup.sh
