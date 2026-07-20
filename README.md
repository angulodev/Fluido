# Fluido 🇬🇧

**Entrenador diario de inglés impulsado por IA**, pensado para hispanohablantes que entienden al leer pero se bloquean al hablar y escuchar.

## ✨ Qué incluye

### Práctica con IA, hecha a tu medida
- **Conversar** — Simulador de situaciones reales (entrevistas, reuniones, small talk) con corrección instantánea estilo "resaltador de profesor" (colapsada por defecto, para no cortar el flujo de la conversación), por texto o con 🎤 Modo voz. Situación aleatoria, sobre tus temas, o **✏️ propón tu propio escenario** describiéndolo en español. En niveles básicos, las contracciones (I'd, you'll, won't…) se muestran con su forma completa entre paréntesis.
- **Escuchar** — Diálogos generados a tu nivel con 30+ situaciones rotativas y **temas personalizados** que la IA crea según tu perfil. Escucha sin leer (0.5×–2×), responde la comprensión, y con la transcripción: audio por línea, **shadowing con puntaje de pronunciación** y traducciones bajo demanda.
- **📖 Historia** — Mini-cuentos interactivos de 3 capítulos donde tú decides qué pasa. Las opciones vienen en inglés: entenderlas es parte del juego.
- **Escribir** — Taller de construcción de oraciones, no solo corrección: eliges tipo (afirmativa/negativa/pregunta) y tiempo verbal, ves la **fórmula** con un ejemplo real y una nota sobre el verbo, y escribes tu oración en un solo cuadro siguiendo esa guía. Recibes corrección completa **+ si respetaste la estructura pedida**, "💡 Dame ideas" con oraciones de ejemplo del escenario, "🔁 Otra estructura" para repetir el mismo escenario cambiando el tiempo verbal, y **✏️ Proponer mi propio escenario** para practicar tu propia situación.
- **🎤 Pronunciación en todas partes** — Frases, vocabulario, historias y diálogos: habla al micrófono y recibe puntaje palabra por palabra, con texto en vivo mientras hablas.

### Memoria de largo plazo
- **Frases, Verbos y +2.900 palabras** con repetición espaciada (SM-2 con factor de facilidad). Máximo **10 palabras nuevas al día** — retención real, no maratones.
- **⚡ Repaso del día** — Sesión mixta que junta todo lo vencido, con rondas encadenadas de 20. Incluye **🔇 modo silencio**: selección múltiple con distractores inteligentes y armar frases palabra a palabra, autocorregidos, con feedback tipo diff (verde lo que acertaste de posición), "no lo sé" honesto y audio opcional para practicar dictado.

### 📋 Cheat sheets y sesiones de estudio
- **Cheat sheets exportables** — Al terminar Escribir, Escuchar o el Repaso: ficha de estudio con tus notas + **tips de IA específicos, elementos para repasar y un consejo**. Descargable como imagen PNG (generada en tu navegador, sin costo) y **compartible por WhatsApp** con un toque.
- **🎓 Sesión de estudio** — Botón flotante que toma notas por ti en segundo plano a través de TODOS los módulos mientras practicas. Al finalizar: resumen completo de tu sesión, estilo cheat sheet. Con el toggle **"Sesión de estudio automática"** en Ajustes, arranca sola al abrir la app y se cierra armando el cheat sheet al salir o pasar a segundo plano — los tips de IA se completan solos la próxima vez que abras Fluido.
- **🗂️ Historial** — Todas tus fichas se archivan automáticamente (con sus tips) y puedes reabrirlas, volver a compartirlas o eliminarlas desde Inicio o Ajustes.

### Experiencia
- Diseño renovado: tema claro **Lavanda** + 12 temas más, nav flotante con burbuja elevada en el tab activo, sombras suaves y microinteracciones.
- Rutas por pestaña (#/listen, #/talk…): las recargas te dejan donde estabas y el botón atrás navega la app.
- Onboarding en 3 pasos que explica qué hace la app y cómo cuida tu privacidad **antes** de pedirte nada.
- Tarjetas "¿cómo funciona?" en cada módulo, misiones diarias, racha con protector semanal, recordatorio diario con notificaciones, estadísticas de actividad, selector de voz/acento (🇺🇸/🇬🇧), export/import de todo tu progreso.

## 🚀 Cómo usarla

1. Abre `index.html` en cualquier navegador (o visita la versión publicada). Es una **PWA instalable** que funciona offline desde la primera visita.
2. Conecta una IA con tu propia clave — Fluido soporta 5 proveedores, con reintento automático a otro modelo si uno falla:
   - **Google Gemini (gratis)**: [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   - **Groq · Llama 3.3 (gratis, ultra rápido)**: [console.groq.com/keys](https://console.groq.com/keys)
   - **OpenRouter (gratis, Qwen/DeepSeek/Llama)**: [openrouter.ai/keys](https://openrouter.ai/keys)
   - **DeepSeek (muy barato)**: [platform.deepseek.com/api_keys](https://platform.deepseek.com/api_keys)
   - **Claude (Anthropic, de pago)**: requiere créditos en [console.anthropic.com](https://console.anthropic.com)

   Puedes configurar más de uno: si el proveedor activo falla (límite de uso, error, etc.), Fluido reintenta automáticamente con los demás que tengas conectados. Este respaldo automático se puede desactivar en Ajustes.
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
