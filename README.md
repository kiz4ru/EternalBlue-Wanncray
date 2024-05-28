# Explotación de EternalBlue para Subir y Ejecutar un Archivo en Windows 7 y Análisis del Ransomware WannaCry

## Introducción

Este proyecto documenta un proceso paso a paso para explotar la vulnerabilidad EternalBlue en una máquina Windows 7. También se incluye un análisis del comportamiento del ransomware WannaCry utilizando INetSim para redirigir peticiones web, Burp Suite para interceptar y analizar dichas peticiones, y btcAnalyzer para investigar las direcciones de Bitcoin asociadas con el ransomware.

## Requisitos

- Máquina atacante: Kali Linux con Metasploit, INetSim, Burp Suite y btcAnalyzer instalados.
- Máquina víctima: Windows 7 sin parche MS17-010 aplicado.
- Ransomware WannaCry.
- Conectividad de red entre la máquina atacante y la víctima.

## Descargas

- [Kali Linux OVA](https://www.kali.org/get-kali/#kali-virtual-machines)
- [Windows 7 OVA](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
- [WannaCry Sample](https://github.com/some-repo/wannacry-sample) (Nota: descarga bajo tu propio riesgo y responsabilidad)

## Configuración del Entorno

### Paso 1: Configurar Kali Linux

1. **Actualizar e instalar Metasploit**:
   ```bash
   sudo apt-get update
   sudo apt-get install metasploit-framework
2. **Instalar INetSim**:
    ```bash
    sudo apt-get install inetsim
3. **Instalar Burp Suite**:
   - Burp Suite ya viene preinstalado en Kali Linux. Si no lo tienes, descárgalo e instálalo desde Burp Suite Community Edition.
4. **Instalar btcAnalyzer**:
   ```bash
   sudo apt-get install python3-pip
   pip3 install btcAnalyzer
### Paso 2: Configurar Windows 7
1. Configurar Red:
  - Asegúrate de que la máquina Windows 7 esté en la misma red que tu Kali Linux.
  - Configura las propiedades de red para usar la IP de Kali como servidor DNS
### Paso 3: Ejecución del Ataque
1. Ejecutar el script de python:
  - python msfEternal.py
2. Seguir los pasos. 

   
   
   
