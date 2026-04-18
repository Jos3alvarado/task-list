# Task List Project

## Descripción
Este proyecto es una aplicación web para gestionar tareas. Está desarrollado utilizando Django y sigue una estructura de proyecto estándar. Incluye funcionalidades básicas para listar, crear, editar y eliminar tareas.

---

## Estructura del Proyecto

```
.
├── db.sqlite3                # Base de datos SQLite
├── manage.py                 # Archivo principal para comandos de Django
├── requirements.txt          # Dependencias del proyecto
├── base_project/             # Configuración principal del proyecto
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py           # Configuración del proyecto
│   ├── urls.py               # Enrutamiento principal
│   └── wsgi.py
├── static/                   # Archivos estáticos
│   └── css/
│       └── base.css          # Estilos base
├── tasks/                    # Aplicación principal
│   ├── __init__.py
│   ├── admin.py              # Configuración del panel de administración
│   ├── apps.py               # Configuración de la aplicación
│   ├── models.py             # Modelos de datos
│   ├── tests.py              # Pruebas unitarias
│   ├── urls.py               # Enrutamiento de la aplicación
│   ├── views.py              # Vistas de la aplicación
│   └── migrations/           # Migraciones de base de datos
│       └── __init__.py
│       └── 0001_initial.py   # Migración inicial
└── templates/                # Plantillas HTML
    └── tasks/
        ├── _base.html        # Plantilla base
        └── tasks_list.html   # Plantilla para listar tareas
```

---

## Instalación y Configuración

### Requisitos Previos
- Python 3.8 o superior
- pip (gestor de paquetes de Python)

### Pasos para Configurar el Proyecto
1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   ```

2. Navega al directorio del proyecto:
   ```bash
   cd task_list
   ```

3. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

4. Realiza las migraciones de la base de datos:
   ```bash
   python manage.py migrate
   ```

5. Inicia el servidor de desarrollo:
   ```bash
   python manage.py runserver
   ```

6. Accede a la aplicación en tu navegador en `http://127.0.0.1:8000/`.

---

## Uso

### Funcionalidades Principales
- **Listar Tareas:** Visualiza todas las tareas existentes.
- **Crear Tareas:** Agrega nuevas tareas.
- **Editar Tareas:** Modifica tareas existentes.
- **Eliminar Tareas:** Borra tareas que ya no sean necesarias.

---

## Contribuir

1. Crea un fork del repositorio.
2. Crea una nueva rama para tu funcionalidad o corrección:
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```
3. Realiza tus cambios y haz commits:
   ```bash
   git commit -m "Descripción de los cambios"
   ```
4. Sube tus cambios a tu fork:
   ```bash
   git push origin feature/nueva-funcionalidad
   ```
5. Crea un Pull Request en el repositorio original.

---

## Licencia
Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.