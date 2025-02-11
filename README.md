# Evolutionary Multi-Objective Optimization Algorithms (EMOA) Benchmarking

This project implements and compares various Evolutionary Multi-Objective Optimization Algorithms (EMOA) using the pymoo framework. The implementation includes benchmarking of popular algorithms against well-known test problems and provides an interactive visualization platform.

## Algorithms Implemented

The following state-of-the-art EMOAs are evaluated:

- NSGA-II (Non-dominated Sorting Genetic Algorithm II)
- NSGA-III (Non-dominated Sorting Genetic Algorithm III)
- MOEA/D (Multi-objective Evolutionary Algorithm Based on Decomposition)
- R-NSGA-II (Reference Point Based NSGA-II)
- SPEA2 (Strength Pareto Evolutionary Algorithm 2)

## Test Problems

The algorithms are tested against the following benchmark problems:

- ZDT Test Suite:
  - ZDT1 (Convex Pareto Front)
  - ZDT2 (Non-convex Pareto Front)
  - ZDT3 (Disconnected Pareto Front)
- DTLZ Test Suite:
  - DTLZ1 (Linear Pareto Front)
  - DTLZ2 (Spherical Pareto Front)

## Technologies Used

- **Backend:**
  - Python 3.8+
  - pymoo (Optimization Framework)
  - Flask (Web Framework)
  - NumPy (Numerical Computations)
  - pandas (Data Management)

- **Frontend:**
  - HTML5
  - CSS3
  - JavaScript
  - Plotly.js (Interactive Visualizations)

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/MOObyMOEA.git
cd MOObyMOEA.git

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required packages
pip install -r requirements.txt
```

## Usage

1. Start the Flask server:
```bash
python3 app.py
```

2. Access the web interface at `http://localhost:5000`

3. Select the desired:
   - Algorithm
   - Test problem
   - Number of generations
   - Population size
   - Other algorithm-specific parameters

4. View and interact with the results through the visualization dashboard

## Project Structure

```
emoa-benchmarking/
├── app.py                 # Flask application
├── requirements.txt       # Project dependencies
├── static/               # Static files
│   ├── css/             # Stylesheets
│   ├── js/              # JavaScript files
│   └── images/          # Images and icons
├── templates/           # HTML templates
├── algorithms/          # EMOA implementations
├── problems/           # Test problem implementations
└── utils/              # Utility functions
```

## Features

- Interactive comparison of different EMOAs
- Real-time visualization of:
  - Pareto fronts
  - Convergence metrics
  - Population diversity
- Performance metrics calculation:
  - Hypervolume
  - IGD (Inverted Generational Distance)
  - Spread
- Export results in various formats (CSV, JSON)
- Customizable algorithm parameters
- Responsive web interface

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- ## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. -->

## Acknowledgments

- pymoo development team
- Multi-objective optimization research community
- Flask and Plotly.js contributors

<!-- ## Citation

If you use this project in your research, please cite:

```bibtex
@software{emoa_benchmarking,
  author = {Your Name},
  title = {EMOA Benchmarking: A Comparative Study of Evolutionary Multi-Objective Optimization Algorithms},
  year = {2025},
  url = {https://github.com/yourusername/MOObyMOEA}
}
``` -->