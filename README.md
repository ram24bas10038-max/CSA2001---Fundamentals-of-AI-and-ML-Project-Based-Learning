# Autonomous Delivery Agent

## Project Overview

This project implements an *Autonomous Delivery Agent* that navigates a 2D grid-based city to deliver packages efficiently. The agent is designed to behave rationally, choosing actions that maximize delivery efficiency and dynamically replanning when necessary. It utilizes foundational AI search algorithms such as *BFS, UCS, and A\** for navigation and decision-making.

---

## Features

- *Grid-based City Simulation:* Representing city blocks, obstacles, and delivery locations.
- *Rational Agent:* Selects optimal routes and actions to maximize delivery efficiency.
- *Dynamic Replanning:* Adapts to changes in the environment (e.g., new obstacles or deliveries).
- *Multiple Search Algorithms:* Supports BFS, UCS, and A* for pathfinding.
- *Well-documented Source Code:* Easy to read, understand, and extend.
- *Test Maps:* Includes small, medium, large, and dynamic test scenarios.

---

## Directory Structure


autonomous-delivery-agent/
├── main.py              # Entry point, demonstration, and dynamic replanning
├── agent.py             # Agent logic and search algorithms
├── environment.py       # Grid and environment configuration
├── maps/                # Sample test maps (small, medium, large, dynamic)
├── README.md            # Project documentation (this file)
└── report.pdf           # Short report (model, design, results, analysis)


---

## Setup and Dependencies

- *Python 3.x* is required.
- The following libraries are used (all part of the Python standard library):
  - argparse : For handling command-line arguments
  - heapq    : For priority queue in A* and UCS
  - collections.deque : For queue implementation in BFS

### Installation

No external packages are needed. To clone and run:

bash
git clone https://github.com/siddujain525-star/autonomous-delivery-agent.git
cd autonomous-delivery-agent
python main.py --help


---

## Usage

Run the main script with optional arguments to specify maps and algorithms:

bash
python main.py --map maps/small.txt --algorithm astar


- --map        : Path to the test map file (e.g., maps/medium.txt)
- --algorithm  : Search algorithm to use (bfs, ucs, astar)

### Output

- The script will print the path, actions taken, and demonstrate dynamic replanning in case of environment changes.

---

## Deliverables

- *Source Code:* All source code files are well-documented and organized.
- *Test Maps:* Four test maps are included in the maps/ directory:
  - small.txt
  - medium.txt
  - large.txt
  - dynamic.txt
- *Report:* A short report detailing the environment model, agent design, experimental results, and analysis (report.pdf).
- *Demonstration:* Dynamic replanning showcased in the main.py script's output log.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with improvements or bug fixes.

---

## License

This project is released under the MIT License.

---

## Authors

- [siddujain525-star](https://github.com/siddujain525-star)

---

## Acknowledgments

- Inspired by AI search algorithms and rational agent design principles.
