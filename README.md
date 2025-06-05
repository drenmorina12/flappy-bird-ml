# Flappy Bird ML

A Python implementation of the classic Flappy Bird game, enhanced with **machine learning** using the **NEAT** (NeuroEvolution of Augmenting Topologies) algorithm. You can either play the game yourself or watch an AI agent learn to play the game entirely on their own, evolving smarter behaviors over multiple generations.

---

## 🧠 How AI Mode Works

- Each bird is controlled by a simple **neural network** evolved using NEAT.
- Birds observe:
  - Their vertical position
  - The distance to the next pipe (top and bottom)
- The fittest birds (those that survive longer and pass pipes) are rewarded, and the next generation is evolved from them.

---

## 📦 Features

- **AI Mode**: Let the AI play the game.
- **Human Mode**: Play Flappy Bird yourself using the spacebar.
- NEAT-Python powered evolution
- Fully animated Flappy Bird gameplay (pygame)
- Dynamic pipe generation and collision detection
- Fitness scoring and selection
- **Visual feedback**: score and generation number on-screen
- Configurable population and mutation parameters
- **Switch Modes Easily**: One file, two modes.
---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3 and `pip` installed.

### Installation

1. Clone this repository:

```bash
git clone https://github.com/drenmorina12/flappy-bird-ml.git
cd flappy-bird-ml
```

2. Install required dependencies:

```bash
pip install -r requirements.txt
```

3. Run the game:

```bash
python main.py
```

---

## ⚙️ Mode Switching

Open `main.py` and change the value of the `MODE` variable at the top of the file:

```python
MODE = "ai"     # Let the AI play the game
# MODE = "human"  # Uncomment to play yourself
```

Choose between:
- `"ai"` - NEAT-based autonomous learning
- `"human"` - Classic spacebar-controlled game

---

## 🔧 Configuration

### Change Jump Velocity

In `main.py`, modify the `JUMP_VEL` constant near the top to adjust how high the bird jumps:

```python
JUMP_VEL = 10.5
```

### AI Settings

Tweak NEAT configurations inside `config-feedforward.txt` (e.g., population size, mutation rates, etc).

---

## 📷 Screenshots

![Screenshot](imgs/screenshot.png)

---

## 🤝 Contributing

Feel free to fork this repo and submit a pull request with enhancements or bug fixes.

---

## 📄 License

This project is licensed under the MIT License.
