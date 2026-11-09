# Design System: [Nombre de la Nutricionista] | Nutrición Clínica Pediátrica y Adultos

## 1. Visual Theme & Atmosphere

**Sensación general:** Cálida, tranquilizadora y confiable, con una suavidad delicada en tonos lila y morado.

**Densidad visual:** Moderadamente aireada; mucho espacio en blanco alrededor de titulares grandes y fotografía, con bloques de contenido fáciles de leer y de recorrer.

**Postura de marca:** Profesional, empática y cercana. Una guía de confianza para familias y adultos, con respaldo académico sólido, sin sonar fría ni clínica. Especialmente sensible con temas delicados (selectividad alimentaria, trastornos de conducta alimentaria, niños con necesidades especiales de salud).

**Motivos distintivos:** Neutros lavanda muy claros, botones redondeados tipo píldora, titular de display expresivo tipo script, fotografía orgánica y cálida, frases tipo marquesina repetidas.

### Características clave
- Paleta cálida y serena de lilas y morados sobre fondo lavanda muy claro
- Tipografía display grande y expresiva combinada con una sans-serif simple para el texto
- Controles redondeados y amigables, superficies calmadas de bajo contraste
- Imágenes de bienestar, familia y alimentación cotidiana como apoyo emocional y credibilidad

---

## 2. Color Palette & Roles

| Rol | Nombre semántico | Valor | Uso |
| --- | --- | --- | --- |
| Acción primaria | Morado Ciruela | `#6B4A9E` | Botones primarios, llamados a la acción clave, énfasis de marca |
| Acento | Lila Suave | `#D9C9F0` | Acento sutil, enlaces, resaltados claros, bloques de apoyo |
| Superficie | Lavanda Bruma | `#F8F4FC` | Fondo de página y superficies principales de contenido |
| Texto | Carbón Violeta | `#1B1620` | Titulares, texto de cuerpo, bordes y texto de contraste |
| Borde | Carbón Violeta | `#1B1620` | Bordes de inputs, contornos de botones secundarios, divisores |

### Primario
- `#6B4A9E` como color de acción principal para CTAs y énfasis de marca (contraste con texto `#F8F4FC` ≈ 6.5:1, cumple AA)
- `#D9C9F0` como acento de apoyo para enlaces, etiquetas y momentos de resaltado suave

### Interactivo
- Los enlaces usan el tono lila o el carbón con decoración mínima; sobre fondo claro, preferir carbón subrayado sutil o morado para asegurar contraste
- El foco y los contornos se apoyan en el carbón violeta para dar contraste
- Los estados hover son sutiles (leve oscurecimiento del morado a `#5B3D89`), coherentes con un sistema de movimiento mínimo

### Escala neutra
- Lavanda Bruma (`#F8F4FC`) es el neutro principal de fondo
- Carbón Violeta (`#1B1620`) es el neutro oscuro principal para texto y bordes
- La paleta es intencionalmente comprimida, con pocos grises más allá de estos neutros cálidos

### Superficie y overlay
- Token de superficie: Lavanda Bruma (`#F8F4FC`)
- Token de bloque alterno (secciones destacadas, tarjetas de servicio): Lila Suave al 35–40 % de opacidad sobre la superficie
- Overlay: sin token explícito; si se usa, debe ser sutil y de tono lila

### Modos de tema
El sistema está pensado para esquema de color claro.

**Modo claro**
- Fondo: `#F8F4FC`
- Superficie: `#F8F4FC`
- Texto: `#1B1620`
- Acento: `#6B4A9E`
- Notas: superficies aireadas y de bajo contraste con texto oscuro para máxima legibilidad.

**Modo oscuro:** no definido; no asumir que existe.

### Sombras y profundidad
- Tratamiento de borde/anillo: mínimo o ninguno; la separación visual depende más del contraste de color que de la elevación
- Sombras de tarjeta: no se usan en botones ni inputs
- Foco: anillo oscuro claro en carbón violeta; evitar brillos o glow intensos

---

## 3. Typography Rules

### Familia tipográfica
- **Primaria:** Halcom
- **Monoespaciada:** Base-Mono-Wide
- **Características OpenType:** ninguna explícita; los titulares display son más estilizados y expresivos que el cuerpo

### Jerarquía

| Rol | Fuente | Tamaño | Peso | Notas |
| --- | --- | --- | --- | --- |
| Titular hero | Carefree | 80px | Regular/Display | Titulares grandes y emocionales de portada |
| Título de sección | Carefree | 65px | Regular/Display | Títulos de sección principales y frases de marca |
| Cuerpo | Halcom | 17.6px | Regular | Texto de párrafo principal |
| Etiqueta / Eyebrow | Halcom | — | Regular/Semibold | Texto pequeño introductorio y entradas de sección |
| Caption / Meta | Halcom o Base-Mono-Wide | — | Regular | Iniciales de autor, datos de credenciales, texto de apoyo pequeño |

### Principios
- La tipografía display es expresiva y cálida, no corporativa ni geométrica
- El cuerpo se mantiene simple y muy legible para sostener una experiencia de consulta y bienestar
- El fuerte contraste de estilo entre títulos y cuerpo es la firma de la marca
- La monoespaciada es un estilo utilitario de apoyo para metadatos (por ejemplo, años, títulos académicos)

---

## 4. Component Stylings

### Botones y enlaces
- **CTA primario:** botón píldora relleno en Morado Ciruela (`#6B4A9E`) con texto Lavanda Bruma (`#F8F4FC`). Etiquetas: "AGENDAR HORA"
- **CTA de WhatsApp:** botón píldora relleno o con contorno, con ícono de WhatsApp discreto; etiqueta "ESCRIBIR POR WHATSAPP". Mantener el morado de marca (no usar el verde de WhatsApp)
- **CTA secundario:** botón transparente con borde y texto en Carbón Violeta
- **Enlaces de texto:** discretos, en carbón o morado, con decoración mínima
- **Hover/active:** retroalimentación contenida, sin movimiento juguetón

### Tarjetas y contenedores
- **Estilo de superficie:** limpio, plano y suave con fondos lavanda
- **Radio:** redondeado; botones con radio de píldora extremo, radio general muy pequeño
- **Borde:** línea fina oscura en inputs y controles secundarios
- **Sombra o elevación:** generalmente ausente; composición plana
- **Espaciado interno:** cómodo y abierto, apto para lectura y secciones apiladas

### Inputs y controles interactivos
- Fondo transparente, borde oscuro, texto oscuro
- Foco: énfasis sutil en carbón, sin glow
- Estados de selección: suaves y coherentes con la marca (relleno lila suave)

### Navegación
- Simple y discreta: texto oscuro sobre fondo claro, integrada a la página, sin barra pesada
- Ítems sugeridos: Inicio · Áreas de atención · Sobre mí · Formación · Contacto
- CTA "AGENDAR HORA" como píldora a la derecha
- En móvil: menú colapsado y botón de WhatsApp siempre accesible (flotante discreto)

### Tratamiento de imágenes
- Fotografía orgánica, de estilo de vida y bienestar, en tonos naturales y suaves (mesa familiar, alimentos reales, retrato cercano de la profesional)
- Imágenes limpias, sin marco; el redondeo, si existe, es sutil
- Evitar imágenes centradas en el cuerpo, la balanza o el "antes y después"; privilegiar alimentos, rutinas y momentos cotidianos
- Al mostrar niños, usar solo imágenes con consentimiento o material de banco apropiado

### Componentes distintivos
- **Marquesina** de frases repetidas, por ejemplo: "NUTRICIÓN CON SENTIDO", "COMER SIN MIEDO", "CADA CUERPO, SU RITMO"
- **Bloques de servicio** con íconos tipo sticker y un enlace corto de acción (ver sección de contenido)
- **Línea de credenciales**: lista de títulos con año/institución en estilo meta
- **Testimonios** (solo reales y con autorización): cita grande con iniciales
- **Sección de contacto/agenda**: invitación cálida con botones de Encuadrado y WhatsApp

---

## 5. Layout Principles

### Sistema de espaciado
- Unidad base: 4px
- Valores repetidos: 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

### Grilla y contenedor
- Lógica: narrativa de una sola columna con módulos apilados y ocasional imagen en pareja
- Ancho máximo de contenido: centrado y limitado para lectura (~1120px; texto ~640–720px)
- Espaciado entre secciones: generoso

### Filosofía de espacio en blanco
- El espacio suaviza la página y preserva un tono calmado que genera confianza
- Alineación: bloques centrados o alineados a la izquierda con fuerte ritmo vertical
- Bloques de texto relativamente angostos para lectura cómoda

### Escala de radio de borde
- Micro: 2px
- Estándar: 23px para inputs
- Grande: uso esporádico
- Píldora: 300px para botones primarios y secundarios

---

## 6. Depth & Elevation

| Nivel | Tratamiento | Uso |
| --- | --- | --- |
| Plano | Sin sombra, superficies lavanda planas | Página y secciones de contenido |
| Anillo | Borde carbón oscuro | Inputs, contornos, botón secundario |
| Tarjeta | Tarjeta plana o con marco mínimo, a veces con fondo lila suave | Bloques de servicio, credenciales, testimonios |
| Foco | Anillo o borde oscuro de alto contraste | Estados de teclado e interacción |

### Principios de profundidad
- La jerarquía se transmite con espaciado, escala tipográfica y contraste de color, no con sombras
- Sin desenfoque, vidrio ni overlays
- La profundidad se evita a favor de una claridad editorial y calmada

---

## 7. Do's and Don'ts

### Do
- Usar neutros lavanda cálidos con el morado ciruela como primario y el lila como apoyo
- Mantener los CTAs en forma de píldora y bien diferenciados (relleno vs. contorno)
- Combinar titulares expresivos con cuerpo simple y legible
- Usar lenguaje inclusivo, empático y sin juicio sobre el peso o la alimentación
- Mantener siempre visibles las vías de contacto: Encuadrado y WhatsApp

### Don't
- No introducir neones, azules fríos ni degradados saturados
- No usar sombras pesadas, glassmorphism ni efectos brillantes
- No hacer botones angulares ni demasiado técnicos
- No usar morados muy oscuros o muy saturados como fondo de grandes superficies
- No incluir promesas de resultados, fotos de "antes y después", cifras de peso ni lenguaje que estigmatice (especialmente en TCA y obesidad infantil)

---

## 8. Responsive Behavior

### Breakpoints

| Nombre | Ancho | Cambios clave |
| --- | --- | --- |
| Mobile | Hasta ~767px | Apilar contenido, reducir escala de titulares, mantener espaciado generoso |
| Tablet | ~768px a 1023px | Secciones apiladas con dos columnas ocasionales |
| Desktop | 1024px en adelante | Tipografía display más grande, imágenes más amplias, más aire entre secciones |

### Touch targets
- Elementos interactivos cómodamente grandes y en forma de píldora
- Padding vertical amplio en enlaces y botones (mínimo 44px de alto)

### Estrategia de colapso
- **Desktop:** diseño editorial por secciones con fuerte imagen y texto display
- **Tablet:** mantener jerarquía comprimiendo espaciado y largo de línea
- **Mobile:** apilar todos los módulos, un CTA principal por sección, tarjetas de servicio y credenciales en orden vertical
- Bloques de servicio: de varias columnas a una sola columna
- Botón de WhatsApp fijo/flotante en móvil, discreto y en tonos de marca

---

## 9. Agent Prompt Guide

### Referencia rápida de color
- CTA primario: `#6B4A9E`
- Hover del CTA: `#5B3D89`
- Fondo: `#F8F4FC`
- Texto de titulares: `#1B1620`
- Texto de cuerpo: `#1B1620`
- Borde/anillo: `#1B1620`
- Acento: `#D9C9F0`

### Resumen
Una estética de bienestar cálida, clara y emocionalmente contenedora. Combina un fondo lavanda muy claro con acentos en morado ciruela y lila. La tipografía une una cara display grande y expresiva con texto de cuerpo calmado y legible. Los botones son píldoras, con CTAs primarios rellenos y acciones secundarias con contorno. La profundidad es mínima; el diseño se apoya en espacio, tipografía y contraste de color. Las imágenes son orgánicas y cotidianas, y respaldan una práctica de nutrición cercana, rigurosa y respetuosa.

### Prompts de ejemplo por componente
- **Hero:** "Crea un hero cálido sobre fondo lavanda claro con un titular grande y expresivo, una introducción breve y empática, un botón píldora morado 'AGENDAR HORA' y un botón secundario con contorno 'ESCRIBIR POR WHATSAPP'."
- **Tarjeta de servicio:** "Crea una tarjeta plana con fondo lila suave, texto oscuro, ícono sticker, título corto y enlace 'Saber más', con mucho espaciado interno."
- **Navegación:** "Navegación simple con texto oscuro sobre fondo claro, enlaces discretos y un botón píldora morado a la derecha."
- **Botón o badge:** "Estilo píldora redondeada; primario relleno en morado ciruela, secundario con contorno carbón."

### Prompt listo para usar
Diseña una landing page clara, cálida y amigable para una nutricionista clínica especializada en intolerancias alimentarias, selectividad alimentaria y trastornos de conducta alimentaria, atención de adultos, niños con necesidades especiales de salud y malnutrición por déficit y por exceso. Usa fondo lavanda claro, acciones primarias en morado ciruela, acentos en lila, texto carbón violeta y tipografía display expresiva. Mantén el diseño aireado, editorial y generador de confianza, con CTAs en forma de píldora, sombras mínimas e imágenes de estilo de vida. Incluye agenda en Encuadrado (encuadrado.com) y contacto por WhatsApp.

### Guía de iteración
- Preservar la paleta lavanda-morado-lila antes de agregar nuevos adornos visuales
- Mantener el fuerte contraste entre titulares expresivos y cuerpo simple
- Mantener componentes planos, redondeados y espaciosos; evitar elevación pesada o estilos fríos y tecnológicos

---

## 10. Contenido de la Landing Page

> Los textos son una propuesta base; reemplazar los datos entre corchetes por los reales.

### Datos de la profesional
- **Nombre:** [Nombre y apellido], Nutricionista
- **Consulta:** consulta privada [ciudad / modalidad presencial y/o telemedicina]
- **Agenda:** Encuadrado (https://encuadrado.com/[usuario])
- **Contacto:** WhatsApp [+56 9 XXXX XXXX]

### Estructura sugerida de la página

**1. Hero**
- Eyebrow: `NUTRICIONISTA · NUTRICIÓN CLÍNICA`
- Titular: "Comer bien también puede ser tranquilo."
- Subtítulo: "Acompañamiento nutricional cercano y basado en evidencia para adultos y niños, con especial foco en intolerancias, selectividad alimentaria y necesidades especiales de salud."
- CTAs: `AGENDAR HORA` (Encuadrado) · `ESCRIBIR POR WHATSAPP`

**2. Marquesina**
- "NUTRICIÓN CON SENTIDO · COMER SIN MIEDO · CADA CUERPO, SU RITMO ·"

**3. Áreas de atención** (tarjetas de servicio con ícono sticker y enlace "Saber más")
- **Intolerancias alimentarias:** "Identificamos y manejamos tus intolerancias y alergias alimentarias para que comas con seguridad, variedad y sin restricciones innecesarias."
- **Selectividad alimentaria y trastornos de conducta alimentaria:** "Acompañamiento respetuoso y sin presión para niños, adolescentes y adultos que tienen una relación difícil con la comida."
- **Atención a adultos:** "Planes personalizados que se adaptan a tu salud, tu rutina y tus objetivos reales."
- **Niños con necesidades especiales de salud:** "Nutrición especializada para niños y niñas con síndrome de Down, parálisis cerebral y dieta cetogénica en epilepsia refractaria, trabajando junto a la familia y el equipo tratante."
- **Malnutrición por déficit y por exceso:** "Abordaje clínico de la desnutrición, el bajo peso, el sobrepeso y la obesidad, con foco en la salud y no en la culpa."

**4. Sobre mí**
- Título: "Hola, soy [Nombre]"
- Texto breve y cálido sobre su enfoque: acompañar a las familias con empatía, evidencia y ética clínica. Mencionar su formación en bioética como sello de un trato respetuoso y centrado en la persona.
- Fotografía de la profesional (retrato natural y cercano)

**5. Formación y credenciales** (lista en estilo meta)
- Nutricionista, Universidad de Concepción
- Magíster en Nutrición Clínica Pediátrica
- Magíster en Bioética
- Diplomado en Obesidad Infantil
- Diplomado en Enfermedad Celíaca y Alergias Alimentarias
- Diplomado en Trastornos de Conducta Alimentaria
- Diplomado en Docencia Clínica

**6. Cómo trabajamos** (3 pasos simples)
1. **Agenda tu hora:** reserva en línea por Encuadrado o escríbeme por WhatsApp.
2. **Primera consulta:** conversamos con calma sobre tu historia, tu salud y tus necesidades.
3. **Plan y seguimiento:** definimos juntos un plan realista, con controles y ajustes a tu ritmo.

**7. Testimonios** (solo reales y con autorización escrita; omitir la sección si aún no hay)
- Cita grande + iniciales + relación (ej. "Mamá de paciente")

**8. Preguntas frecuentes** (acordeón plano)
- ¿Atiendes niños y adultos?
- ¿Cómo agendo mi hora?
- ¿Cuánto dura la primera consulta?
- ¿Trabajas con otros profesionales de salud?
- ¿Atiendes por telemedicina?

**9. CTA final / Contacto**
- Titular: "Demos el primer paso, juntos."
- Texto: "Agenda tu hora en línea o escríbeme por WhatsApp para resolver tus dudas."
- CTAs: `AGENDAR EN ENCUADRADO` · `ESCRIBIR POR WHATSAPP`

**10. Footer**
- Nombre, título profesional, ciudad, enlaces a Encuadrado y WhatsApp, redes sociales (si aplica)
- Nota breve: "La información de este sitio es de carácter educativo y no reemplaza la consulta profesional."

### Voz y tono
- Profesional, cálida, tranquilizadora y accesible
- Lenguaje claro, sin tecnicismos innecesarios, sin juicios sobre peso, alimentación o cuerpo
- Titulares con patrón: claim empático + resultado positivo
- Lenguaje de CTA: directo e invitante ("AGENDAR HORA", "ESCRIBIR POR WHATSAPP", "SABER MÁS")

### Patrón de señales de confianza
- Credenciales académicas visibles
- Enfoque ético (bioética) y trabajo con equipos de salud
- Testimonios reales y autorizados
- Transparencia: cómo agendar, qué esperar de la primera consulta

---

## Apéndice: Patrones de interacción
- **Scroll:** landing narrativa guiada por secciones
- **Hover:** sutil y de bajo movimiento
- **Click:** acciones primarias inmediatas y claras, sin animaciones dramáticas
- **Tono de animación:** calmado, de apoyo y contenido
- **Accesibilidad:** contraste AA como mínimo, foco visible, textos alternativos descriptivos en imágenes, respetar `prefers-reduced-motion` (la marquesina debe poder pausarse)
