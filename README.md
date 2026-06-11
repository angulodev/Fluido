# Fluido 🇬🇧

**Entrenador diario de inglés impulsado por IA**, pensado para hispanohablantes que entienden al leer pero se bloquean al hablar o escuchar.

## ✨ Qué incluye

- **Conversar** — Simulaciones de situaciones reales (reuniones, entrevistas, small talk) con corrección instantánea estilo "resaltador de profesor".
- **Frases** — Mazo de repaso espaciado con frases de supervivencia profesional + generación de frases nuevas con IA según tu perfil.
- **Escuchar** — Diálogos generados por IA leídos en voz alta (velocidad ajustable) con preguntas de comprensión antes de revelar la transcripción.
- Onboarding personalizado, racha diaria, misiones, niveles A2/B1/B2.

## 🚀 Cómo usarla

1. Abre `index.html` en cualquier navegador (o visita la versión publicada).
2. Conecta una IA con tu propia clave:
   - **Google Gemini (gratis)**: crea tu clave en [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   - **Claude (Anthropic)**: requiere créditos en [console.anthropic.com](https://console.anthropic.com)
3. Responde el cuestionario inicial y entrena 15 minutos al día.

Tu clave y tu progreso se guardan **solo en tu navegador**. Nada sale de tu dispositivo, salvo las llamadas a la IA que tú configuraste.

## 🛠️ Stack

Un solo archivo HTML: React 18 (UMD) + Babel standalone, Web Speech API para el audio, localStorage para persistencia. Sin backend, sin build, sin dependencias que instalar.

## 🗺️ Roadmap (Fase 2)

- Cuentas de usuario con Supabase Auth
- Banco de ejercicios compartido en Postgres (reduce costos de generación)
- Edge Function como proxy de IA con límites diarios por usuario
- PWA instalable con recordatorios

---

Hecho con ❤️ desde Chile.
