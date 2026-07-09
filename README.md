# Plant bending analysis

This project contains two self-contained Jupyter notebooks for plant stem bending and cross-section flexural stiffness calculations:

- The [cantilever_beam_plant_model.ipynb](https://github.com/tristanmontoya/plant-bending-analysis/blob/main/cantilever_beam_plant_model.ipynb) notebook builds a concentric-layer stem geometry from pith, vascular, and ground tissue thicknesses, computes the flexural stiffness from the layer radii and moduli, solves for the cantilever beam response under a distributed load, and plots the stem radius profile and beam deflection.
- The [offset_ring_flexural_stiffness.ipynb](https://github.com/tristanmontoya/plant-bending-analysis/blob/main/offset_ring_flexural_stiffness.ipynb) notebook computes the elastic neutral axis and flexural stiffness for offset rings with different elastic moduli.

## Setup

Clone this repository and change into the project directory:

```bash
git clone https://github.com/tristanmontoya/plant-bending-analysis.git
cd plant-bending-analysis
```

Create `.venv` and install the pinned notebook environment:

```bash
python -m venv .venv
.venv/bin/pip install -r requirements.txt
```

The pinned environment is listed in `requirements.txt`, which includes:

- NumPy
- SciPy
- Matplotlib
- ipykernel
- notebook

## Usage

Start Jupyter Notebook from the project environment:

```bash
.venv/bin/jupyter notebook
```

Then open either notebook in the browser and select the
`.venv` Python kernel if needed.
