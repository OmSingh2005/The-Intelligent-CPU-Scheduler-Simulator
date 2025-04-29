# The Intelligent CPU Scheduler Simulator

<!--- ![CPU Scheduler Banner](https://via.placeholder.com/800x200?text=CPU+Scheduler+Simulator) --->

> A practical CPU scheduling simulation tool with real-time visualization, heuristic suggestions, and test-based conclusions for various scheduling algorithms. Built to support training AI/ML prediction models using large-sample-test methods.

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🔍 Overview

This project is a comprehensive CPU scheduling simulator designed for:
- **Educational purposes** - Visualize how different CPU scheduling algorithms work
- **Performance analysis** - Compare metrics across algorithms to determine optimal solutions
- **AI/ML research** - Generate datasets for training predictive models for dynamic scheduling
- **Heuristic evaluation** - Get suggestions for the best algorithm based on process characteristics

## ✨ Features

### 📊 Visualization
- **Interactive Gantt Charts** for both preemptive and non-preemptive algorithms
- **Real-time process execution** visualization
- **Performance metrics** displayed graphically

### 🧠 Algorithm Implementation
#### Currently Implemented:
- **First Come First Serve (FCFS)** - Non-preemptive
- **Shortest Job First (SJF)** - Non-preemptive
- **Round Robin (RR)** - Preemptive
- **Priority Scheduling** - Non-preemptive
- **Shortest Remaining Time First (SRTF)** - Preemptive

### 📈 Analysis Tools
- **Performance Metrics**:
  - Average Waiting Time
  - Average Turnaround Time
  - Average Response Time
  - CPU Utilization
- **Comparative Analysis** across algorithms
- **Heuristic Algorithm Suggestions** based on workload characteristics

### 🧪 Testing & Data Generation
- **Large Sample Testing** framework
- **Sample & Population Data** generators for AI/ML training
- **Statistical Analysis** of algorithm performance

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Required libraries (matplotlib, numpy, pandas, tkinter)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/OmSingh2005/The-Intelligent-CPU-Scheduler-Simulator.git
cd The-Intelligent-CPU-Scheduler-Simulator
```

2. Install dependencies:
```bash
pip install -r docs/requirements.txt
```

3. Run the simulator:
```bash
python src/main.py
```

## 📁 Project Structure

```
/src
  |--- algorithms.py          # Scheduling algorithms implementations
  |--- gui.py                 # GUI implementation with tkinter
  |--- visualization.py       # Visualization components (Gantt charts, metrics)
  |--- main.py                # Entry point for the application
  |--- suggest_algorithm.py   # Heuristic Methods for algorithm suggestions
/tests
  |--- LargeSampleGraph.py    # Graph visualization for large datasets
  |--- test_rr.py             # Round Robin algorithm test cases
  |--- test_srtf.py           # SRTF algorithm test cases
  |--- test_suggest_algorithm.py # Heuristics testing
  |--- datagen.py             # Sample & Population Data Generator
  |--- SamplePr.xlsx          # Population DataSet for tests
  |--- RandSamples.xlsx       # Sample population generator
/docs
  |--- README.md              # Documentation
  |--- requirements.txt       # Required Libraries
```

## 🖥️ Usage

### Basic Simulation
1. Launch the application
2. Enter process details (arrival time, burst time, priority if needed)
3. Select a scheduling algorithm
4. Click "Run Simulation"
5. View the Gantt chart and performance metrics

### Advanced Features
- **Algorithm Suggestions**: Use the "Suggest Algorithm" feature for optimal scheduling
- **Large Dataset Testing**: Run tests with the included sample datasets
- **Custom Dataset Generation**: Create your own process datasets for testing

## 📊 Example Results

Here's an example of the simulator in action, showing a Gantt chart for the Round Robin algorithm:

Performance metrics comparison:

| Algorithm | Avg. Waiting Time | Avg. Turnaround Time | Avg. Response Time |
|-----------|-------------------|----------------------|-------------------|
| FCFS      | 10.5              | 15.2                 | 10.5              |
| SJF       | 6.2               | 10.9                 | 6.2               |
| SRTF      | 5.8               | 10.5                 | 2.3               |
| RR (q=2)  | 9.1               | 13.8                 | 4.2               |
| Priority  | 8.7               | 13.4                 | 8.7               |

Also a initial dashboard sample snapshot
![Sample Gantt Chart](https://i.imgur.com/V869ULC.png)

## 🔮 Future Enhancements

- **Priority Scheduling (Preemptive)** implementation
- **AI/ML Integration** for dynamic scheduling algorithm selection
- **Advanced Heuristics** for better algorithm suggestions
- **Enhanced GUI** with more interactive features
- **Multi-core Simulation** capabilities
- **Process Dependencies** and resource constraints

## 🤝 Contributing

We welcome contributions to improve the simulator! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 👥 Contributors

- **[Shivam Yadav](https://github.com/Shivamsdr)**
- **[Om Singh Chauhan](https://github.com/OmSingh2005)**
- **[Aryan Kumar](https://github.com/AryanKumarLpu)**

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- Thanks to all the contributors who have helped with the development
- Special appreciation to operating systems textbook authors whose algorithms we've implemented
- The open-source community for providing tools and libraries used in this project

---

*Feel free to suggest improvements, report issues, or contribute to this project. If you have ideas for adding AI/ML-based enhancements, let's collaborate!*
