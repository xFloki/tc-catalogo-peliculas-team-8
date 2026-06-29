# 🎬 Catálogo de Películas — Team 8

Proyecto del Sprint 03-04 del Bootcamp IA Generativa (The Bridge Tech).  
Construimos un catálogo enriquecido de películas usando Pandas, la API de TMDB y Gemini AI.

---

## 👥 Equipo

| Nombre | Parte liderada |
|--------|---------------|
| Alejandro Dietta Martin | Parte 1 · Pandas |
| Marta Roldán Mariscal | Parte 2 · TMDB API |
| PENDING | Parte 3 · Gemini |
| PENDING | Parte 4 · Opcional |
| PENDING | Parte 4 · Opcional |

---

## 🗂️ Estructura del proyecto

```
tc-catalogo-peliculas-team-8/
├── data/
│   ├── movies.csv
│   ├── ratings.csv
│   ├── tags.csv
│   └── links.csv
├── notebook.ipynb
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

## 🚀 Cómo empezar

### 1. Clonar el repositorio

```bash
git clone https://github.com/xFloki/tc-catalogo-peliculas-team-8.git
cd tc-catalogo-peliculas-team-8
```

### 2. Crear y activar el entorno virtual

```bash
python -m venv venv

# Mac/Linux
source venv/bin/activate 

# Windows (Git Bash)
source venv/Scripts/activate

# Windows (CMD)
venv\Scripts\activate
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 4. Configurar las claves de API

```bash
cp .env.example .env
```

Edita el archivo `.env` con tus claves reales (ver sección de credenciales abajo). **Nunca subas este archivo al repositorio.**

### 5. Ejecutar el notebook

```bash
jupyter notebook notebook.ipynb
```

Ejecuta las celdas en orden de arriba a abajo.

---

## 🔑 Credenciales necesarias

Las variables de entorno que necesitas están en `.env.example`. Necesitarás:

- **TMDB_API_KEY** — obtenla en [themoviedb.org](https://www.themoviedb.org/settings/api) (registro gratuito)
- **GEMINI_API_KEY** — obtenla en [aistudio.google.com](https://aistudio.google.com/app/apikey)

⚠️ Nunca pongas las claves directamente en el notebook ni en ningún archivo que se suba al repo.

---

## 📦 Dependencias principales

Ver `requirements.txt` para la lista completa. Las principales:

- `pandas` — análisis y manipulación de datos
- `requests` — llamadas a la API de TMDB
- `google-genai` — cliente oficial de Gemini
- `python-dotenv` — carga de variables de entorno
- `jupyter` — entorno de notebooks

---

## 🌿 Git Flow

Usamos una versión adaptada de Git Flow:

```
main        ← producción estable (solo merge desde develop vía PR)
develop     ← integración continua (rama de trabajo compartida)
feature/*   ← ramas cortas por tarea, se borran tras el merge
```

**Norma de oro: nunca se hace commit directo a `main`.**

### Workflow diario

```bash
# 1. Partir siempre de develop actualizado
git checkout develop
git pull origin develop
git checkout -b feature/mi-tarea

# 2. Trabajar y commitear
git add .
git commit -m "feat: descripción de lo que hice"

# 3. Subir y abrir PR hacia develop
git push origin feature/mi-tarea
# → Abrir Pull Request en GitHub hacia develop
```

---

## ✅ Checklist de setup inicial

- [x] Repositorio creado en GitHub y compartido con el equipo
- [x] Rama `develop` creada desde `main`
- [x] Protección de rama `main` activada (requiere PR + 1 aprobación)
- [x] README con instrucciones de clonado y dependencias
- [x] `.gitignore` configurado (`.env`, `venv/`, `*.pyc`, `__pycache__/`)
- [x] `.env.example` con las variables necesarias (sin valores reales)
- [ ] Reparto de tareas acordado por todo el equipo
- [ ] Parte 1 · Pandas completada
- [ ] Parte 2 · TMDB API completada
- [ ] Parte 3 · Gemini completada
- [ ] Parte 4 · Opcional completada

---

*Bootcamp IA Generativa · The Bridge Tech · Sprint 03-04*
