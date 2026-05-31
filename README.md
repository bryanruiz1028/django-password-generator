# 🔑 Django Professional Password Generator

Una aplicación web robusta, segura y moderna que permite generar contraseñas seguras y aleatorias basadas en parámetros configurables elegidos por el usuario. Desarrollada en **Python** utilizando el framework de alto rendimiento **Django** y estilizada estéticamente con **Bootstrap**.

[![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.x-green?style=flat-square&logo=django)](https://www.djangoproject.com/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.x-purple?style=flat-square&logo=bootstrap)](https://getbootstrap.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

---

## 🌟 Características Clave

*   **Configuración a Medida:** Genera contraseñas personalizadas ajustando parámetros en tiempo real:
    *   **Longitud de Contraseña:** Desde 6 hasta 50 caracteres para máxima seguridad.
    *   **Inclusión de Mayúsculas:** Incorpora caracteres alfabéticos de la A a la Z.
    *   **Inclusión de Números:** Añade dígitos numéricos del 0 al 9.
    *   **Inclusión de Caracteres Especiales:** Inserta símbolos especiales seguros (`!`, `@`, `#`, `$`, `%`, etc.).
*   **Lógica Criptográfica Segura:** Implementa algoritmos de aleatoriedad robusta en Python para evitar patrones predecibles.
*   **Interfaz Responsiva y Limpia:** Estilizada con componentes modernos de **Bootstrap 5**, optimizada para visualización móvil e interactiva.
*   **Botón de Copiado Rápido:** Copia al portapapeles con un solo clic para máxima facilidad de uso.

---

## 🛠️ Tecnologías y Arquitectura

*   **Lenguaje Backend:** Python 3
*   **Web Framework:** Django (Mapeo de rutas, controlador de vistas MVT).
*   **Frontend UI:** Bootstrap 5 (CSS & JS) y HTML5 Semántico.
*   **Lógica de Generación:** Módulo nativo `random` y manipulación estructurada de arreglos ASCII.

---

## 🚀 Instalación y Despliegue Local

Sigue estos pasos para desplegar y correr la aplicación en tu servidor local:

### 1. Requisitos Previos
Asegúrate de tener instalado Python 3.9 o superior en tu sistema.

### 2. Clonar el Repositorio
```bash
git clone https://github.com/bryanruiz1028/django-password-generator.git
cd django-password-generator
```

### 3. Crear y Activar un Entorno Virtual (Opcional, pero Recomendado)
En PowerShell (Windows):
```powershell
python -m venv venv
.\venv\Scripts\Activate
```

En Linux/MacOS:
```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Instalar Dependencias
```bash
pip install -r requirements.txt
# O alternativamente:
pip install django
```

### 5. Correr Migraciones de Django
```bash
python manage.py migrate
```

### 6. Iniciar el Servidor de Desarrollo
```bash
python manage.py runserver
```
El servidor se iniciará en `http://127.0.0.1:8000/`. Abre esta URL en tu navegador.

---

## 📂 Estructura del Proyecto

```text
password_generator/         # Directorio raíz del proyecto Django
├── generator/              # Directorio de la aplicación (App)
│   ├── templates/          # Plantillas HTML estructuradas
│   │   └── generator/
│   │       ├── home.html   # Página principal con el formulario
│   │       └── password.html # Muestra la contraseña generada
│   ├── views.py            # Vistas lógicas (Generador de contraseñas)
│   └── apps.py
├── password_generator/     # Configuración central de Django
│   ├── settings.py         # Ajustes globales
│   ├── urls.py             # Mapeo de rutas URL de la aplicación
│   └── wsgi.py
└── manage.py               # Comando administrativo de Django
```

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.
