# 🌈 MoodTrackr

Una aplicación moderna para registrar, visualizar y entender tus emociones diarias.
Desarrollada con **React**, **TypeScript**, **Express** y **PostgreSQL**.

---

## 🚀 Características principales

- 📅 **Registro diario** de emociones, notas y nivel de energía.
- 📊 **Gráficas interactivas** con tus tendencias emocionales.
- 🤖 **Análisis automático** mediante IA (modo experimental).
- 🔐 **Autenticación segura** con JWT.
- 🌙 **Modo oscuro** y diseño responsive.

---

## 🧠 Tecnologías utilizadas

| Capa | Tecnología |
|------|-------------|
| Frontend | React + Vite + Tailwind CSS |
| Backend | Node.js + Express + TypeScript |
| Base de datos | PostgreSQL + TypeORM |
| Autenticación | JWT + bcrypt |
| Despliegue | Docker + Render + GitHub Actions |

---

## ⚙️ Instalación y configuración

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/tuusuario/moodtrackr.git
cd moodtrackr

### 2️⃣ Configurar variables de entorno

Crea un archivo `.env` en la raíz del proyecto con el siguiente contenido:

```
# Backend
PORT=4000
DATABASE_URL=postgresql://user:password@localhost:5432/moodtrackr
JWT_SECRET=supersecreto123

# Frontend
VITE_API_URL=http://localhost:4000/api

```

### 3️⃣ Instalar dependencias

```bash
npm install

```

### 4️⃣ Ejecutar el entorno local

```bash
npm run dev

```

---

## 🧩 Estructura del proyecto

```
moodtrackr/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── services/
│   │   ├── entities/
│   │   └── routes/
│   └── index.ts
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   └── styles/
│   └── main.tsx
└── docker-compose.yml

```

---

## 🧪 Scripts disponibles

| Comando | Descripción |
| --- | --- |
| `npm run dev` | Inicia el servidor y el cliente en modo desarrollo |
| `npm run build` | Compila frontend y backend |
| `npm run test` | Ejecuta las pruebas unitarias |
| `npm run lint` | Verifica el código con ESLint |

---

## 🧭 API Endpoints

| Método | Endpoint | Descripción |
| --- | --- | --- |
| `POST` | `/api/auth/register` | Crear un nuevo usuario |
| `POST` | `/api/auth/login` | Iniciar sesión |
| `GET` | `/api/moods` | Obtener todos los registros del usuario |
| `POST` | `/api/moods` | Crear un nuevo registro de ánimo |
| `GET` | `/api/moods/:id` | Obtener detalle de un registro |

---

## 👩‍💻 Contribuir

1. Haz un fork del proyecto
2. Crea una rama para tu feature:
    
    ```bash
    git checkout -b feature/mi-nueva-funcionalidad
    
    ```
    
3. Realiza tus cambios y commitea:
    
    ```bash
    git commit -m "Agrega nueva funcionalidad"
    
    ```
    
4. Envía un pull request 🚀

---

## 🧯 Pruebas unitarias

Este proyecto utiliza **Jest** y **Testing Library** para validar la lógica y componentes.

```bash
npm run test

```

Ejemplo de prueba:

```tsx
// src/tests/moodService.test.ts
import { MoodService } from "../services/MoodService"

describe("MoodService", () => {
  it("crea un registro válido", async () => {
    const service = new MoodService()
    const mood = await service.create({ mood: "Feliz", energy: 8 })
    expect(mood.id).toBeDefined()
  })
})

```

---

## 📄 Licencia

Este proyecto está bajo la **licencia MIT**.

Eres libre de usarlo, modificarlo y compartirlo con atribución.

---

## 💖 Agradecimientos

- A la comunidad open-source 💪
- A quienes priorizan su salud mental 🧘‍♀️
- A ti, por usar MoodTrackr 💫

---

> “Tu estado de ánimo no define quién eres, pero entenderlo puede cambiar tu vida.”
> 
> 
> — Equipo MoodTrackr
>
