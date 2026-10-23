# Proyecto: Control de Acceso y Gestión de Memoria RAM con Punteros — LPR 2026

**Escuela de Educación Secundaria Técnica N° 1 — Vicente López**  
**Curso:** 5° Año 3° División — Especialidad Computación / Programación  
**Materia:** Laboratorio de Programación (LPR)  
**Profesor:** Prof. York Mansilla Muñoz & Prof. Yamil  
**Estudiante:** Alexander Luca Veit

## 📌 Descripción de la Actividad

Esta actividad aborda la gestión directa de memoria RAM mediante el uso de punteros en C++. Se desarrolla una aplicación de control de acceso que manipula direcciones físicas de memoria en formato hexadecimal (`0x...`), captura datos mediante desreferenciación (`*p`), y valida condiciones de acceso operando directamente sobre las direcciones de la pila de memoria (Stack).

## 🗂 Estructura del Repositorio

```text
cadenaspunteros/
├── src/                # Código fuente y binario compilado
│   ├── main.cpp        # Código fuente en C++ con punteros
│   └── main.exe        # Ejecutable generado
├── capturas/           # Capturas de pantalla del proceso
│   ├── esquema_ram.png
│   └── ejecucion_punteros.png
├── docs/               # Documentación
│   └── InformeProyectoCADENASPUNTEROS.pdf
├── .gitignore
├── LICENSE             # Licencia MIT
└── README.md
```

## 💻 Implementación

El programa se encuentra en `src/main.cpp` y demuestra el uso de punteros para el control de acceso:

- **Declaración de puntero:** `int* p = &edad;` guarda la dirección de memoria de la variable `edad` en la pila (Stack).
- **Captura por desreferenciación:** Se utiliza `cin >> *p;` para ingresar el valor directamente en la memoria apuntada por el puntero. Esto evita sobrescribir la dirección del puntero.
- **Análisis de acceso:** Se evalúa `*p >= 18` con el valor desreferenciado para determinar si el usuario es mayor o menor de edad.
- **Visualización de memoria:** Se imprime la dirección hexadecimal (`p`) para observar la dirección física asignada en la RAM.

**Salida:** Según el resultado, muestra `[ACCESO APROBADO]` o `[ACCESO RECHAZADO]`, la edad registrada y la dirección hexadecimal en RAM.

## 🛠️ Requisitos e Instalación

Para compilar y ejecutar este proyecto en Windows 10/11:

- **Visual Studio Code:** Con las extensiones oficiales C/C++ de Microsoft.
- **Compilador MinGW (GCC/G++):** Configurado en las variables de entorno (`PATH` de Windows).
- **Git for Windows:** Para la gestión del repositorio y sincronización con GitHub.

## ▶️ Comandos para compilar y ejecutar (PowerShell - VS Code)

Asegurate de estar parado en la raíz de la carpeta `cadenaspunteros` en la terminal integrada de VS Code (`Ctrl + Ñ`).

### Compilar el código fuente con punteros

```bash
g++ src/main.cpp -o src/cadenaspunteros.exe
```

### Ejecutar la aplicación

```bash
./src/cadenaspunteros.exe
```

## 🧪 Evidencias

El repositorio incluye capturas del proceso en la carpeta `capturas/`:

- `esquema_ram.png` - Esquema del uso de punteros en memoria RAM/Stack
- `ejecucion_punteros.png` - Ejecución del programa mostrando acceso y direcciones hexadecimales

## 👤 Autor

- **Alexander Luca Veit** — Programador / Estudiante  
  GitHub: [Xen-alt10](https://github.com/Xen-alt10)  
  Repositorio: [cadenaspunteros](https://github.com/Xen-alt10/cadenaspunteros)

## 📄 Licencia

Este proyecto está bajo licencia [MIT](LICENSE). Copyright (c) 2026 Xen-alt10.
