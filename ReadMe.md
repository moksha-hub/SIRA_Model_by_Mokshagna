# Learning the Susceptible-Infected-Removed (SIR) Model with Neural ODEs

This repository hosts a project aimed at deducing the deterministic dynamics of the classical SIR epidemic model using advanced machine learning techniques. The SIR model—defined by a system of ordinary differential equations (ODEs)—is fundamental in epidemiology, yet its traditional formulation often fails to capture the inherent randomness of real-world outbreaks. This project bridges that gap by training a neural ODE model on synthetic epidemic data generated via Monte Carlo and network-based simulations.

---

## Project Overview

**Objective:**  
The primary goal is to recover continuous functions S(t), I(t), and R(t) that accurately describe the evolution of susceptible, infected, and recovered populations over time. This is achieved by leveraging a large dataset of simulated epidemics, where each simulation varies key SIR parameters. By integrating auto-differentiation and symbolic methods into the training process, the model learns an interpretable representation of epidemic dynamics that can support improved predictive capabilities and public health interventions.

**Approach:**  
- **Stochastic Data Generation:**  
  Synthetic epidemic trajectories are created using Monte Carlo methods and network-based simulations, which capture the randomness and variability present in real-world scenarios.
  
- **Neural ODE Modeling:**  
  A neural ODE is trained to learn the underlying continuous dynamics from the stochastic simulation data. This model integrates techniques from deep learning and differential equations, allowing it to bridge the gap between discrete simulation outputs and smooth epidemic curves.
  
- **Experimental Automation:**  
  An automated training pipeline is implemented to systematically tune hyperparameters, ensuring reproducibility and scalability. This includes rigorous benchmarking against classical numerical solvers such as Runge-Kutta methods.

**Challenges Addressed:**  
During development, challenges such as data variability, sensitivity to hyperparameters, and numerical stability were encountered. These issues were managed through robust data pre-processing, extensive experimentation, and careful design of the neural ODE architecture.

---

## Key Features

- **Comprehensive Simulation Framework:**  
  Generate diverse epidemic scenarios through stochastic simulation techniques that mimic various outbreak conditions.

- **Interpretable Neural ODE Model:**  
  Train a neural network that learns continuous SIR dynamics, offering insights into disease progression that are interpretable and actionable.

- **Automated Experimentation:**  
  The project includes a suite of automation scripts to systematically explore different parameter settings, ensuring the model's robustness and performance are thoroughly validated.

- **Integration of Advanced Mathematical Techniques:**  
  Utilizes auto-differentiation and symbolic methods to refine the model’s approximation of the SIR dynamics, enhancing both accuracy and interpretability.

---

## Installation

To set up the project locally:
1. **Clone the Repository:**  
   Use Git to clone the project from GitHub.
2. **Install Dependencies:**  
   Install the required Python packages as specified in the requirements file.
3. **Set Up the Environment:**  
   Optionally, create a virtual environment to manage dependencies and ensure reproducibility.

---

## Usage

- **Data Simulation:**  
  Run the simulation module to generate synthetic epidemic trajectories. These simulations serve as the training data for the neural ODE model.
  
- **Model Training:**  
  Use the provided training scripts to fine-tune the neural ODE model on the simulated data. The training process leverages auto-differentiation to learn the continuous functions that define the epidemic's evolution.
  
- **Evaluation and Analysis:**  
  Evaluate the model's performance by comparing its predictions with classical ODE solutions. Visualization tools help in understanding how well the model captures the dynamics of S, I, and R over time.

---

## Contributing

Contributions to the project are highly encouraged. Whether it's improving the simulation module, enhancing the neural ODE training pipeline, or refining documentation, your input is valuable. If you wish to contribute:
- Fork the repository.
- Create a new branch for your changes.
- Submit a pull request with a clear description of your modifications.
- For major changes, please open an issue first to discuss your ideas.

---

## License

This project is open-sourced under the MIT License. All code, models, and documentation are available for further development and collaborative research.

---

## Acknowledgments

I would like to thank the mentors, the research community, and public health experts whose insights into epidemic modeling and advanced machine learning have guided this work.

---

## Contact

For any questions or feedback, please contact me at [mokshagnak004@gmail.com](mailto:mokshagnak004@gmail.com).

---

Thank you for exploring the Learning the SIR Model project. Your contributions and feedback are greatly appreciated as we work together to enhance our understanding of epidemic dynamics through innovative machine learning approaches.
