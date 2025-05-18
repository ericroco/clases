# Documentación Técnica y Funcional del Wireframe de la Aplicación PiensaPlay  
**Tu entrenador en competencia mediática**

---

## **1. Información General**

| Campo | Descripción |
|-------|-------------|
| **Nombre del Proyecto** | PiensaPlay |
| **Subtítulo** | Tu entrenador en competencia mediática |
| **Tipo de Aplicación** | Móvil (iOS/Android) – Versión web futura |
| **Público Objetivo Principal** | Niños y niñas de 8 a 12 años |
| **Versión Futura** | Adolescentes, docentes, familias |
| **Objetivo Principal** | Promover el aprendizaje de habilidades de Alfabetización Mediática e Informacional (AMI) mediante dinámicas lúdicas y educativas |
| **Valores y Conceptos Clave** | Pensamiento crítico, juego y aprendizaje, creatividad, seguridad y responsabilidad digital, diversidad e inclusión, curiosidad |

---

## **2. Estructura Modular de la Aplicación**

La aplicación se organiza en **siete módulos principales**, cada uno con un propósito específico, componentes visuales definidos y funcionalidades asociadas.

| Número | Módulo | Propósito |
|--------|--------|-----------|
| 1 | Pantalla de Bienvenida / Inicio Local | Personalizar la experiencia del usuario sin necesidad de crear cuentas o usar contraseñas |
| 2 | Pantalla de Inicio | Ser el punto de entrada principal de la aplicación, ofreciendo una interfaz amigable y motivadora tras el inicio local |
| 3 | Juegos Educativos | Ofrecer actividades interactivas clasificadas por categorías temáticas para enseñar habilidades AMI de forma divertida |
| 4 | Desafíos Diarios | Proporcionar una actividad breve diaria que refuerce conceptos clave de manera continua y motivadora |
| 5 | Mi Progreso | Permitir al usuario visualizar su avance en distintas áreas y niveles alcanzados, fomentando la motivación y el reconocimiento personal |
| 6 | Glosario de Términos | Facilitar el aprendizaje de nuevo vocabulario relacionado con AMI, con notificaciones inteligentes cuando se introducen nuevos términos en las actividades |
| 7 | Perfil del Usuario | Mostrar información personal básica, permitir la personalización de la experiencia y acceder a opciones básicas de ayuda |

---

## **3. Detalles de Cada Módulo**

### **Módulo 1: Pantalla de Bienvenida / Inicio Local**

#### **Propósito**
Personalizar la experiencia del niño sin necesidad de crear cuentas o usar contraseñas. Se inicia una sesión local basada únicamente en nombre y edad.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Logo animado** | Posible mascota o personaje guía que da la bienvenida visualmente. |
| **"¡Hola! Como te llamas?"** | Mensaje inicial de bienvenida personalizado. |
| **Campo Nombre** | Entrada de texto donde el niño ingresa su nombre. Este dato se usará para personalizar la experiencia. |
| **Campo Edad (8-12)** | Selector numérico o campo editable para elegir la edad entre 8 y 12 años. Ayuda a adaptar el nivel de dificultad. |
| **Selecciona tu avatar** | Galería interactiva de avatares predefinidos. El usuario puede seleccionar uno para representarse en la app. |
| **Botón "jJugar!"** | Acción principal que inicia la navegación hacia la pantalla principal de la aplicación. |
| **Texto informativo:** `"Solo es necesario tu nombre y edad para adaptar la app a ti"` | Justifica la recopilación de datos personales mínimos para ofrecer una experiencia personalizada. |

#### **Consideraciones de Seguridad**
- No se almacenan datos sensibles.
- Sesión local, no requiere conexión ni registro.
- Datos anonimizados si se recopilan estadísticas generales.

#### **Estilo Visual**
- Colores vibrantes y cálidos.
- Tipografía redondeada y legible.
- Iconografía clara y expresiva.
- Uso de mascota guía animada durante carga.

---

### **Módulo 2: Pantalla de Inicio**

#### **Propósito**
Ser el punto de entrada principal de la aplicación, ofreciendo una interfaz amigable y motivadora tras el inicio local.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Logo animado** | Refuerza la identidad visual de la aplicación. |
| **"iHola Sofia! iLista para aprender hoy?"** | Saludo personalizado que motiva al usuario a comenzar. |
| **Acceso rápido a funciones principales** | Botones directos a Juegos Educativos, Desafío del Día y Mi Progreso. |
| **Mini gráfico de progreso semanal** | Visualización sencilla del progreso del niño en la última semana. |
| **Botones secundarios** | Acceso a Ayuda, Glosario y Configuración. |

#### **Estilo Visual**
- Colores vibrantes y cálidos.
- Tipografía redondeada y legible.
- Iconografía clara y expresiva.

---

### **Módulo 3: Juegos Educativos**

#### **Propósito**
Ofrecer actividades interactivas clasificadas por categorías temáticas para enseñar habilidades AMI de forma divertida.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Selector de categoría** | Filtros por Análisis de Contenido, Producción Digital y Seguridad Online. |
| **Rejilla de juegos** | Cada juego tiene miniatura, nombre, nivel de dificultad, descripción breve y estado (bloqueado/completado). |
| **Filtro por edad, dificultad y tema** | Herramientas para encontrar los juegos más adecuados. |
| **Barra de búsqueda** | Permite buscar juegos por palabra clave. |
| **Sugerencias personalizadas** | Recomendaciones según el historial de juegos completados. |

#### **Ejemplos de Juegos**
- **Detective de Fake News**: Identificar noticias falsas mediante ejercicios interactivos.
- **Crea tu propio video seguro**: Enseña buenas prácticas al crear contenido audiovisual.
- **Redes sociales ¿amigas o peligrosas?**: Aprender a navegar responsablemente por redes sociales.

---

### **Módulo 4: Desafíos Diarios**

#### **Propósito**
Proporcionar una actividad breve diaria que refuerce conceptos clave de manera continua y motivadora.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Desafío destacado del día** | Imagen ilustrativa, consigna clara y botón para iniciar. |
| **Historial de desafíos completados** | Registro cronológico de los desafíos realizados previamente. |
| **Recordatorios configurables** | Notificaciones programables para incentivar el uso regular. |
| **Enlaces a recursos complementarios** | Artículos explicativos y videos cortos relacionados con el desafío del día. |

#### **Ejemplos de Desafíos**
- **"¿Cómo sabes si esta noticia es real?"** – Ejercicio de análisis de fuentes.
- **"¿Qué haces si ves contenido inapropiado online?"** – Simulación de situación real.
- **"Diseña tu propia contraseña segura"** – Actividad interactiva sobre seguridad digital.

---

### **Módulo 5: Mi Progreso**

#### **Propósito**
Permitir al usuario visualizar su avance en distintas áreas y niveles alcanzados, fomentando la motivación y el reconocimiento personal.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Gráficos de barras o circulares** | Muestran el porcentaje de juegos completados y niveles alcanzados en cada categoría. |
| **Medallas o insignias ganadas** | Representan logros específicos (ej.: “Comentario respetuoso”). |
| **Historial de juegos y desafíos realizados** | Lista completa de actividades completadas. |
| **Objetivos pendientes** | Muestra qué retos aún no han sido superados. |
| **Resumen semanal/mensual** | Gráficos comparativos del tiempo invertido y avance general. |

#### **Indicadores Clave**
- Total de juegos completados
- Tiempo invertido en la app
- Logros semanales

---

### **Módulo 6: Glosario de Términos**

#### **Propósito**
Facilitar el aprendizaje de nuevo vocabulario relacionado con AMI, con notificaciones inteligentes cuando se introducen nuevos términos en las actividades.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Lista de términos ordenados alfabéticamente** | Fácil acceso y navegación. |
| **Tarjetas de término** | Incluyen icono, palabra y definición sencilla. |
| **Búsqueda por palabra clave** | Campo de texto para encontrar rápidamente un término. |
| **Notificación integrada** | `"¡Nuevo término añadido!"` + mini tarjeta del término. |
| **Modo exploración** | Ver términos por categoría: Medios, Seguridad, Redes sociales, Veracidad. |

#### **Ejemplos de Términos**
- **Fake News**: Noticias falsas.
- **Fuente confiable**: Sitio o persona que ofrece información veraz.
- **Contraseña segura**: Clave difícil de adivinar.
- **Comentario respetuoso**: Opinión sin ofensas.

---

### **Módulo 7: Perfil del Usuario**

#### **Propósito**
Mostrar información personal básica, permitir la personalización de la experiencia y acceder a opciones básicas de ayuda.

#### **Componentes Visuales y Funcionales**

| Elemento | Descripción funcional |
|----------|------------------------|
| **Nombre del usuario** | `Sofia` – Visible en todo momento. |
| **Edad** | `10 años` – Seleccionada durante el registro. |
| **Avatar actual** | Puede cambiarse desde el perfil. |
| **Opciones de personalización** | Idioma, modo claro/oscuro, volumen y efectos sonoros. |
| **Ayuda rápida** | Guía sencilla sobre cómo usar la aplicación. |
| **Cerrar sesión / Reiniciar sesión local** | Útil para compartir dispositivos. |

---

## **4. Barra de Navegación Inferior**

Ubicación: Parte inferior visible en todas las pantallas principales.

| Opción | Descripción funcional |
|-------|------------------------|
| **Inicio** | Vuelve a la pantalla principal de la aplicación desde cualquier otra sección. |
| **Juegos** | Accede a la sección de juegos educativos disponibles, organizados por categoría y dificultad. |
| **Desafios** | Redirige a la lista de desafíos diarios y pendientes. |
| **Progreso** | Muestra estadísticas de aprendizaje del usuario: tiempo invertido, niveles alcanzados, insignias ganadas, etc. |
| **Perfil** | Lleva al perfil del usuario, donde puede configurar opciones personales, revisar historial y cerrar sesión. |

---

## **5. Estilo Visual y Consideraciones Técnicas**

### **Paleta de Colores**
- **Verde (#4CAF50)**: Primario – crecimiento y confianza
- **Naranja (#FF9800)**: Secundario – energía y creatividad
- **Beige (#F5F5F5)**: Fondo – limpieza y calidez
- **Negro (#000000) y Blanco (#FFFFFF)**: Contrastes

### **Tipografía**
- **Fuente principal:** Roboto Rounded (legible y amigable)
- **Tamaños sugeridos:**
  - Títulos: 24px
  - Subtítulos: 18px
  - Texto normal: 16px

### **Iconografía**
- Estilo plano y minimalista
- Ilustraciones expresivas y coloridas
- Uso de mascota guía (ej.: robot curioso o zorro inteligente)

### **Animaciones y Transiciones**
- Transiciones suaves entre pantallas
- Animaciones de recompensa cuando se completa una tarea

### **Accesibilidad**
- Contraste suficiente
- Texto legible
- Soporte para lectores de pantalla

---

## **6. Escalabilidad Futura**

Aunque la versión inicial se enfoca en niños de 8 a 12 años, se prevé ampliar la plataforma a:

- **Adolescentes**: Módulos más complejos y temas como privacidad y redes sociales.
- **Docentes**: Panel de control para asignar actividades y ver reportes de alumnos.
- **Familias**: Contenido compartido y consejos para padres.
- **Plataforma Web**: Complemento de la app móvil con recursos adicionales.

---

## **7. Flujo de Interacción del Usuario**

1. **Registro Inicial:**
   - Nombre
   - Edad
   - Avatar
   - Confirmar con `¡Jugar!`

2. **Inicio:**
   - Ver `Desafio del Dia`
   - Acceder a `Juegos`, `Desafios`, `Progreso` o `Perfil`

3. **Juegos Educativos:**
   - Elegir categoría
   - Buscar juego
   - Comenzar juego

4. **Desafío del Día:**
   - Iniciar desafío
   - Completar actividad
   - Ganar insignia o puntos

5. **Progreso:**
   - Revisar gráficos de avance
   - Explorar sugerencias
   - Consultar logros

6. **Perfil:**
   - Editar datos personales
   - Cambiar configuraciones
   - Reiniciar sesión

7. **Glosario:**
   - Buscar término
   - Añadir nuevo término
   - Repasar definiciones

---