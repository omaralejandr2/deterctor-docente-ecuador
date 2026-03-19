# 🇪🇨 Detector de Sobrecarga Docente — Ecuador

App web con IA para detectar sobrecarga y riesgo de burnout en docentes de secundaria del Ecuador.
Basada en normativa MinEduc, LOEI y BGU.

---

## 🚀 Publicar en Vercel (paso a paso)

### Paso 1 — Subir a GitHub

1. Entra a [github.com](https://github.com) e inicia sesión
2. Haz clic en **"New repository"** (botón verde)
3. Ponle nombre: `detector-docente-ecuador`
4. Déjalo **público** → clic en **"Create repository"**
5. En la siguiente pantalla verás instrucciones. Copia el link del repositorio (algo como `https://github.com/tu-usuario/detector-docente-ecuador.git`)

Luego, en tu computadora Windows:
- Descarga e instala **[Git para Windows](https://git-scm.com/download/win)**
- Abre la carpeta del proyecto → clic derecho → **"Git Bash Here"**
- Ejecuta estos comandos uno por uno:

```bash
git init
git add .
git commit -m "primer commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/detector-docente-ecuador.git
git push -u origin main
```

---

### Paso 2 — Conectar con Vercel

1. Entra a [vercel.com](https://vercel.com) → **"Sign up with GitHub"**
2. Haz clic en **"Add New Project"**
3. Selecciona el repositorio `detector-docente-ecuador`
4. Vercel detecta automáticamente que es Vite — no cambies nada
5. **ANTES de hacer Deploy**, ve a **"Environment Variables"** y agrega:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** tu clave de API de Anthropic (la encuentras en [console.anthropic.com](https://console.anthropic.com))
6. Haz clic en **"Deploy"**

¡Listo! En 2-3 minutos tendrás una URL como:
`https://detector-docente-ecuador.vercel.app`

---

### Paso 3 — Compartir

Comparte esa URL con tus colegas por WhatsApp, correo o redes sociales.
Funciona en celular y computadora, sin instalar nada.

---

## 🔑 ¿Dónde obtengo mi API Key de Anthropic?

1. Entra a [console.anthropic.com](https://console.anthropic.com)
2. Crea una cuenta gratuita
3. Ve a **"API Keys"** → **"Create Key"**
4. Copia la clave y guárdala en un lugar seguro (solo se muestra una vez)

> **Nota:** Anthropic ofrece créditos gratuitos al registrarse. Para uso moderado (pocos cientos de análisis), el costo es muy bajo.

---

## 📁 Estructura del proyecto

```
detector-docente/
├── api/
│   └── analizar.js        ← Función serverless (API key segura aquí)
├── src/
│   ├── App.jsx            ← App principal React
│   └── main.jsx           ← Punto de entrada
├── public/
│   └── favicon.svg
├── index.html
├── package.json
├── vite.config.js
└── vercel.json
```

---

## ⚖️ Aviso

Esta app es orientativa y no reemplaza orientación profesional de salud mental.
Basada en LOEI, Acuerdos Ministeriales y estándares MinEduc Ecuador.
