# Práctica: Gestión de Hilos (POSIX Threads)

## Descripción
Este proyecto implementa rutinas en lenguaje C para la creación, gestión y sincronización de hilos concurrentes utilizando la biblioteca `pthread` en un entorno Linux. Demuestra las diferencias de rendimiento entre ejecuciones secuenciales y concurrentes, así como el uso de exclusión mutua (Mutex) para evitar condiciones de carrera.

## Objetivos
- Instanciar múltiples hilos en un solo proceso.
- Proteger secciones críticas mediante el uso de Mutex.
- Analizar el impacto de la concurrencia y la sobrecarga del sistema (*overhead*) en los tiempos de ejecución.

## Tecnologías Utilizadas
- Lenguaje: C
- Compilador: GCC
- Biblioteca: POSIX Threads (`pthread`) y `<time.h>`
- SO objetivo: Linux / UNIX-like

## Instrucciones de Compilación
El proyecto incluye diferentes versiones del código en la carpeta `src/`. Para compilar cualquiera de ellos, abre la terminal y asegúrate de incluir la bandera `-lpthread`.

Ejemplo:
```bash
gcc -o bin/hilos_rendimiento src/hilos_rendimiento.c -lpthread