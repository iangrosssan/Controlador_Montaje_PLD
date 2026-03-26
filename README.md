# Montaje PLD (Controlador de Motores Ópticos)

Parametrización de motores ópticos para calibración en proyecto Capstone. Este software permite el control de un lente con dos ejes motorizados para la deposición de películas delgadas mediante láser pulsado (PLD).

## 🎯 Metas del Proyecto

1. **Interfaz Gráfica Sencilla**: Utilización de PyQt5 para proveer de una herramienta de control interactiva (con rutinas de conexión y calibración).
2. **Automatización de Calibración**: Establecer el rango de operación el los ejes X e Y mediante el movimiento de los dos ejes motorizados.
3. **Soporte de Rutinas Automáticas**: Ejecutar rutinas recurrentes (ej: movimiento de vaivén cronometrado) de forma desatendida.

## 🚀 Módulos Actuales

### 1. Interfaz de Usuario (Frontend)

**Estado:** *Completado*

- Ventanas modulares para conexión (`w_connect`) y calibración (`w_calibrate`).
- Estilizado de la UI con QSS para una mejor visualización.

### 2. Lógica de Control (Backend)

**Estado:** *Funcional*

- Conexión al hardware a través de controladores virtuales.
- Definición de clases, manejo de teclado y rutinas de movimiento repetitivo.
- Ejecución de perfil "Timed Back and Forth" para uno o dos ejes de forma simultánea.

### 3. Modos Experimentales

- Uso interactivo para pruebas rápidas mediante `Jupyter_Controlador.ipynb`.

## 🛠 Instalación y Uso

### Requisitos

- Python 3.x
- PyQt5

### Inicio Rápido

```bash
python3 main.py
```

## 📁 Estructura del Proyecto

```text
zzz-Controlador_Montaje_PLD/
├── frontend/                  
├── backend/                   
├── Jupyter_Controlador.ipynb  
└── main.py                    
```
Vea el archivo `structure.txt` para conocer la organización detallada del código en el repositorio.
