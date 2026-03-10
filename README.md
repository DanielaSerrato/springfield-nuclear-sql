# Curso de SQL – Springfield Nuclear

Este repositorio contiene todos los recursos para un curso de SQL utilizando un dataset ficticio de una planta nuclear. Está pensado para facilitar la distribución del material a tus estudiantes y que puedan comenzar a practicar de inmediato.

## Estructura de carpetas

```
springfield_nuclear_repo/
├── datasets/
│   └── springfield_nuclear.sql   # Script para crear y poblar la base de datos.
├── clases/                       # Lugar para scripts y ejemplos usados en clase.
├── talleres/                     # Ejercicios propuestos para los estudiantes.
└── soluciones/                   # Soluciones a ejercicios (manténlo vacío hasta publicarlos).
```

### datasets/springfield_nuclear.sql

El script SQL crea la base de datos `springfield_nuclear`, todas sus tablas y carga datos de ejemplo. Es un único archivo para asegurar reproducibilidad.

## Cómo cargar el dataset

Estos son los pasos recomendados para que los estudiantes instalen y carguen la base de datos en sus equipos:

1. **Instalar MySQL y Workbench**  
   Descarga e instala MySQL Server y MySQL Workbench desde la página oficial (https://dev.mysql.com/downloads/installer/).

2. **Abrir MySQL Workbench**  
   Conéctate a `Local instance MySQL` usando el usuario root y la contraseña configurada durante la instalación.

3. **Abrir el script**  
   Selecciona *File → Open SQL Script* y abre `datasets/springfield_nuclear.sql`.

4. **Ejecutar el script**  
   Ejecuta todo el contenido con el botón del rayo (⚡) o con `Ctrl + Shift + Enter`.

5. **Verificar que los datos estén cargados**  
   Ejecuta en la consola:

   ```sql
   SHOW DATABASES;
   USE springfield_nuclear;
   SHOW TABLES;
   SELECT * FROM empleados LIMIT 5;
   ```

   Si ves registros, la carga fue exitosa.

> **Tip**: El script incluye `DROP DATABASE IF EXISTS springfield_nuclear;` al inicio para que los estudiantes puedan volver a ejecutar el script sin problemas si necesitan reiniciar.



Este material se proporciona con fines educativos. Puedes adaptarlo libremente para tus clases.
