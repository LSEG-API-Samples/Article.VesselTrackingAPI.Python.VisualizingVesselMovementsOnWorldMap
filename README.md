# Visualizing Vessel Movements on a World Map with the Vessel Tracking API and Python

This project retrieves historical vessel positions from the Vessel Tracking API and visualizes the route as a static map and animated GIF.

## Prerequisites

- Python 3.10 or later
- Visual Studio Code with the Jupyter extension
- A Vessel Tracking API key

## Installation

Install the required packages:

```powershell
py -m pip install --upgrade pip
py -m pip install -r requirements.txt
```

## API configuration

Create a `config.ini` file in the same directory as the notebook:

```ini
[vessel_tracking]
api_key = apikey-v1 YOUR_API_KEY
```

Do not commit this file. Add it to `.gitignore`:

```gitignore
config.ini
.venv/
*.gif
```

## Run the notebook

Open `vessel-movement-visualization.ipynb` and run its cells in order.

The notebook will:

1. Retrieve historical vessel positions.
2. Clean and order the returned data.
3. Plot the route on a map.
4. Create and save an animated GIF.
