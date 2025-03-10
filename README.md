# Gestor de Vacunas - Clínica Veterinaria 🐾

## Descripción del Proyecto
Sistema web desarrollado en Django para la gestión de vacunación de mascotas en clínicas veterinarias. Permite llevar un control detallado del historial de vacunación, recordatorios automáticos y gestión de citas veterinarias. Implementa principios de accesibilidad web para garantizar una experiencia inclusiva para todos los usuarios.

## Características Principales 🌟
- Registro y gestión de propietarios de mascotas
- Control de historial de vacunación
- Sistema de recordatorios automáticos
- Panel administrativo para veterinarios
- Interfaz responsive y amigable
- Integración con redes sociales
- Sistema de contacto vía WhatsApp
- Implementación de HTML semántico para mejor accesibilidad
- Compatibilidad con lectores de pantalla

## Tecnologías Utilizadas 💻
- **Backend:** Django 5.1.6
- **Frontend:** HTML5 Semántico, CSS3, JavaScript
- **Base de Datos:** MySQL
- **Dependencias Principales:**
  - django-environ 0.12.0
  - django-jazzmin 3.0.1
  - Pillow 11.1.0
  - reportlab 4.3.1
- **Estándares de Accesibilidad:**
  - WCAG 2.1 (Web Content Accessibility Guidelines)
  - WAI-ARIA (Web Accessibility Initiative - Accessible Rich Internet Applications)

## Requisitos Previos 📋
- Python 3.x
- MySQL Server
- Entorno virtual (virtualenv o venv)

## Instalación 🔧

1. **Clonar el repositorio**
```bash
git clone [https://github.com/kevincl03/App-Gestion-Vacunas.git]
cd App-Gestion-Vacunas
```

2. **Crear y activar entorno virtual**
```bash
# Windows
python -m venv env
env/Scripts/activate

# Linux/Mac
python3 -m venv env
source env/bin/activate
```

3. **Instalar dependencias**
```bash
pip install -r requirements.txt
```

4. **Configurar variables de entorno**
```bash
# Crear archivo .env basado en .env.example
cp .env.example .env
# Editar .env con tus configuraciones
```

5. **Realizar migraciones**
```bash
python manage.py migrate
```

6. **Crear superusuario**
```bash
python manage.py createsuperuser
```

7. **Iniciar servidor de desarrollo**
```bash
python manage.py runserver
```

## Estructura del Proyecto 📁
```
Respaldo-proyecto-gestor-vacuna/
├── gestor_vacuna/          # Configuración principal del proyecto
├── vacunacion/             # Aplicación principal
│   ├── templates/          # Plantillas HTML semánticas
│   ├── static/             # Archivos estáticos (CSS, JS, imágenes)
│   ├── models.py           # Modelos de la base de datos
│   └── views.py            # Lógica de la aplicación
├── static/                 # Archivos estáticos globales
├── env/                    # Entorno virtual
├── requirements.txt        # Dependencias del proyecto
└── manage.py              # Script de gestión de Django
```

## Configuración de la Base de Datos 🗄️
El proyecto está configurado para usar MySQL. Asegúrate de tener las siguientes variables en tu archivo `.env`:
```
DB_NAME=nombre_de_tu_base_de_datos
DB_USER=usuario
DB_PASSWORD=contraseña
DB_HOST=localhost
DB_PORT=3306
```

## Funcionalidades Principales 🛠️
1. **Gestión de Propietarios**
   - Registro de nuevos propietarios
   - Actualización de información personal
   - Visualización de historial de mascotas

2. **Gestión de Mascotas**
   - Registro de nuevas mascotas
   - Control de vacunación
   - Historial médico

3. **Sistema de Vacunación**
   - Registro de vacunas aplicadas
   - Calendario de vacunación
   - Recordatorios automáticos

4. **Panel Administrativo**
   - Gestión de usuarios
   - Control de citas
   - Reportes y estadísticas

## HTML Semántico y Accesibilidad Web 🌐

### Implementación de HTML Semántico
El proyecto implementa HTML semántico para mejorar la estructura, accesibilidad y SEO de la aplicación:

- **Estructura de Página**
  - `<header>`: Contiene el logotipo, navegación principal y barra de búsqueda
  - `<nav>`: Implementado para menús de navegación principales y secundarios
  - `<main>`: Engloba el contenido principal de cada página
  - `<section>`: Divide el contenido en secciones lógicas (registro, historial, etc.)
  - `<article>`: Utilizado para contenido independiente como tarjetas de mascotas
  - `<aside>`: Implementado para información complementaria y widgets
  - `<footer>`: Contiene información de contacto, enlaces de interés y derechos de autor

- **Elementos Semánticos Específicos**
  - `<figure>` y `<figcaption>`: Para imágenes de mascotas con sus descripciones
  - `<time>`: Utilizado para fechas de vacunación y citas
  - `<address>`: Para información de contacto de la clínica
  - `<details>` y `<summary>`: Implementados en secciones expandibles de FAQ

### Mejoras de Accesibilidad
- **Atributos ARIA**
  - Roles ARIA para componentes interactivos
  - Estados y propiedades ARIA para mejorar la navegación con lectores de pantalla
  - Landmarks ARIA para facilitar la navegación por secciones

- **Formularios Accesibles**
  - Etiquetas `<label>` correctamente asociadas con campos de formulario
  - Mensajes de error accesibles y descriptivos
  - Agrupación lógica con `<fieldset>` y `<legend>`

- **Contraste y Tipografía**
  - Relación de contraste mínima de 4.5:1 para texto normal
  - Tamaños de fuente adaptables y legibles
  - Posibilidad de aumentar el tamaño del texto sin pérdida de funcionalidad

- **Navegación por Teclado**
  - Orden de tabulación lógico y coherente
  - Indicadores visuales de enfoque para usuarios de teclado
  - Atajos de teclado para funciones principales

### Beneficios Implementados
- Mejor experiencia para usuarios con discapacidades visuales, motoras o cognitivas
- Mayor compatibilidad con tecnologías de asistencia
- Mejora en el posicionamiento SEO
- Código más mantenible y estructurado
- Experiencia de usuario mejorada para todos los visitantes

## Seguridad 🔒
- Implementación de autenticación de usuarios
- Protección contra CSRF
- Manejo seguro de sesiones
- Variables de entorno para datos sensibles

## Contribución 🤝
Si deseas contribuir al proyecto:
1. Haz un Fork del repositorio
2. Crea una nueva rama (`git checkout -b feature/nueva-caracteristica`)
3. Realiza tus cambios y haz commit (`git commit -am 'Añadir nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Crea un Pull Request

## Autores ✒️
- Kevin Alexander Chanchi Lopez
- Carlos Andres Montoya Hoyos
- Abel Audino Pantoja Rodriguez

 😊