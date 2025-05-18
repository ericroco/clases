# Documentación Completa del Wireframe  
## Aplicación PiensaPlay – Tu entrenador en competencia mediática

> **Versión 1.0**  
> *Fecha: 5 de abril de 2025*

---

## 📋 Índice

1. [Información General](#información-general)  
2. [Estructura Modular de la Aplicación](#estructura-modular-de-la-aplicación)  
3. [Módulo 1: Pantalla de Bienvenida / Inicio Local](#módulo-1-pantalla-de-bienvenida--inicio-local)  
4. [Módulo 2: Pantalla de Inicio](#módulo-2-pantalla-de-inicio)  
5. [Módulo 3: Juegos Educativos](#módulo-3-juegos-educativos)  
6. [Módulo 4: Desafíos Diarios](#módulo-4-desafíos-diarios)  
7. [Módulo 5: Mi Progreso](#módulo-5-mi-progreso)  
8. [Módulo 6: Glosario de Términos](#módulo-6-glosario-de-términos)  
9. [Módulo 7: Perfil del Usuario](#módulo-7-perfil-del-usuario)  
10. [Guía de Estilo Visual](#guía-de-estilo-visual)  
11. [Consideraciones Técnicas](#consideraciones-técnicas)  
12. [Escalabilidad Futura](#escalabilidad-futura)

---

## 1. Información General

| Campo | Descripción |
|-------|-------------|
| **Nombre del Proyecto** | PiensaPlay |
| **Subtítulo** | Tu entrenador en competencia mediática |
| **Tipo de Aplicación** | Móvil (iOS/Android) |
| **Público Objetivo Principal** | Niños y niñas de 8 a 12 años |
| **Versión Futura** | Adolescentes, docentes, familias |
| **Objetivo Principal** | Promover el aprendizaje de habilidades de Alfabetización Mediática e Informacional (AMI) mediante dinámicas lúdicas y educativas |
| **Valores y Conceptos Clave** | Pensamiento crítico, juego y aprendizaje, creatividad, seguridad y responsabilidad digital, diversidad e inclusión, curiosidad |

---

## 2. Estructura Modular de la Aplicación

La aplicación se divide en **7 módulos principales**, cada uno con su propósito, componentes visuales y funcionalidades asociadas:

| Número | Módulo | Propósito |
|--------|--------|-----------|
| 1 | Pantalla de Bienvenida / Inicio Local | Personalizar la experiencia del niño sin necesidad de crear cuentas o usar contraseñas |
| 2 | Pantalla de Inicio | Ser el punto de entrada principal de la aplicación |
| 3 | Juegos Educativos | Ofrecer actividades interactivas clasificadas por categorías temáticas para enseñar habilidades AMI de forma divertida |
| 4 | Desafíos Diarios | Proporcionar una actividad breve diaria que refuerce conceptos clave |
| 5 | Mi Progreso | Visualización del avance del usuario |
| 6 | Glosario de Términos | Acceso a definiciones clave y notificaciones de nuevos términos |
| 7 | Perfil del Usuario | Información personal y configuración básica |

---

## 3. Módulo 1: Pantalla de Bienvenida / Inicio Local

### Propósito
Personalizar la experiencia del niño sin necesidad de crear cuentas o usar contraseñas. Se inicia una sesión local basada únicamente en nombre y edad.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Logo animado** | Posible mascota o personaje guía. Mejora la conexión emocional con la app. |
| **"¡Hola! Como te llamas?"** | Mensaje inicial de bienvenida personalizado. Debería usarse una fuente más clara y legible para facilitar la lectura. |
| **Campo Nombre** | Entrada de texto editable donde el niño ingresa su nombre. |
| **Campo Edad (8-12)** | Selector numérico o campo editable. Mejoraría la UX si fuera un selector desplegable con rangos predefinidos. |
| **Selecciona tu avatar** | Galería interactiva de avatares predefinidos. Se recomienda ofrecer opciones diversas e inclusivas (género, etnia, etc.). |
| **Botón "¡Jugar!"** | Acción principal que inicia la navegación hacia la pantalla principal.|
| **Texto informativo:** `"Solo es necesario tu nombre y edad para adaptar la app a ti"` | Justifica la recopilación de datos personales mínimos.` |

### Mejoras Sugeridas
- Corregir errores ortográficos y gramaticales.
- Usar iconografía estándar para campos de formulario (usuario, edad).
- Incluir opción para cambiar idioma desde esta pantalla.
---

## 4. Módulo 2: Pantalla de Inicio

### Propósito
Ser el punto de entrada principal de la aplicación, ofreciendo una interfaz amigable y motivadora tras el inicio local.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Logo animado** | Refuerza la identidad visual de la aplicación. |
| **"¡Hola Sofia! ¿Lista para aprender hoy?"** | Saludo personalizado. |
| **Acceso rápido a funciones principales** | Botones directos a Juegos Educativos, Desafío del Día y Mi Progreso. |
| **Mini gráfico de progreso semanal** | Visualización sencilla del progreso del niño en la última semana. Mejora la motivación al ver avances. |
| **Botones secundarios** | Acceso a Ayuda, Glosario y Configuración. |

### Mejoras Sugeridas
- Incluir una imagen o ícono representativo del desafío del día.
- Mostrar tiempo estimado de completación del desafío diario.
- Agregar tutorial interactivo para usuarios nuevos.

---

## 5. Módulo 3: Juegos Educativos

### Propósito
Ofrecer actividades interactivas clasificadas por categorías temáticas para enseñar habilidades AMI de forma divertida.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Selector de categoría** | Filtros por Análisis de Contenido, Producción Digital y Seguridad Online. |
| **Rejilla de juegos** | Cada juego tiene miniatura, nombre, nivel de dificultad, descripción breve y estado (bloqueado/completado). |
| **Filtro por edad, dificultad y tema** | Herramientas para encontrar los juegos más adecuados. |
| **Barra de búsqueda** | Permite buscar juegos por palabra clave. |
| **Sugerencias personalizadas** | Recomendaciones según el historial de juegos completados. |

### Ejemplos de Juegos
- **Detective de Fake News**: Identificar noticias falsas mediante ejercicios interactivos.
- **Crea tu propio video seguro**: Enseña buenas prácticas al crear contenido audiovisual.
- **Redes sociales ¿amigas o peligrosas?**: Aprender a navegar responsablemente por redes sociales.

### Mejoras Sugeridas
- Incluir descripciones breves de los objetivos pedagógicos de cada juego.
- Mostrar el tiempo promedio necesario para completar cada juego.
- Permitir que los niños den calificaciones o comentarios sobre los juegos.
- Añadir modo multijugador local o por turnos para fomentar el trabajo colaborativo.

---

## 6. Módulo 4: Desafíos Diarios

### Propósito
Proporcionar una actividad breve diaria que refuerce conceptos clave de manera continua y motivadora.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Desafío destacado del día** | Imagen ilustrativa, consigna clara y botón para iniciar. |
| **Historial de desafíos completados** | Registro cronológico de los desafíos realizados previamente. |
| **Recordatorios configurables** | Notificaciones programables para incentivar el uso regular. |
| **Enlaces a recursos complementarios** | Artículos explicativos y videos cortos relacionados con el desafío del día. |

### Ejemplos de Desafíos
- **"¿Cómo sabes si esta noticia es real?"** – Ejercicio de análisis de fuentes.
- **"¿Qué haces si ves contenido inapropiado online?"** – Simulación de situación real.
- **"Diseña tu propia contraseña segura"** – Actividad interactiva sobre seguridad digital.

### Mejoras Sugeridas
- Agregar opción de repetir el desafío con nuevos contenidos.
- Mostrar retroalimentación inmediata al finalizar el desafío.
- Incluir sistema de recompensas simbólicas (ej.: puntos, insignias).
- Permitir compartir resultados con padres/tutores (opcional y con consentimiento).

---

## 7. Módulo 5: Mi Progreso

### Propósito
Permitir al usuario visualizar su avance en distintas áreas y niveles alcanzados, fomentando la motivación y el reconocimiento personal.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Gráficos de barras o circulares** | Muestran el porcentaje de juegos completados y niveles alcanzados en cada categoría. |
| **Medallas o insignias ganadas** | Representan logros específicos (ej.: “Comentario respetuoso”). |
| **Historial de juegos y desafíos realizados** | Lista completa de actividades completadas. |
| **Objetivos pendientes** | Muestra qué retos aún no han sido superados. |
| **Resumen semanal/mensual** | Gráficos comparativos del tiempo invertido y avance general. |

### Indicadores Clave
- Total de juegos completados
- Tiempo invertido en la app
- Logros semanales

### Mejoras Sugeridas
- Incluir metas personalizables (ej.: “Completa 3 juegos esta semana”).
- Agregar opción de exportar el progreso (PDF o CSV).
- Mostrar recomendaciones de juegos según áreas de mejora.
- Integrar sistema de niveles (nivel 1, nivel 2, etc.) para hacerlo más gamificado.

---

## 8. Módulo 6: Glosario de Términos

### Propósito
Facilitar el aprendizaje de nuevo vocabulario relacionado con AMI, con notificaciones inteligentes cuando se introducen nuevos términos en las actividades.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Lista de términos ordenados alfabéticamente** | Fácil acceso y navegación. |
| **Tarjetas de término** | Incluyen icono, palabra y definición sencilla. |
| **Búsqueda por palabra clave** | Campo de texto para encontrar rápidamente un término. |
| **Notificación integrada** | `"¡Nuevo término añadido!"` + mini tarjeta del término. |
| **Modo exploración** | Ver términos por categoría: Medios, Seguridad, Redes sociales, Veracidad. |

### Ejemplos de Términos
- **Fake News**: Noticias falsas.
- **Fuente confiable**: Sitio o persona que ofrece información veraz.
- **Contraseña segura**: Clave difícil de adivinar.
- **Comentario respetuoso**: Opinión sin ofensas.

### Mejoras Sugeridas
- Incluir imágenes o ejemplos visuales junto a cada definición.
- Agregar opción de escuchar la pronunciación de los términos.
- Permitir que los niños creen sus propias tarjetas de memoria.
- Vincular términos al glosario desde los juegos y desafíos.

---

## 9. Módulo 7: Perfil del Usuario

### Propósito
Mostrar información personal básica, permitir la personalización de la experiencia y acceder a opciones básicas de ayuda.

### Componentes Visuales y Funcionales

| Elemento | Descripción funcional |
|----------|------------------------|
| **Nombre del usuario** | `Sofia` – Visible en todo momento. |
| **Edad** | `10 anos` – Seleccionada durante el registro. |
| **Avatar actual** | Puede cambiarse desde el perfil. |
| **Opciones de personalización** | Idioma, modo claro/oscuro, volumen y efectos sonoros. |
| **Ayuda rápida** | Guía sencilla sobre cómo usar la aplicación. |
| **Cerrar sesión / Reiniciar sesión local** | Útil para compartir dispositivos. |

### Mejoras Sugeridas
- Agregar opción de cambiar el avatar sin salir del perfil.
- Incluir resumen rápido del progreso dentro del perfil.
- Mostrar tutorial de ayuda contextual según el módulo actual.
- Agregar opción de restablecer progreso (con confirmación).

---

## 10. Guía de Estilo Visual

### Paleta de Colores
- Verde (#4CAF50): Primario – crecimiento y confianza
- Naranja (#FF9800): Secundario – energía y creatividad
- Beige (#F5F5F5): Fondo – limpieza y calidez
- Negro (#000000) y Blanco (#FFFFFF): Contrastes

### Tipografía
- Fuente principal: Roboto Rounded (legible y amigable)
- Tamaños sugeridos:
  - Títulos: 24px
  - Subtítulos: 18px
  - Texto normal: 16px

### Iconografía
- Estilo plano y minimalista
- Ilustraciones expresivas y coloridas
- Uso de mascota guía (ej.: robot curioso o zorro inteligente)

---

## 11. Consideraciones Técnicas

- **Responsive Design:** Compatible con móviles, tablets y navegadores web.
- **Accesibilidad:**
  - Contraste suficiente
  - Texto legible
  - Soporte para lectores de pantalla
- **Animaciones simples:**
  - Transiciones suaves entre pantallas
  - Animaciones de recompensa cuando se completa una tarea
- **Sin distracciones externas:** No incluir publicidad ni enlaces a redes sociales

---

## 12. Escalabilidad Futura

Aunque la versión inicial se enfoca en niños de 8 a 12 años, se prevé ampliar la plataforma a:

- **Adolescentes:** Módulos más complejos y temas como privacidad y redes sociales.
- **Docentes:** Panel de control para asignar actividades y ver reportes de alumnos.
- **Familias:** Contenido compartido y consejos para padres.
- **Plataforma Web:** Complemento de la app móvil con recursos adicionales.
