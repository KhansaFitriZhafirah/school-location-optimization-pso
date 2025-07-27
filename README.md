# 🧭 Optimizing School Location Using Particle Swarm Optimization: A Case Study in Wonomerto Village

This project utilizes the Particle Swarm Optimization (PSO) algorithm to determine the optimal location for a new high school in Wonomerto Village, Indonesia. By processing spatial data extracted from OpenStreetMap, the project aims to minimize the average travel distance between students' homes and the proposed school. This work was developed as part of the final project for the Introduction to Computational Intelligence course at IPB University.

---

## 🎯 Project Objectives

- To implement a **swarm intelligence-based algorithm (PSO)** for spatial optimization.
- To support **data-driven decision making** in rural infrastructure planning.
- To visualize the optimal school location and demonstrate the convergence of the optimization process.

---

## 🗺️ Dataset and Tools

- **Spatial Data Source**: OpenStreetMap (via Overpass Turbo API)
- **Target Area**: Wonomerto Village, Kecamatan Bandar, Kabupaten Batang, Central Java
- **Programming Language**: Python (Google Collab/Jupyter Notebook)
- **Libraries Used**: Pandas, NumPy, Matplotlib
- **Optimization Algorithm**: Particle Swarm Optimization (custom implementation)

---

## ⚙️ Workflow Overview

1. **Data Collection**
   - Retrieve geographic coordinates of residential buildings from OpenStreetMap using Overpass Turbo.
   - Divide the village area into 3 bounding boxes to ensure complete spatial coverage.

2. **Data Preprocessing**
   - Combine coordinates from all bounding boxes.
   - Visualize data using scatter plots.

3. **PSO Implementation**
   - Initialize 30 particles with random locations.
   - Update velocities and positions using cognitive and social components.
   - Objective Function: Minimize the total Euclidean distance to all buildings.

4. **Optimization and Visualization**
   - Track convergence over 40 iterations.
   - Plot the optimal location and its connections to all houses.

---

## 📊 Key Results

- **Optimal Coordinates for New School**: `(-7.06952169, 109.79080754)`
- **Optimization Result**: A well-centered location that reduces the average travel distance from all **residents' houses**.
- **Convergence**: The PSO algorithm successfully converged after 24–40 iterations with consistent improvement.

---

## 📊 Visualization

The final visualization displays:

- The distribution of all **residents' houses**.
- The optimal school location.
- Connection lines indicating the distance between each **house**.

This provides clear insight into how the selected point minimizes access distance across the village.

---

## ✅ Future Improvements

- Integrating more real-world constraints (road access, land availability).
- Extending to multi-school scenarios using hierarchical optimization.
