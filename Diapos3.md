#  **Guía de Estudio: Jerarquía y Organización de Memoria**

##  1. **Jerarquía de Memoria**

###  Niveles de la jerarquía:
1. **Registros del CPU (L0)**  
   - Velocidad máxima.  
   - Muy poca capacidad.  
   - Almacenan datos temporales durante ejecución de instrucciones.

2. **Memoria Caché (L1, L2, L3)**  
   - Memoria rápida entre la CPU y la memoria principal.  
   - Puede estar integrada en el chip del procesador.

3. **Memoria Principal (RAM) (L1 o L2)**  
   - Almacena programas y datos en uso actual.  
   - Volátil (se pierde al apagar).

4. **Memoria Secundaria (L3 o más)**  
   - Disco duro, SSD, etc.  
   - Capacidad alta, velocidad baja.  
   - Permanente (no volátil).

 **Objetivo de la jerarquía**: equilibrar costo, velocidad y capacidad.

---

##  2. **Características de la Memoria**

| Característica | Descripción |
|----------------|-------------|
| **Función** | Memoria interna, caché, principal o secundaria |
| **Tecnología** | Semiconductoras (estáticas/dinámicas), magnéticas, ópticas, emergentes |
| **Volatilidad** | Volátil (RAM), no volátil (ROM, FLASH) |
| **Operación** | Lectura/escritura (RAM), solo lectura (ROM, PROM, EPROM, EEPROM, FLASH) |
| **Método de acceso** | Aleatorio (RAM), secuencial (cintas), directo (discos) |
| **Direccionamiento** | Por posición (dirección específica), por contenido (memorias asociativas) |

---

##  3. **Unidad de Transferencia**

- **Interna**: controlada por el ancho del bus de datos.
- **Externa**: se transfieren bloques grandes de datos.
- **Dirección mínima**: palabra o byte, dependiendo del sistema.

---

##  4. **Organización de la Memoria Principal**

- Se organiza como una **matriz de filas y columnas**.
- Chips pueden ser de tipo:
  - **n x m bits** (más pines)
  - **n x 1 bit** (menos pines)

 Ejemplo:
- Un chip de 8 Mbits puede tener diferentes configuraciones físicas (ej.: 1M x 8, 512K x 16).

---

## 🔹 5. **Memoria Caché**

###  ¿Qué es?
- Memoria pequeña y rápida ubicada entre la CPU y la memoria principal.
- Puede estar dentro del procesador (integrada) o fuera (externa).

###  Funcionamiento básico:
1. La CPU solicita una dirección de memoria.
2. Se verifica si esa información está en la caché.
3. Si está (acceso exitoso): se usa directamente desde la caché.
4. Si no está (fallo de caché): se trae el bloque completo desde la memoria principal a la caché.

---

##  6. **Elementos de Diseño de la Caché**

| Elemento | Descripción |
|---------|-------------|
| **Tamaño de caché** | A mayor tamaño, más espacio pero también más lenta y costosa. |
| **Función de correspondencia** | Asigna bloques de memoria a líneas de caché (directa, asociativa, asociativa por conjuntos) |
| **Algoritmo de sustitución** | Qué bloque reemplazar cuando hay fallo (LRU, FIFO, LFU, aleatorio) |
| **Política de escritura** | Escritura inmediata (write-through) o diferida (write-back) |
| **Tamaño de línea** | Cuántos bytes se transfieren cada vez (ej.: 32, 64 bytes) |
| **Número de niveles de caché** | Caché L1, L2, L3 (cada nivel más grande pero más lento) |
| **Caché unificada vs dividida** | Compartida para instrucciones y datos vs separada |

---

##  7. **Tipos de Correspondencia en Caché**

###  **Correspondencia Directa**
- Cada bloque de memoria va a una única línea de caché.
- Fórmula: `i = j mod m` donde i es línea de caché, j es bloque de memoria, m es número de líneas.
- Ventaja: simple y barato.
- Desventaja: conflictos frecuentes si dos bloques usan misma línea.

###  **Correspondencia Asociativa**
- Cualquier bloque puede ir a cualquier línea.
- Requiere memoria asociativa (costosa).
- Ventaja: menos conflictos.
- Desventaja: alto costo y complejidad.

###  **Correspondencia Asociativa por Conjuntos**
- Compromiso entre las dos anteriores.
- La caché se divide en conjuntos; cada bloque va a un conjunto específico, pero puede estar en cualquiera de sus líneas.
- Ejemplo: caché asociativa de 2 vías → cada conjunto tiene 2 líneas.

---

##  8. **Formato de Dirección en Caché**

Depende del tipo de correspondencia:

| Tipo | Campo 1 | Campo 2 | Campo 3 |
|------|---------|---------|---------|
| **Directa** | Etiqueta | Línea | Palabra |
| **Asociativa** | Etiqueta | — | Palabra |
| **Asociativa por conjuntos** | Etiqueta | Conjunto | Palabra |

 Ejemplo con 24 bits de dirección:
- **Palabra**: 2 bits (bloque de 4 bytes)
- **Etiqueta + Línea/Conjunto**: 22 bits restantes

---

##  9. **Algoritmos de Sustitución de Bloques**

| Algoritmo | Descripción |
|----------|-------------|
| **LRU (Least Recently Used)** | Reemplaza el bloque menos usado recientemente |
| **FIFO (First In First Out)** | Reemplaza el bloque más antiguo |
| **LFU (Least Frequently Used)** | Reemplaza el bloque menos usado en total |
| **Aleatorio** | Elige una línea al azar |

---

##  10. **Políticas de Escritura**

| Política | Descripción |
|---------|-------------|
| **Write Through (Escritura inmediata)** | Escribe en caché y en memoria principal simultáneamente |
| **Write Back (Post-escritura)** | Solo escribe en caché, marca el bloque como “sucio” (dirty bit) y lo escribe en memoria al reemplazarlo |

 Consideraciones:
- Write through es más segura pero genera más tráfico.
- Write back es más rápido pero requiere coherencia en sistemas multiprocesador.

---

##  11. **Memorias ROM, PROM, EPROM, EEPROM, FLASH**

| Tipo | Características |
|------|------------------|
| **ROM** | Contenido grabado en fábrica, no modificable |
| **PROM** | Programable una sola vez |
| **EPROM** | Borrable con luz UV y reprogramable |
| **EEPROM** | Borrable eléctricamente, permite modificar partes específicas |
| **FLASH** | Alternativa a EEPROM, permite borrar bloques completos, más rápida y económica |

---

##  12. **Memoria Estática vs Dinámica (SRAM vs DRAM)**

| Característica | **SRAM** | **DRAM** |
|----------------|----------|----------|
| **Tipo de almacenamiento** | Circuitos de transistores (flip-flop) | Condensador (carga eléctrica) |
| **Velocidad** | Más rápida | Más lenta |
| **Costo** | Más cara | Más barata |
| **Complejidad** | Menos densa | Más densa |
| **Volatilidad** | Sí | Sí |
| **Aplicación típica** | Caché | Memoria principal |

 **Nota importante:** La SRAM no necesita refresco constante, mientras que la DRAM sí.
