# Taller Algoritmos Variacionales

Taller de bienvenida del grupo MoleQLs sobre el **Variational Quantum Eigensolver (VQE)**.

## Contenido del repositorio

- [`clase_vqe_fundamentos.pdf`](clase_vqe_fundamentos.pdf) — apunte teórico: el Hamiltoniano como operador de energía, el principio variacional, y cómo parametrizar un estado.
- [`cuadernillo_vqe.ipynb`](cuadernillo_vqe.ipynb) — cuadernillo práctico en Qiskit que acompaña la teoría: construcción del Hamiltoniano, ansatz parametrizado, optimización clásica y entrelazamiento.
- [`requirements.txt`](requirements.txt) — dependencias de Python necesarias para correr el cuadernillo.

## Instalación

### 1. Requisitos previos

- [Python 3.10](https://www.python.org/downloads/) o superior.
- [Git](https://git-scm.com/downloads).

### 2. Descargar el repositorio

Clónalo con `git`:

```bash
git clone https://github.com/JoaquinQu/Taller-Algoritmos-Variacionales.git
cd Taller-Algoritmos-Variacionales
```

O bien, descárgalo como ZIP desde GitHub (botón **Code → Download ZIP**) y descomprímelo.

### 3. Crear un entorno virtual

Desde la carpeta del repositorio:

```bash
python -m venv .venv
```

Actívalo:

- **Windows (PowerShell):**
  ```powershell
  .venv\Scripts\Activate.ps1
  ```
- **Windows (Git Bash / WSL) o macOS/Linux:**
  ```bash
  source .venv/Scripts/activate   # Windows Git Bash
  source .venv/bin/activate       # macOS/Linux
  ```

Vas a saber que quedó activo porque tu terminal muestra `(.venv)` al inicio de la línea.

### 4. Instalar las librerías

Con el entorno virtual activado, instala todo lo necesario desde `requirements.txt`:

```bash
pip install -r requirements.txt
```

Esto instala `numpy`, `scipy`, `qiskit` (con sus herramientas de visualización) y `jupyter`.

## Cómo usar el cuadernillo

Con el entorno activado, abre Jupyter:

```bash
jupyter notebook cuadernillo_vqe.ipynb
```

(o `jupyter lab` si prefieres esa interfaz). Las celdas de código se apoyan en las anteriores, así que conviene ejecutarlas en orden dentro de cada sección en vez de saltarse celdas.
