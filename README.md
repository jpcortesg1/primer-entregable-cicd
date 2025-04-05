# CI/CD Pipeline Project

Este proyecto demuestra la implementación de un pipeline de Integración Continua y Entrega Continua (CI/CD) utilizando GitHub Actions.

## Componentes del Proyecto

### 1. Script Python (main.py)
El script `main.py` es una aplicación simple que muestra información del sistema:
- Sistema operativo y su versión
- Fecha y hora actual

### 2. Workflow de GitHub Actions (.github/workflows/mi_workflow.yml)
El workflow está configurado para:
- Ejecutarse automáticamente en los siguientes eventos:
  - Push a la rama main
  - Pull requests a la rama main
  - Manualmente (workflow_dispatch)
- Realizar las siguientes acciones:
  - Imprimir un mensaje personalizado
  - Mostrar la fecha y hora actual
  - Configurar Python 3.11
  - Ejecutar el script main.py

## Cómo Usar

1. Clona este repositorio
2. El workflow se ejecutará automáticamente cuando:
   - Haces push a la rama main
   - Creas un pull request a la rama main
3. También puedes ejecutar el workflow manualmente desde la pestaña "Actions" en GitHub

## Requisitos

- Python 3.11
- Acceso a GitHub Actions

## Autores

- Juan Pablo Cortés
- Juan Esteban Cardona

## Estructura del Proyecto

```
.
├── .github/
│   └── workflows/
│       └── mi_workflow.yml
├── main.py
└── README.md
```