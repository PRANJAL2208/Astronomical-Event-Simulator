# 🌌 Astronomical Event Simulator

**Simulating Galaxy Formation with Physics and AI**

---

## 📝 Abstract

The Astronomical Event Simulator predicts the course of galaxy formation by integrating Machine Learning (ML) techniques and mathematical models, while rigorously adhering to astrophysical principles such as conservation of energy and momentum. The project evolved from regression-based orbit prediction to a robust framework combining:
- 🚀 An **Explosion Model** (Big Bang simulation),
- 🌠 **Gravitational Clustering**,
- 🌌 **N-Body Simulation** using High Performance Computing (HPC) support.

The simulator produces physically accurate visualizations of galaxy formation and celestial interactions, paving the way for future inclusion of dark matter and reinforcement learning for dynamic cosmic evolution.

---

## 🔧 Project Structure

```
.
├── checknbodyproc.py        # Orchestrates multiprocessing simulation runs
├── exp.py                   # Generates celestial fragments via Big Bang logic
├── planet.py                # Core `planet` class with position and velocity updates
├── spectralcluster.py       # Optional spectral clustering using gravitational influence
├── test.py                  # Gravitational clustering and CSV-to-planet parser
├── planets.csv              # Input dataset of planetary bodies (mass, position, velocity)
├── *.pyc                    # Compiled bytecode files (auto-generated)
```

---

## 🚀 Methodology

### 1. Explosion Model (📂 `exp.py`)
- Simulates a Big Bang-like event
- Generates random celestial fragments with mass, velocity, and position
- Outputs: list of planet objects and 3D animation of particle dispersal

### 2. Clustering Algorithms (📂 `test.py`, `spectralcluster.py`)
- **Gravitational Clustering**: Assigns planets to galaxies based on mass and proximity
- Evaluated against K-Means and DBSCAN, which failed to capture physical dependencies

### 3. N-Body Simulation (📂 `checknbodyproc.py`)
- Simulates gravitational interaction among clustered planets
- Uses `matplotlib` to animate galaxy evolution
- Multiprocessing accelerates simulation across galaxy clusters

---

## 📈 Results

✅ Improved simulation accuracy after moving from ML regression to physics-based modeling  
✅ Galaxy structures form naturally through gravitational clustering  
✅ Planetary orbits evolve realistically over time, adhering to:
- Newton’s Laws of Motion  
- Law of Universal Gravitation  
- Conservation of Momentum & Energy  

---

## 🖥️ How to Run

### Run Full Galaxy Formation Simulation

```bash
python checknbodyproc.py
```

### Run Explosion Model Only

```bash
python exp.py
```

### Run Gravitational Clustering Test

```bash
python test.py
```

---

## 📦 Requirements

```bash
pip install numpy pandas matplotlib scikit-learn
```

---

## 📊 Dataset Format (`planets.csv`)

Your CSV should include:

- `Mass`
- `Position_x`, `Position_y`, `Position_z`
- `Velocity_x`, `Velocity_y`, `Velocity_z`

Example:

| Mass | Position_x | Position_y | Position_z | Velocity_x | Velocity_y | Velocity_z |
|------|------------|------------|------------|------------|------------|------------|
| 4.2  | 1.0        | -2.1       | 0.5        | 0.1        | 0.03       | 0.2        |

---

## 🎯 Future Work

- 🌌 Incorporate **dark matter** effects for realism
- 🤖 Add **reinforcement learning** to simulate evolving galaxies
- 💻 HPC-based acceleration for simulating larger star systems
- 🌟 Include stellar evolution, black holes, and supernovae for long-term cosmic modeling

---

## 👨‍👩‍👧‍👦 Team Members

- Prateek  
- Arjun  
- Pranjal  
- Surbhi  

---

## 📚 References

1. [NASA Open Data](https://data.nasa.gov/)  
2. *Orbital Mechanics for Engineering Students* – H.D. Curtis  
3. [Scholarpedia: N-body simulations](http://www.scholarpedia.org/article/N-body_simulations_(gravitational))  
4. [Galaxy Formation by Malcolm S. Longair](https://www.cambridge.org/core/books/galaxy-formation/)

---

## 📽️ Presentation

🎥 View project presentation on Canva:  
[Canva Slide Deck](https://www.canva.com/design/DAGXv-0oGkI/LLVv1jQCr-Aw9J_zRCmoyA/edit?utm_content=DAGXv-0oGkI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

---

## 📝 License

This project is released under the MIT License.
