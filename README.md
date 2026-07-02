# Fluido 🇬🇧

**Entrenador diario de inglés impulsado por IA**, pensado para hispanohablantes que entienden al leer pero se bloquean al hablar o escuchar.

## ✨ Qué incluye

- **Conversar** — Simulaciones de situaciones reales (reuniones, entrevistas, small talk) con corrección instantánea estilo "resaltador de profesor" y dictado por voz.
- **Frases** — Mazo de repaso espaciado (SRS estilo SM-2 con factor de facilidad por tarjeta) con frases de supervivencia profesional + generación de frases nuevas con IA según tu perfil o por escenario, con filtro anti-duplicados contra todo el mazo.
- **🎤 Práctica de pronunciación** — En cada tarjeta puedes grabar tu voz: Fluido compara palabra por palabra lo que dijiste contra la frase objetivo y te da un puntaje con las palabras falladas en rojo.
- **Escuchar** — Diálogos generados por IA leídos en voz alta (velocidad 0.5×–2×) con preguntas de comprensión antes de revelar la transcripción.
  - **30 situaciones rotativas** (restaurante, aeropuerto, médico, arriendo, soporte técnico…) con memoria anti-repetición: no se repite un tema hasta pasados 10 audios.
  - **✨ Temas personalizados**: la IA genera 8 situaciones a la medida de TU perfil (trabajo, objetivos, intereses) con un solo llamado. Si cambias tu perfil, Fluido te avisa para actualizarlos.
  - **⭐ Temas propios**: agrega a mano las situaciones que quieras practicar.
  - **🗣️ Shadowing**: en la transcripción, reproduce cada línea por separado y repítela con el micrófono para obtener tu puntaje de pronunciación línea a línea.
- **Verbos y Vocabulario** — Bancos offline con repaso espaciado (mismo motor SM-2) y ejemplos en contexto generados por IA según tu nivel.
- **Quiz de gramática** — Sin conexión, filtrado por nivel CEFR.
- **Escribir** — Corrección y conversación escrita con IA.
- **⚡ Repaso del día** — Tarjeta en el inicio que suma todo lo vencido en los tres sistemas SRS (frases + verbos + vocabulario) para que no se te escape nada.
- **📊 Progreso real** — Recomendación de subir/bajar de nivel basada en tu desempeño en producción y comprensión, más gráfico de actividad de los últimos 7 días.
- **🔥 Racha con protector** — Si fallas un día con racha ≥3, Fluido lo perdona automáticamente (máximo 1 vez por semana).
- **🔔 Recordatorio diario** — Notificación a la hora que elijas (con la app o PWA abierta en segundo plano).
- **🗣️ Selector de voz** — Elige el acento y la voz del audio en inglés (🇺🇸/🇬🇧); por defecto Fluido escoge automáticamente la mejor voz disponible del dispositivo.
- Onboarding personalizado, misiones diarias, niveles A0/A2/B1/B2/C1, 12 temas visuales, exportación e importación de todo tu progreso.

## 🚀 Cómo usarla

1. Abre `index.html` en cualquier navegador (o visita la versión publicada). Es una **PWA instalable** que funciona offline desde la primera visita.
2. Conecta una IA con tu propia clave:
   - **Google Gemini (gratis)**: crea tu clave en [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   - **Claude (Anthropic)**: requiere créditos en [console.anthropic.com](https://console.anthropic.com)
3. Responde el cuestionario inicial y entrena 15 minutos al día.

Tu clave y tu progreso se guardan **solo en tu navegador**. Nada sale de tu dispositivo, salvo las llamadas a la IA que tú configuraste. Puedes exportar un respaldo completo desde Ajustes.

> 💡 La práctica de pronunciación y el dictado por voz usan la Web Speech API — funcionan mejor en Chrome (Android y desktop).

## 🛠️ Stack

Un solo archivo HTML: React 18 (UMD) + Babel standalone, Web Speech API (síntesis + reconocimiento de voz), Service Worker con pre-cache para uso offline, localStorage para persistencia. Sin backend, sin build, sin dependencias que instalar.

## 🗺️ Roadmap (Fase 2)

- Cuentas de usuario con Supabase Auth
- Banco de ejercicios compartido en Postgres (reduce costos de generación)
- Edge Function como proxy de IA con límites diarios por usuario
- Notificaciones push reales (sin necesidad de tener la app abierta)

---

Hecho con ❤️ desde Chile.
