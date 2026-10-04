# Mant_Pers_2023 - Mantenimiento de Personas

Aplicación Java para gestión de personas con acceso a ficheros de acceso directo.

## Requisitos

- Java 8 o superior
- Directorio `data/` en la raíz del proyecto (se crea automáticamente si no existe)

## Configuración

La aplicación almacena los datos en `data/personas.dat`. El directorio `data/` **debe existir** antes de ejecutar la aplicación.

### Crear el directorio data

```bash
mkdir data
```

O en Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force -Path data
```

## Ejecución

```bash
# Compilar
javac -d bin src/mantPersona/*.java

# Ejecutar
java -cp bin mantPersona.MantPersona
```

## Estructura del proyecto

```
Mant_Pers_2023/
├── src/
│   └── mantPersona/
│       ├── MantPersona.java
│       ├── Persona.java
│       └── Teclado.java
├── bin/              # Bytecode compilado (ignorado por git)
├── data/             # Directorio de datos (crear manualmente)
│   └── personas.dat  # Fichero de acceso directo
└── README.md
```

## Notas

- El archivo `personas.dat` se crea automáticamente en `data/` al ejecutar la aplicación por primera vez.
- Los archivos `.class` en `bin/` están en `.gitignore` y no deben versionarse.