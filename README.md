# Hi, I'm Erfan 👋

MSc student at **Politecnico di Torino** working on **machine learning and reinforcement learning for energy systems**. I build ML pipelines that are tested, containerized and ready to deploy, and RL agents that stay robust when the real world doesn't match the simulator.

---

## About Me

- 🎓 MSc in Digital Skills for Sustainable Societal Transitions, Politecnico di Torino · BSc in Engineering of Urban Development
- 🤖 Reinforcement learning: SAC, PPO, REINFORCE, Actor-Critic, domain randomization, sim-to-sim transfer
- 🛠️ ML engineering: feature stores, drift monitoring, automated retraining, FastAPI serving, Docker, CI/CD
- ⚡ Energy systems: renewable power forecasting, building and district energy, co-simulation
- 🔭 Thesis: **Domain Randomization for Heatwave-Robust RL in District Energy Management**
- 💼 Open to **Machine Learning Engineer** roles
- 📍 Turin, Italy

---

## Tech Stack

### Languages
[![Python](https://img.shields.io/badge/Python-333333?style=flat&logo=python&logoColor=white)](https://www.python.org/)

### Machine Learning & RL
[![PyTorch](https://img.shields.io/badge/PyTorch-333333?style=flat&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Stable-Baselines3](https://img.shields.io/badge/Stable--Baselines3-333333?style=flat)](https://stable-baselines3.readthedocs.io/)
[![Gymnasium](https://img.shields.io/badge/Gymnasium-333333?style=flat)](https://gymnasium.farama.org/)
[![MuJoCo](https://img.shields.io/badge/MuJoCo-333333?style=flat)](https://mujoco.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-333333?style=flat&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-333333?style=flat)](https://xgboost.ai/)
[![pandas](https://img.shields.io/badge/pandas-333333?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-333333?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)
[![TensorBoard](https://img.shields.io/badge/TensorBoard-333333?style=flat&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/tensorboard)

### MLOps & Backend
[![FastAPI](https://img.shields.io/badge/FastAPI-333333?style=flat&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Docker](https://img.shields.io/badge/Docker-333333?style=flat&logo=docker&logoColor=white)](https://www.docker.com/)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-333333?style=flat&logo=githubactions&logoColor=white)](https://github.com/features/actions)
[![Feast](https://img.shields.io/badge/Feast-333333?style=flat)](https://feast.dev/)
[![Streamlit](https://img.shields.io/badge/Streamlit-333333?style=flat&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![pytest](https://img.shields.io/badge/pytest-333333?style=flat&logo=pytest&logoColor=white)](https://pytest.org/)

### Energy Systems & Simulation
[![CityLearn](https://img.shields.io/badge/CityLearn-333333?style=flat)](https://www.citylearn.net/)
[![HELICS](https://img.shields.io/badge/HELICS-333333?style=flat)](https://helics.org/)

### IoT, GIS & Tools
[![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-333333?style=flat&logo=raspberrypi&logoColor=white)](https://www.raspberrypi.com/)
[![MQTT](https://img.shields.io/badge/MQTT-333333?style=flat&logo=mqtt&logoColor=white)](https://mqtt.org/)
[![QGIS](https://img.shields.io/badge/QGIS-333333?style=flat&logo=qgis&logoColor=white)](https://qgis.org/)
[![Git](https://img.shields.io/badge/Git-333333?style=flat&logo=git&logoColor=white)](https://git-scm.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-333333?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/)

---

## Featured Projects

### 🦿 [Robust RL for Sim-to-Sim Transfer in MuJoCo Hopper](https://github.com/Erfan-Afshinnia/robust-rl-hopper-domain-randomization)
Can a controller trained in one simulator still work when the physics change? Policies are trained on a source Hopper and tested, with no fine-tuning, on a target whose torso is 43% heavier.
- Ported a legacy `mujoco-py` / Gym environment to **Gymnasium** and official **MuJoCo** bindings, with 18 registered variants
- Wrote **REINFORCE** and **Actor-Critic** from scratch in **PyTorch**; used **SAC** and **PPO** (Stable-Baselines3) as baselines
- Ran 30 SAC training runs across 3 seeds and 3,000 evaluation episodes
- Torso-mass randomization raised mean target return from **830 → 1,271**; wide uniform randomization (±50%) beat the baseline on every seed
- 36 unit tests in CI, one command per study, fully reproducible

### ☀️ [Solar Power Prediction & ML Pipeline](https://github.com/Erfan-Afshinnia/solar-power-ml-pipeline)
End-to-end, production-style pipeline that predicts solar plant AC power from weather and time features.
- **XGBoost** model with shared feature engineering and a **Feast** feature store
- **KS-test drift detection** with drift-gated weekly retraining in **GitHub Actions**
- Champion/candidate promotion: a new model replaces the old one only if its MAE is lower
- Served with **FastAPI** (single and batch prediction) inside **Docker**, with a **Streamlit** monitoring dashboard and pytest tests

### 🌐 [IoT Earthquake Early Warning & Utilities Shut-Off](https://github.com/Erfan-Afshinnia/IoT-based-Earthquake-Early-Warning-and-Vital-Utilities-Shut-off-System) *(team project)*
Real-time platform that detects seismic activity and automatically shuts off gas, electricity and water.
- Accelerometer and velocity sensors streaming over **MQTT** to a **Raspberry Pi** controller
- REST data catalog, Telegram bot alerts and a live web dashboard

---

## Experience

### Reinforcement Learning Co-Simulation Intern — Energy Center Lab, Politecnico di Torino
**Nov 2025 – Apr 2026 · Turin, Italy**
- Built a stable, flexible framework that integrates reinforcement learning training and testing into energy co-simulation
- Used **HELICS** co-simulation for distributed energy systems

---

## Research

- 📄 **Survey of RL frameworks for energy systems** *(in preparation)* — systematic comparison of 33+ Gymnasium-based frameworks across buildings, power grids, EV/V2G and microgrids
- 🎓 **MSc thesis** *(in progress)* — domain randomization for heatwave-robust RL in district energy management

---

## Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-333333?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/erfan-afshinnia-2ab451218/)
[![GitHub](https://img.shields.io/badge/GitHub-333333?style=flat&logo=github&logoColor=white)](https://github.com/Erfan-Afshinnia)
