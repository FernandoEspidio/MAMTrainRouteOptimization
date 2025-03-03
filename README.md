# Train Route Optimization System :steam_locomotive:

A multi-agent system designed to optimize freight train routes, **minimizing travel time** and **resource consumption**. This project integrates **Python**, **Flask**, and **Unity** to provide real-time, animated simulations of train movements.

## ✨ Key Features
- **A\* Search Algorithm**: Finds collision-free, efficient routes, prioritizing trains with higher urgency or critical cargo.
- **Multi-Agent Simulation**: Each train operates as an autonomous agent, making path decisions based on load, remaining time, and current traffic.
- **Bitmap Processing**: Converts railway images into bitmaps, feeding them into the pathfinding algorithm.
- **Flask API**: Exposes a service that calculates routes and sends data to Unity for live visualization.
- **Real-Time Unity Rendering**: Animates train positions and interactions, helping users see potential collisions and rerouting decisions immediately.

## ⚙️ Tech Stack
- **Python** (3.8+)
  - [AgentPy](https://github.com/JoelForamitti/agentpy) for multi-agent logic
  - [Flask](https://flask.palletsprojects.com/) for the API
  - Additional libraries: `numpy`, `pillow`, etc.
- **Unity** (C#) for 3D visualization
- **A\* Algorithm** for pathfinding
- **Bitmaps** for map representation

## 🏗️ Setup
1. **Clone** this repository:
   ```bash
   git clone https://github.com/<your-username>/train-route-optimization.git
# Train Route Optimization

## 🚀 Install Dependencies (Python Side)

```bash
cd train-route-optimization
python -m venv venv
source venv/bin/activate   # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

## 🖥️ Run Flask Server

```bash
python app.py
```

## 🎮 Open Unity

1. Load the `UnityProject` folder in Unity Hub.
2. In the main scene, configure the API endpoint in the relevant script.
3. Press **Play** to see trains moving on the generated paths.

## 🚆 Usage

- Configure the railway map (bitmap) and train details (number of trains, priorities, etc.) in `app.py` or a config file.
- Start the Flask server to calculate optimal routes.
- Visualize in Unity to watch each train’s real-time movement.

### The system will:

- Receive route data from Flask.
- Show collision-free paths (or indicate conflicts if rerouting is necessary).
- Provide feedback on travel times and delays.

## 📌 Example

1. Place your railway map as `rail_map.png` (or use the sample provided).
2. Adjust `config.json` to set train counts, speeds, start/end nodes, etc.
3. Run `python app.py` and launch Unity to see the results in action.

## 🔮 Future Improvements

- **Adaptive Algorithms:** Investigate alternative pathfinding methods like **D* Lite** or advanced heuristic tuning.
- **Dynamic Map Updates:** Introduce multiple maps or dynamically alter segments (e.g., construction, weather).
- **Interactive Controls:** Add Unity UI panels for pausing/resuming simulations, adjusting train priorities on the fly.

## 🤝 Contributing

1. Fork the repository and create a feature branch:
   
   ```bash
   git checkout -b feature/amazing-feature
   ```
   
2. Commit your changes and push the branch.
3. Open a **Pull Request** to merge into the main branch.

---

🚄 **Train Route Optimization** - Enhancing railway logistics with efficient routing and real-time visualization.

