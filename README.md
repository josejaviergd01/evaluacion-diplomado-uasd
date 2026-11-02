# Sistema de Control de Asistencias & Formaciones 📋📊

Aplicación web interactiva para el levantamiento de datos de asistencia a capacitaciones, talleres y cursos, con módulo integrado de reportería, analítica y preparación para base de datos SQL.

---

## 🚀 Cómo probarlo inmediatamente

1. Navega a la carpeta `sistema_asistencias`.
2. Haz **doble clic sobre el archivo `index.html`** (se abrirá en Chrome, Edge, Brave o tu navegador predeterminado).
3. ¡Listo! Ya viene pre-cargado con datos de prueba realistas para que explores:
   * **Pestaña 1 (Formulario):** Registra una nueva asistencia y observa cómo se agrega en tiempo real.
   * **Pestaña 2 (Reportería):** Visualiza los KPIs, el gráfico de barras por taller, el gráfico circular de puntualidad/asistencia y los filtros de búsqueda.
   * **Botón Exportar:** Descarga la matriz completa a un archivo `.csv` compatible con Microsoft Excel.

---

## 🛠️ Cómo publicar este proyecto en GitHub con Visual Studio Code

### Paso 1: Inicializar Git en esta carpeta
Abre una terminal en Visual Studio Code o PowerShell dentro de `sistema_asistencias` y ejecuta:

```bash
git init
git add .
git commit -m "feat: Version inicial con formulario y modulo de reporteria"
```

### Paso 2: Crear el repositorio en GitHub
1. Entra a tu cuenta en [GitHub.com](https://github.com).
2. Haz clic en **New Repository** (Nuevo Repositorio).
3. Ponle un nombre, por ejemplo: `control-asistencias-capacitaciones`.
4. Elige si prefieres que sea **Público** o **Privado**.
5. No marques la casilla de "Add README" (ya lo tenemos creado).
6. Haz clic en **Create repository**.

### Paso 3: Enlazar y subir desde tu computadora
Copia los comandos que te da GitHub y ejecútalos en la terminal de VS Code:

```bash
git remote add origin https://github.com/TU_USUARIO/control-asistencias-capacitaciones.git
git branch -M main
git push -u origin main
```

### Paso 4: Publicar gratis en GitHub Pages (Para usarlo desde el celular o cualquier PC)
1. En tu repositorio de GitHub, ve a **Settings** (Configuración) -> pestaña **Pages**.
2. En **Build and deployment > Branch**, selecciona `main` y la carpeta `/ (root)`.
3. Haz clic en **Save**.
4. En 1 minuto tendrás un enlace público como:
   `https://TU_USUARIO.github.io/control-asistencias-capacitaciones/`
   ¡Tu mamá podrá usarlo directamente desde su teléfono o tablet durante las formaciones!

---

## 🗄️ Próximo paso: Conexión a Base de Datos SQL

En la **Pestaña 3 del HTML** encontrarás el script SQL listo para crear las tablas relacionales (`formaciones` y `asistencias`).

Cuando desees dar el salto a una base de datos centralizada permanente:
* **Opción Nube (Supabase / PostgreSQL):** Conectamos el archivo JavaScript a Supabase para que las asistencias que registre tu mamá queden guardadas en la nube en tiempo real.
* **Opción Local (Python FastAPI / SQLite):** Creamos un microservicio backend local para almacenar los registros en un archivo SQL local.
