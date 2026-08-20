# Josue_Herrera_Electica_2026_C2
Repositorio Electíva Diseño Mecatrónico 2026-C2 
# PLC4UNI - Modelo NIVARA GC1

**PLC4UNI** es un Controlador Lógico Programable (PLC) modular, de código abierto y diseño robusto, creado específicamente como una plataforma didáctica para la enseñanza de mecatrónica y automatización. 

Este proyecto permite a los estudiantes interactuar con circuitos industriales reales manteniendo la seguridad del núcleo de procesamiento mediante aislamiento optoacoplado. El sistema está basado en el microcontrolador ESP32-S3.

## ¿En qué consiste el proyecto?
El proyecto abarca todo el ciclo de desarrollo de producto (basado en la norma IEEE-830 STD), incluyendo:
*   **Diseño Electrónico:** Esquemáticos y placa de circuito impreso (PCB) con entradas aisladas (24V DC), salidas a transistores de potencia/relé y puertos analógicos protegidos.
*   **Diseño Mecánico:** Carcasas personalizadas (superior e inferior) optimizadas para manufactura local mediante impresión 3D.
*   **Firmware/Software:** Código base de control que opera mediante un *Scan Cycle* de lazo cerrado (menor a 10ms) para garantizar el determinismo en tiempo real durante las prácticas.

## Programas Utilizados
Para visualizar, editar o compilar los archivos de este repositorio, se utilizaron las siguientes herramientas:
*   **[KiCad](https://www.kicad.org/):** Para el diseño esquemático, enrutamiento de la PCB y visualización 3D electrónica (`.kicad_sch`, `.kicad_pcb`).
*   **[FreeCAD](https://www.freecadweb.org/):** Para el diseño mecánico y modelado tridimensional de las carcasas (`.FCStd`).
*   **[Arduino IDE](https://www.arduino.cc/en/software) / [PlatformIO](https://platformio.org/):** Entornos de desarrollo para la programación del firmware en C/C++.
*   **Git:** Para el control de versiones de todo el proyecto.

## ¿Qué necesitas descargar e instalar?
Para trabajar con este proyecto en tu propia máquina, sigue estos pasos:

### 1. Clonar el repositorio
```bash
git clone https://github.com/JosueHerrera05/Josue_Herrera_Electica_2026_C2.git
```

### 2. Software Requerido
*   Instala **KiCad** (versión 7 o superior recomendada) si deseas editar las pistas, modificar los esquemas eléctricos o ver los modelos 3D de la placa.
*   Instala **FreeCAD** si necesitas modificar el diseño del chasis para ajustarlo a tu impresora 3D.
*   Instala el entorno de programación de tu preferencia (**Arduino IDE** o VSCode + **PlatformIO**) para cargar programas al PLC.

### 3. Dependencias de Hardware (Drivers y Librerías)
*   **Controlador USB-Serial:** Descarga e instala los drivers CH340 o CP2102 (según el módulo puente utilizado en tu placa) para que tu PC reconozca el PLC al conectarlo por cable USB.
*   **Gestor de Tarjetas ESP32:** Si usas Arduino IDE, debes instalar el paquete de tarjetas de Espressif (*esp32 by Espressif Systems*) desde el Gestor de Tarjetas para poder compilar y subir código al procesador ESP32-S3-WROOM-1.

## Estructura del Repositorio
*   `/CAD/`: Archivos de diseño mecánico y modelado 3D para la carcasa (FreeCAD).
*   `/PLC Electiva/`: Archivos del proyecto electrónico (KiCad), incluyendo esquemáticos, footprints y PCB.
*   `/Documentacion/`: Ensayos, manuales, reglamentos de seguridad y el documento oficial de especificaciones de requisitos (IEEE-830).
*   `/PLC4UNI/`: Directorio que contiene datasheets, referencias y archivos complementarios para la manufactura.

## Autores
*   **Desarrollo, Programación y Diseño:** Josue Stalin Herrera Valdez
*   **Dirección de Proyecto:** Carlos Pichardo
*   **Institución:** Instituto Tecnológico de Las Américas (ITLA) - Tecnólogo en Mecatrónica
