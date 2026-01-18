# 3D_Plots_using_Plotly_Libraries

This project demonstrates how to create **interactive 3D visualizations** using Plotly. A single figure combines three different 3D plot types:
- **3D Line** (sin–cos curve)
- **3D Scatter** (individual points)
- **3D Surface** (wave-like surface generated from a mathematical function)

---

## What this visualization shows

### 1) 3D Line Plot
- Uses a smooth curve based on:
  - `y = sin(x)`
  - `z = cos(x)`
- Helps visualize how two functions vary together in 3D space.

### 2) 3D Scatter Plot
- Shows separate 3D points (markers).
- Useful for visualizing 3D data samples or coordinates.

### 3) 3D Surface Plot
- Builds a surface using a meshgrid and a function:
  - `z = sin(sqrt(x² + y²))`
- Useful for terrain-like plots, heat surfaces, or mathematical visualizations.

---

## Data Used

### Line Data
- `x = np.linspace(0, 10, 50)`
- `y = sin(x)`
- `z = cos(x)`

### Scatter Data
- A small set of fixed points:
  - `x = [1, 2, 3, 4]`
  - `y = [2, 3, 1, 5]`
  - `z = [5, 3, 6, 2]`

### Surface Data
- 2D grid created using `meshgrid`:
  - `x_surface` and `y_surface` from `-5` to `5`
- Surface function:
  - `z_surface = sin(sqrt(x_surface² + y_surface²))`

---

## Key Concepts Used
- **`go.Scatter3d`** for 3D line and scatter plots
- **`go.Surface`** for 3D surface plots
- **Combining multiple traces** inside a single `go.Figure`
- **Scene axis labels** using `scene=dict(...)`
- **Interactive view** (rotate/zoom/pan inside the plot)

---

## Libraries Used

- `plotly.graph_objects`  
  Used to create 3D plots: `Scatter3d`, `Surface`, and `Figure`

- `numpy`  
  Used to generate numeric values, ranges, meshgrids, and apply math functions

---

## Output
- An interactive 3D figure titled: **"3D Plot Examples Using Plotly"**
- Contains:
  - 3D Line
  - 3D Scatter points
  - 3D Surface wave plot

---

## Developer
Grishma C.D
