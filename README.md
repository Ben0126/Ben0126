# <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Waving%20Hand.png" alt="Waving Hand" width="35" height="35" /> Hello, I'm Shun-Pin (Ben) Yeh

<div align="center">
  <a href="README.md">🇺🇸 English</a> |
  <a href="README_zh.md">🇹🇼 中文</a>
</div>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=22&pause=1000&color=0C8AF7&center=true&vCenter=true&width=460&lines=Robotics+Software+Engineer;Multi-Drone+Autonomy+(PX4%2C+ROS+2);Reinforcement+Learning+%26+Control" alt="Typing SVG" />
</div>

<div align="center">

[![Email](https://img.shields.io/badge/Email-spyeh26%40gmail.com-blue?style=flat-square&logo=gmail)](mailto:spyeh26@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-benyeh26-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/benyeh26/)
[![Personal Website](https://img.shields.io/badge/Website-Portfolio-9cf?style=flat-square&logo=vercel)](https://my-web-gules.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-Ben0126-black?style=flat-square&logo=github)](https://github.com/Ben0126)

</div>

## 🌱 About Me

M.Eng. ECE student at Oregon State University focused on robotics software: reinforcement learning, control, and multi-drone autonomy. Built a drone-swarm collision-avoidance system at ITRI (C++, ROS 2, PX4), from Gazebo simulation to a 10-drone flight test. Seeking a Summer 2027 internship in Robotics Software or Autonomy.

- 🎓 **Now**: Master of Engineering in Electrical and Computer Engineering, **Oregon State University** (Expected Mar 2028)
- 🎓 Bachelor of Science in Green Energy and Information Technology, **National Taitung University** (Sep 2020 - Jun 2024) · GPA: 3.3/4.0 | Graduated with College Student Research Scholarship
- 💼 Robotics Software Engineering Intern, **Industrial Technology Research Institute (ITRI)** – Information and Communications Research Laboratories (2026)
- 💼 Engineer Intern, **Industrial Technology Research Institute (ITRI)** – Electronic and Optoelectronic System Research Lab. (2023–2024)

## 📊 By the Numbers

<div align="center">

| ✈️ **`10`** | 🚁 **`10`** | 💻 **`50`** | 📚 **`4`** |
|:---:|:---:|:---:|:---:|
| Drones in Physical Flight Test | Drones in Gazebo PX4 SITL | Drones in Offline Scaling Harness | Publications |

</div>

## 🔬 Experience

### 🚁 Industrial Technology Research Institute (ITRI) | Information and Communications Research Laboratories
**Robotics Software Engineering Intern** _(Jul 2026 - Aug 2026)_
- Owned the collision-avoidance system for a centralized drone swarm in C++ with ROS 2 and PX4, designing a new APF-based algorithm that avoids collisions without breaking formation.
- Validated with red/green A/B tests in Gazebo PX4 SITL with up to 10 drones: head-on and crossing drones kept ≥5.4 m apart vs. as close as 0.04 m with avoidance off. In a 50-drone offline closed-loop harness, the planner used <1% of the 20 ms control budget. At that scale, communication was the bottleneck, not compute.
- In a 10-drone physical flight test, the other drones steered around two that dropped into failsafe hover on sensor faults.

### 🏫 Republic of China (Taiwan) Army | 
**Mandatory Military Service** _(Jan 2025 - Apr 2025)_

### 👨‍💻 Industrial Technology Research Institute (ITRI) | Electronic and Optoelectronic System Research Lab.
**Engineer Intern** _(Nov 2023 - Aug 2024)_
- Integrated and maintained a GPS-denied quadcopter's flight controller, onboard computer and depth camera in C/C++ and ROS, using visual-inertial odometry (VIO) for position hold.
- Debugged a vision-based follow-me feature from the tracking model through ROS to the flight controller. In flight tests, isolated failure cases where the model's output was correct but the drone did not move or moved the wrong amount, then tuned the response.

### 🏫 National Taitung University | Intelligent Energy Management Lab
**Research Assistant** _(Aug 2023 - Feb 2024)_
- Mentored 4 new lab members on metaheuristic algorithms.
- Optimized a Particle Swarm Optimization (PSO) algorithm for 3D path planning, improving computational efficiency by 32%.
- Ran experiments and data analysis contributing to publications in intelligent energy management.

### 🏫 National Taitung University | Intelligent Green Technology Control Course
**Teaching Assistant** _(Feb 2022 - Jun 2022)_
- Guided 34+ students through drone control projects, teaching MATLAB and Tello drone control.
- Introduced drone principles and swarm flight concepts to inspire student project designs.

### 🏫 National Taitung University | Intelligent Control Lab
**Research Assistant** _(Jul 2021 - Dec 2021)_
- Investigated GA-PID, fuzzy logic, and PID control for drone controllers, leading to a conference paper on indoor quadcopter altitude control.
- Assisted with MOST research proposals on drone control and obstacle avoidance; mentored lab members in drone assembly and maintenance.

## 🔭 Projects

### 🚁 Vision-DPPO
> Visuomotor Quadrotor Hover via Flow Matching (Sim)

Built a 6-DOF quadrotor simulator (quaternion attitude, RK4 at 200 Hz, first-order motor lag) and a synthetic, domain-randomized 64×64 FPV renderer, then recorded HDF5 demonstrations from a state-based PPO expert and a PID teacher. Trained a 13.5M-parameter flow-matching policy by imitation. It maps 2 FPV frames, IMU and a mode flag to 50 Hz thrust/body-rate commands for a 200 Hz INDI inner loop (CNN encoder, IMU-to-vision cross-attention, 1D U-Net). Found my old RMSE metric rewarded early crashes by averaging only over steps flown. Built a frozen eval harness (paired starts, survival-conditioned error, bootstrap CIs, measured oracle) that exposed my prior best gains as artifacts. Ran 3-seed ablations with it: a Dispersive Loss rebuilt from its authors' code gave no pass-rate gain (−2.2 pp, pooled seed std 6.3 pp). Better sensing, far-range demos and 3.3× capacity each left hover error ~2.4–3.0 m vs a 0.07 m oracle.

- 🛠️ **Tech Stack**: PyTorch, PPO
- 🗓️ **Timeline**: Feb 2026 - Jun 2026
- 🚩 **Status**: Completed · Paper Draft

### 🏭 Factory ERP System

Built and deployed a full-stack ERP on Docker to replace a manufacturer's MS Access system only the owner could operate, so new staff can run daily operations, with 5 shop-floor display stations. Rebuilt the order-to-shipment workflow around orders after the product-first data model clashed with how the factory runs: approving an order now creates the work order and purchase drafts for missing materials when stock is short. Wrote 14 idempotent import commands, each with a dry-run mode, to migrate 31 legacy databases (~690K source rows). Implemented a pricing engine that combines product specs with material cost multipliers using margin-preserving formulas, exposed through DRF endpoints.

- 🛠️ **Tech Stack**: Django REST Framework, React, JavaScript, PostgreSQL
- 🚩 **Status**: Deployed (Rolling Out)

### 🔧 NoteHub
> Self-Hosted Markdown Notes App

Built a 6-tool MCP server so Claude Desktop can search and read notes via the app's HTTP API. Its only two write tools are additive (append to inbox, create a flashcard note), so the agent can never rewrite or delete notes. Fixed a race that returned HTTP 500 on folder imports when the file watcher and importer indexed the same note at once. Added an asyncio lock to serialize indexing, a SQLite upsert, and concurrency regression tests.

- 🛠️ **Tech Stack**: FastAPI, React, SQLite FTS5
- 🚩 **Status**: Personal Project

### 🌐 Other Small Projects

- 🍽️ **FoodFate**
  > Built a restaurant recommendation app with personalized filtering, a roulette-style random picker, and Google Maps integration.

- ⌨️ **English Typing & Listening Practice**
  > A web app for improving English typing speed and listening comprehension.
  - 🔗 [Go to App](https://ben0126.github.io/english_typing_practice/)

- ☕ **Corvallis Coffee Map**
  > An interactive recommendation map of coffee shops and restaurants in Corvallis, OR.
  - 🔗 [Go to App](https://ben0126.github.io/corvallis-coffee-map/)

- 💰 **Bookkeeping App**
  > A simple personal expense and budget tracker.
  - 🔗 [Go to App](https://bookkeeping-app-three.vercel.app/)

## 💻 Technical Skills

### Programming & Tools
<div>
  <img src="https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/-MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white" />
  <img src="https://img.shields.io/badge/-ROS%20%2F%20ROS%202-22314E?style=for-the-badge&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/-PX4-00A1DE?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-Gazebo%20SITL-F58113?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/-Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/-React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/-Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</div>

### Domains of Expertise
- 🚁 **Robotics** - ROS 2 / ROS, PX4, Gazebo SITL, Visual-Inertial Odometry (VIO), Swarm Collision Avoidance (APF), Flight Testing
- 🤖 **AI / ML** - Reinforcement Learning (PPO), Imitation Learning (Diffusion / Flow Matching), PyTorch, Actor-Critic, PSO / GA (metaheuristics)
- 🔧 **Software** - C++, C, Python, JavaScript, MATLAB, SQL (PostgreSQL), Git, Linux, Docker, Django, React, Flutter

## 📚 Publications

### Journal Papers
- Liu, C.H., **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Shen, S.C., Ding, Z.A., Chu, L.M.\* (2023). "Design of Reinforcement Learning Controller for Quadcopter in Flight Environment with Random Disturbance," *Green Science & Technology Journal (ISSN: 2223-6961), Vol. 13, No. 1, pp. 45-54*.

### Conference Papers
- Liu, C.H.\*, **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Luo, G.Y., Shen, S.C., Ding, Z.A., Chu, L.M. (2023). "Performance Evaluation of Proximal Policy Optimization Algorithm in Controlling Quadcopters," *IEEE International Symposium on Computer, Consumer and Control (IEEE-IS3C), Taichung, Taiwan*.

- Liu, C.H.\*, **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Luo, G.Y., Chu, L.M.\* (2023). "Analysis of Various Control Strategies for Indoor Quadcopter Applications," *Conference of Research and Development in Technology Education (CRDTE), Kaohsiung, Taiwan*. (Oral presentation)

- Liu, C.H.\*, Lai, W.L., Shen, S.C., **Yeh, S.P.**, Wu, P.C., Wang, Y.C., Luo, G.Y. (2022). "Impact of control strategies on altitude control in indoor quadcopter," *IET International Conference on Engineering Technologies and Applications (IET ICETA), Changhua, Taiwan*. (Poster presentation)

## 🏆 Awards & Honors

- 🎓 **College Student Research Scholarship** - Ministry of Science and Technology, Taiwan (co-author)
- 🥇 **SOS-IPO (1st Place)** - College Competition for Innovative Startup Pitch
- 🥇 **Startup Internship Learning Showcase (1st Place)** - College Competition

## 📊 Developer Profile

<div align="center">

  <a href="https://github.com/Ben0126">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=Ben0126&theme=tokyonight" alt="GitHub Streak" />
  </a>
</div>

<div align="center">

  <img src="https://skillicons.dev/icons?i=python,cpp,matlab,pytorch,ros,django,react,flutter,postgres,git,linux&perline=6" alt="Skills" />
</div>

<details>
  <summary>📈 GitHub Statistics</summary>
  <div align="center">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Ben0126&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ben0126&layout=compact&langs_count=7&theme=tokyonight"/>
  </div>
</details>

## 🔗 Contact Me

Seeking a Summer 2027 internship in Robotics Software or Autonomy. Feel free to reach out:

- 📧 Email: [spyeh26@gmail.com](mailto:spyeh26@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/benyeh26](https://www.linkedin.com/in/benyeh26/)
- 🌐 Personal Website: [https://my-web-gules.vercel.app/](https://my-web-gules.vercel.app/)

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Ben0126&color=blue&style=flat-square&label=Profile+Views" alt="Profile Views Counter" />
</div>
