<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

  <h1>Resumen del Taller Raspberry Pi 3</h1>

  <div class="section">
    <h2> Descripción General</h2>
    <p>
      Este documento resume las actividades desarrolladas durante el taller de la <strong>Raspberry Pi 3</strong>,
      donde se exploró el sistema operativo <strong>Raspbian</strong>, la creación de dashboards con <strong>Streamlit</strong> y <strong>Grafana</strong>,
      el uso de <strong>cron y crontab</strong> para la automatización de tareas y la <strong>exploración del entorno de red</strong> con herramientas como <em>nmap</em> y <em>arp</em>.
    </p>
    <p>
      Todas las evidencias visuales del proceso (instalación, dashboards y resultados de red)
      se encuentran anexas en la carpeta <strong>"carpeta de evidencias"</strong> dentro del repositorio de GitHub.
    </p>
  </div>

  <div class="section">
    <h2> Instalación y Manejo de Raspbian</h2>
    <p>
      Se instaló el sistema operativo <strong>Raspberry Pi OS (Raspbian)</strong> utilizando la herramienta
      <em>Raspberry Pi Imager</em>. Tras la instalación, se realizaron configuraciones iniciales de idioma, red WiFi y actualización del sistema.
    </p>
    <p>
      La Raspberry Pi quedó completamente funcional y conectada a la red, sirviendo como base para las siguientes etapas del taller.
    </p>
  </div>

  <div class="section">
    <h2> Dashboard con Streamlit</h2>
    <p>
      Se desarrolló un dashboard sencillo en <strong>Python</strong> utilizando la librería <strong>Streamlit</strong>,
      el cual permite visualizar datos simulados en tiempo real (temperatura, humedad y presión).
      Este dashboard se ejecuta en el navegador mediante la dirección <em>http://localhost:8501</em>.
    </p>
    <p>
      Su propósito fue demostrar la facilidad de generar interfaces interactivas para monitoreo o visualización de datos en sistemas embebidos.
    </p>
  </div>

  <div class="section">
    <h2> Exploración de Grafana</h2>
    <p>
      Se instaló y configuró <strong>Grafana</strong> como herramienta de visualización avanzada. 
      Mediante la fuente de datos integrada <em>TestData DB</em>, se construyó un dashboard de ejemplo con gráficas de línea y gauge.
    </p>
    <p>
      Esta práctica permitió comprender la integración de sistemas de monitoreo en tiempo real dentro de la Raspberry Pi.
      Las capturas del panel de Grafana están disponibles en la carpeta <strong>"carpeta de evidencias"</strong>.
    </p>
  </div>

  <div class="section">
    <h2> Automatización con Cron y Crontab</h2>
    <p>
      Se creó un script de respaldo automático (<em>backup.sh</em>) encargado de comprimir la carpeta <em>Documents</em> diariamente.
      Posteriormente, se programó su ejecución automática mediante <strong>crontab</strong> a las 2:00 a.m. todos los días.
    </p>
    <p>
      Esta sección permitió experimentar con la automatización de procesos dentro del entorno Linux,
      optimizando tareas repetitivas sin intervención manual.
    </p>
  </div>

  <div class="section">
    <h2> Exploración del Entorno de Red</h2>
    <p>
      Se analizaron los aspectos básicos de la red a la cual estaba conectada la Raspberry Pi:
    </p>
    <ul>
      <li>Obtención de la IP local con <code>hostname -I</code>.</li>
      <li>Detección de equipos vecinos usando <code>arp -a</code> y <code>nmap -sn</code>.</li>
      <li>Escaneo de puertos activos en el sistema con <code>nmap -p 1-1024 localhost</code>.</li>
    </ul>
    <p>
      Con esto se logró identificar los dispositivos cercanos, los servicios activos y se comprendió la importancia de una auditoría de red básica.
    </p>
  </div>

  <div class="section">
    <h2> Documento en Overleaf</h2>
    <p>
      Todo el proceso técnico detallado se encuentra documentado en el archivo 
      <strong><em>Taller6.pdf</em></strong>, el cual incluye las explicaciones, códigos y resultados de cada etapa.
      Este archivo está preparado para compilarse en <a href="https://www.overleaf.com" target="_blank">Overleaf</a>.
    </p>
  </div>

  <div class="section">
    <h2> Conclusiones</h2>
    <ul>
      <li>Se configuró exitosamente el sistema operativo Raspbian en la Raspberry Pi 3.</li>
      <li>Se construyó un dashboard funcional con Streamlit y uno complementario con Grafana.</li>
      <li>Se implementó un sistema de automatización de tareas mediante cron y crontab.</li>
      <li>Se exploró el entorno de red, identificando dispositivos, IPs y puertos activos.</li>
      <li>Se comprobó el potencial de la Raspberry Pi como herramienta educativa y de desarrollo en ingeniería electrónica.</li>
    </ul>
  </div>
</body>
</html>
