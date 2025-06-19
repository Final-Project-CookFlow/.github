# CookFlow

CookFlow es una aplicación web para gestionar y compartir recetas de cocina. Este repositorio incluye instrucciones para instalar tanto el **frontend** (React + Vite) como el **backend** (Django + Django REST Framework).

---

## Requisitos previos

- [Node.js](https://nodejs.org/) (versión 18 o superior recomendada)
- [npm](https://www.npmjs.com/) o [yarn](https://yarnpkg.com/)
- [Python 3.10+](https://www.python.org/)
- [PostgreSQL](https://www.postgresql.org/) (u otro motor compatible)
- [pip](https://pip.pypa.io/)

---

## Instalación del Backend

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/tu-usuario/cookflow-backend.git
   cd cookflow-backend
   ```

2. **Crea y activa un entorno virtual:**

   En Windows:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

   En macOS/Linux:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Instala las dependencias:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configura las variables de entorno:**

   Crea un archivo `.env` en la raíz del backend con tus variables (ajusta según tu entorno):

   ```
   SECRET_KEY=tu_clave_secreta
   DEBUG=True
   ALLOWED_HOSTS=localhost,127.0.0.1
   DATABASE_URL=postgres://usuario:contraseña@localhost:5432/cookflow
   ```

5. **Aplica las migraciones y crea un superusuario:**

   ```bash
   python manage.py migrate
   python manage.py createsuperuser
   ```

6. **Carga datos de ejemplo (opcional):**

   ```bash
   python manage.py seed_all
   ```

7. **Inicia el servidor de desarrollo:**

   ```bash
   python manage.py runserver
   ```

   El backend estará disponible en [http://localhost:8000](http://localhost:8000).

---

## Instalación del Frontend

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/tu-usuario/cookflow-frontend.git
   cd cookflow-frontend
   ```

2. **Instala las dependencias:**

   Con npm:
   ```bash
   npm install
   ```

   O con yarn:
   ```bash
   yarn install
   ```

3. **Configura las variables de entorno:**

   Crea un archivo `.env` en la raíz del frontend y añade:

   ```
   VITE_API_URL=http://localhost:8000/api
   VITE_MEDIA_URL=http://localhost:8000/media/
   ```

4. **Inicia la aplicación en modo desarrollo:**

   Con npm:
   ```bash
   npm run dev
   ```

   O con yarn:
   ```bash
   yarn dev
   ```

   La aplicación estará disponible en [http://localhost:5173](http://localhost:5173).

---

## Scripts útiles (Frontend)

- `npm run dev` — Inicia el servidor de desarrollo.
- `npm run build` — Genera la versión de producción.
- `npm run preview` — Previsualiza la build de producción localmente.

---

## Notas

- Asegúrate de que el backend esté corriendo y accesible desde la URL configurada en `VITE_API_URL`.
- Si usas rutas o puertos diferentes, actualiza las variables de entorno en ambos proyectos.
- Para acceder al panel de administración de Django, visita [http://localhost:8000/admin](http://localhost:8000/admin).

---

## Developers
- [**Saturnino Méndez Cantero** - *@FrostyValue*](https://www.linkedin.com/in/saturnino-mendez/)
- [**Lorena Martínez Díaz** - *@aelnor-dev*](https://www.linkedin.com/in/lorena-martínez-díaz/)
- [**Rafael Fernández Rodríguez** - *@FoloCurso*](https://www.linkedin.com/in/rafael-fernández-rodríguez-96b031347/)
- [**Hema Priya** - *@void-craft*](https://www.linkedin.com/in/hemaps/)
- [**Noemí Casaprima Pendás** - *@Noemi1977*](https://www.linkedin.com/in/noemicasaprimapendas/)
- [**Nico Fernández** - *@srlsrx*](https://github.com/srlsrx)
- [**Ángel Miguel Aragón** - *@Algol95*](https://github.com/Algol95)
- [**Jose Manuel Barreiro Álvarez** - *@jomabal98*](https://www.linkedin.com/in/jose-manuel-barreiro-álvarez/)
- [**Sergio Jorquera Gimeno** - *@sergio-jorquera*](https://www.linkedin.com/in/sergio-jorquera-gimeno-48472934a/)
- [**Saray Miguel Narganes** - *@sarayminar*](https://www.linkedin.com/in/saray-miguel-narganes/)
- [**Yuliia Martynovych** - *@sarayminar*](https://www.linkedin.com/in/martynovych/)
- [**Ana Castro** - *@cuyssi*](https://www.linkedin.com/in/anabcastro/)

