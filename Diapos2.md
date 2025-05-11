#  **Guía de Estudio: Plataformas de Procesamiento – FPGA, Microcontroladores y Procesadores**

---

##  1. **Tipos de Plataformas de Procesamiento**

###  **Procesador (Microprocessor)**
- Esencialmente es la **CPU de una computadora**.
- Ejecuta instrucciones secuenciales de un programa.
- Basado en la **arquitectura de Von Neumann**.
- Diseñado para **uso general**: computadoras, servidores, dispositivos móviles.
- No incluye memoria ni periféricos; estos deben conectarse externamente.

####  Componentes típicos:
- **Unidad Aritmético-Lógica (ALU)**
- **Unidad de Control (CU)**
- **Registros internos**
- **Memoria caché**
- **Controladores de bus**
- **Interfaces de entrada/salida (I/O)**

####  Ejemplos:
- Intel Core i9
- AMD Ryzen
- ARM Cortex-A series

---

###  **Microcontrolador (Microcontroller)**
- Un circuito integrado programable que contiene:
  - CPU
  - Memoria (RAM, ROM/Flash)
  - Periféricos (timers, puertos I/O, ADC/DAC, etc.)
- Programado para realizar **funciones específicas**.
- Basado en arquitecturas como **Harvard o Princeton** (Von Neumann).
- Ideal para sistemas embebidos con requisitos específicos.

####  Características:
- **Autónomo**: no requiere componentes externos adicionales.
- Diseño compacto, bajo consumo.
- Uso común en electrodomésticos, automoción, sensores, drones, etc.

####  Ejemplos:
- **Atmel AVR**: ATmega1609, ATmega328P (usado en Arduino)
- **PIC Microcontrollers** de Microchip
- **STM32** de STMicroelectronics

####  Aplicaciones comunes:
- Sistemas de control industrial
- Automatización del hogar
- Dispositivos médicos portátiles
- Interfaces de usuario simples

---

###  **FPGA (Field Programmable Gate Array)**
- **No es un procesador tradicional**.
- Es un **circuito lógico programable** que se puede configurar para implementar cualquier función digital.
- Se programa mediante **lenguajes de descripción de hardware (HDL)** como **VHDL** o **Verilog**.
- Puede simular el comportamiento de un **procesador o microcontrolador**, pero no ejecuta programas como tal.

####  Características:
- **Paralelismo natural**: múltiples operaciones simultáneas.
- **Reconfigurable**: puede cambiar su funcionalidad tras la fabricación.
- No depende de un conjunto fijo de instrucciones.
- Muy flexible, pero requiere conocimientos en diseño digital y síntesis lógica.

####  Ejemplos:
- **Xilinx Spartan**
- **Intel (Altera) Cyclone**
- **Lattice MachXO**

####  Aplicaciones comunes:
- Comunicaciones de alta velocidad
- Procesamiento de señales digitales (DSP)
- Sistemas militares y aeroespaciales
- Prototipado de ASICs
- Visión artificial, robótica avanzada

---

##  2. **Comparación entre las tres plataformas**

| Característica | **Procesador** | **Microcontrolador** | **FPGA** |
|----------------|----------------|-----------------------|----------|
| Tipo de dispositivo | CPU sola | Sistema completo en chip | Circuito lógico reprogramable |
| Arquitectura típica | Von Neumann | Harvard / Von Neumann | Hardware personalizado |
| Lenguaje de programación | C/C++, ensamblador | C, ensamblador, Basic | VHDL, Verilog |
| Paralelismo | Bajo (ejecución secuencial) | Limitado | Alto (operaciones paralelas nativas) |
| Flexibilidad | Media | Alta | Máxima |
| Consumo energético | Alto | Medio-Bajo | Alto (dependiendo de la carga) |
| Costo | Medio-Alto | Bajo-Medio | Alto |
| Aplicaciones típicas | PC, servidores, smartphones | Sistemas embebidos | Sistemas críticos, prototipado, DSP |

---

##  3. **Diferencia entre FPGA y ASIC**

| Concepto | **FPGA** | **ASIC** |
|---------|-----------|-----------|
| Significado | Field Programmable Gate Array | Application Specific Integrated Circuit |
| Reconfigurable | Sí | No |
| Costo inicial | Bajo (sin diseño físico) | Alto |
| Velocidad | Menor que ASIC | Alta |
| Consumo de energía | Alto (dinámico) | Optimizable |
| Tiempo de desarrollo | Corto | Largo |
| Aplicación | Prototipado, flexibilidad | Producción masiva, funciones fijas |

 **Nota:** Los FPGAs son ideales para prototipar circuitos antes de convertirlos en ASICs.

---

##  4. **Arquitectura Interna de un FPGA**

###  Bloques principales:
1. **Logic Blocks (Bloques Lógicos):**
   - Implementan funciones lógicas básicas.
   - Pueden contener tablas de verdad (Look-Up Tables - LUTs).

2. **Programmable Interconnects (Interconexiones Programables):**
   - Permiten conectar bloques lógicos entre sí según la necesidad del diseño.

3. **Input/Output Blocks (IOBs):**
   - Gestionan la comunicación con dispositivos externos.
   - Configurables para diferentes niveles de voltaje y protocolos.

4. **Memoria Embebida (Block RAM, Distributed RAM):**
   - Almacenamiento local dentro del FPGA para datos o instrucciones.

5. **DSP Slices:**
   - Bloques dedicados a operaciones matemáticas complejas (multiplicación, suma, filtrado).

6. **Clock Management Tiles:**
   - Gestión de señales de reloj (PLLs, DLLs).

---

##  5. **Ciclo de Desarrollo en FPGA**

1. **Diseño RTL (Register Transfer Level):**
   - En lenguaje VHDL o Verilog.

2. **Síntesis:**
   - Conversión del código HDL a una red de compuertas lógicas.

3. **Mapeo (Mapping):**
   - Asignación de las compuertas al hardware específico del FPGA.

4. **Colocación y Ruteo (Place and Route):**
   - Determina cómo se colocan los bloques y se conectan físicamente.

5. **Generación del bitstream:**
   - Archivo binario que configura el FPGA.

6. **Implementación y prueba:**
   - Carga del bitstream y verificación del funcionamiento.

---

##  6. **Aplicaciones por Sector**

| Sector | Porcentaje de uso | Ejemplos |
|--------|--------------------|----------|
| **Comunicaciones** | 42% | Redes inalámbricas, fibra óptica, routers |
| **Consumo** | 18% | Dispositivos móviles, wearables, consolas |
| **Automotriz** | 3% | Sistemas ADAS, sensores, infotenimiento |
| **Industrial** | 18% | Control de máquinas, automatización |
| **Defensa/Aeroespacial** | 6% | Sistemas de radar, aviónica, misiles |
| **Test y Medición** | 13% | Osciloscopios, analizadores lógicos |

---

##  7. **Ejemplo de Plataforma FPGA**

###  **Xilinx Spartan-6**
- Serie económica para aplicaciones educativas e industriales.
- Soporta interfaces como SPI, UART, Ethernet.
- Uso común en proyectos de aprendizaje y prototipado rápido.

###  **Genesys 2 (Basado en Xilinx Kintex-7)**
- FPGA de alto rendimiento.
- Memoria DDR3, interfaces HDMI, USB, Ethernet.
- Ideal para investigación y proyectos avanzados.

---

##  8. **Ventajas y Desventajas**

| Ventajas | Desventajas |
|----------|--------------|
| Alta flexibilidad | Curva de aprendizaje pronunciada |
| Capacidad de reconfiguración | Mayor consumo energético |
| Paralelismo real | Costo elevado comparado con MCUs |
| Útil para prototipado | Requiere herramientas de diseño especializadas |

---

##  9. **Términos Clave**

- **Von Neumann**: Arquitectura donde programa y datos comparten memoria.
- **Harvard**: Arquitectura separada para instrucciones y datos.
- **RTL (Register Transfer Level)**: Nivel de abstracción para diseñar circuitos digitales.
- **Bitstream**: Archivo de configuración para programar un FPGA.
- **LUT (Look-Up Table)**: Elemento básico para implementar funciones lógicas en FPGAs.
- **HDL (Hardware Description Language)**: Lenguaje como VHDL o Verilog.
- **ASIC**: Circuito integrado para aplicación específica.
- **Prototipo**: Versión preliminar de un sistema, muchas veces desarrollada en FPGA.
