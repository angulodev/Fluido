# Fluido 🇬🇧

**Entrenador diario de inglés impulsado por IA**, pensado para hispanohablantes que entienden al leer pero se bloquean al hablar y escuchar.

## ✨ Qué incluye

### Práctica con IA, hecha a tu medida
- **Conversar** — Simulador de situaciones reales (entrevistas, reuniones, small talk) con corrección instantánea estilo "resaltador de profesor", por texto o con 🎤 Modo voz.
- **Escuchar** — Diálogos generados a tu nivel con 30+ situaciones rotativas y **temas personalizados** que la IA crea según tu perfil. Escucha sin leer (0.5×–2×), responde la comprensión, y con la transcripción: audio por línea, **shadowing con puntaje de pronunciación** y traducciones bajo demanda.
- **📖 Historia** — Mini-cuentos interactivos de 3 capítulos donde tú decides qué pasa. Las opciones vienen en inglés: entenderlas es parte del juego.
- **Escribir** — Taller con profesor: consignas a tu nivel (o sobre tus temas), versión corregida completa y cada error explicado en español. Con conversación de seguimiento.
- **🎤 Pronunciación en todas partes** — Frases, vocabulario, historias y diálogos: habla al micrófono y recibe puntaje palabra por palabra, con texto en vivo mientras hablas.

### Memoria de largo plazo
- **Frases, Verbos y +2.900 palabras** con repetición espaciada (SM-2 con factor de facilidad). Máximo **10 palabras nuevas al día** — retención real, no maratones.
- **⚡ Repaso del día** — Sesión mixta que junta todo lo vencido, con rondas encadenadas de 20. Incluye **🔇 modo silencio**: selección múltiple con distractores inteligentes y armar frases palabra a palabra, autocorregidos, con feedback tipo diff (verde lo que acertaste de posición), "no lo sé" honesto y audio opcional para practicar dictado.

### 📋 Cheat sheets y sesiones de estudio
- **Cheat sheets exportables** — Al terminar Escribir, Escuchar o el Repaso: ficha de estudio con tus notas + **tips de IA específicos, elementos para repasar y un consejo**. Descargable como imagen PNG (generada en tu navegador, sin costo) y **compartible por WhatsApp** con un toque.
- **🎓 Sesión de estudio** — Botón flotante que toma notas por ti en segundo plano a través de TODOS los módulos mientras practicas. Al finalizar: resumen completo de tu sesión, estilo cheat sheet.
- **🗂️ Historial** — Todas tus fichas se archivan automáticamente (con sus tips) y puedes reabrirlas, volver a compartirlas o eliminarlas desde Inicio o Ajustes.

### Experiencia
- Diseño renovado: tema claro **Lavanda** + 12 temas más, nav flotante, sombras suaves y microinteracciones.
- Rutas por pestaña (#/listen, #/talk…): las recargas te dejan donde estabas y el botón atrás navega la app.
- Onboarding en 3 pasos que explica qué hace la app y cómo cuida tu privacidad **antes** de pedirte nada.
- Tarjetas "¿cómo funciona?" en cada módulo, misiones diarias, racha con protector semanal, recordatorio diario con notificaciones, estadísticas de actividad, selector de voz/acento (🇺🇸/🇬🇧), export/import de todo tu progreso.

## 🚀 Cómo usarla

1. Abre `index.html` en cualquier navegador (o visita la versión publicada). Es una **PWA instalable** que funciona offline desde la primera visita.
2. Conecta una IA con tu propia clave:
   - **Google Gemini (gratis)**: [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   - **Claude (Anthropic)**: requiere créditos en [console.anthropic.com](https://console.anthropic.com)
3. Responde el cuestionario inicial y entrena 15 minutos al día.

Tu clave y tu progreso se guardan **solo en tu navegador**. Fluido no tiene servidores: nada sale de tu dispositivo salvo las llamadas al proveedor de IA que tú elijas. Respaldo completo exportable desde Ajustes.

> 💡 La práctica de pronunciación y el dictado por voz usan la Web Speech API — funcionan mejor en Chrome (Android y desktop).

## 🛠️ Stack

Un solo archivo HTML: React 18 (UMD) + Babel standalone, Web Speech API (síntesis + reconocimiento), Canvas API para las imágenes de cheat sheets, Service Worker con pre-cache y notificaciones, localStorage como persistencia. Sin backend, sin build, sin dependencias que instalar.

## 🗺️ Roadmap (Fase 2)

- Cuentas de usuario con Supabase Auth y sincronización entre dispositivos (progreso + biblioteca de cheat sheets)
- Banco de ejercicios compartido en Postgres (reduce costos de generación)
- Edge Function como proxy de IA con límites diarios por usuario
- Notificaciones push reales (sin necesidad de tener la app abierta)

---

Hecho con ❤️ desde Chile.
