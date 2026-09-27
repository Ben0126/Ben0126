# <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Waving%20Hand.png" alt="Waving Hand" width="35" height="35" /> 你好，我是葉舜斌 (Ben)

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
[![Phone](https://img.shields.io/badge/Phone-(+1)541--250--2269-green?style=flat-square&logo=whatsapp)](tel:+15412502269)

</div>

## 🌱 關於我

Oregon State University 電機與電腦工程（ECE）工程碩士（M.Eng.）學生，專注於機器人軟體：強化學習、控制與多無人機自主系統。在工研院（ITRI）開發無人機群避碰系統，從 Gazebo 模擬一路做到 10 架無人機實機飛行測試（PX4、ROS 2）。

- 🎓 **目前**：**Oregon State University** **電機與電腦工程** 工程碩士（M.Eng.，預計 2028 年 3 月畢業）
- 🎓 **國立臺東大學** **綠色與資訊科技學士學位學程** 學士（GPA：3.3/4.0）
- 💼 **工研院 資訊與通訊研究所（ICL）** 機器人軟體工程實習生（2026）
- 💼 **工研院 電子與光電系統研究所（EOSL）** 工程師實習生（2023–2024）
- 🔍 **正在尋找 2027 年暑期的 Robotics Software / Autonomy 實習機會**

## 📊 數據一覽

<div align="center">

| 🚁 **`50`** | ✈️ **`10`** | 🛡️ **`100%`** | 📚 **`4`** |
|:---:|:---:|:---:|:---:|
| 架無人機 SITL 群飛驗證 | 架無人機實機飛行測試 | 測試情境零碰撞 | 篇論文發表 |

</div>

## 🔬 經歷

### 🚁 工業技術研究院（ITRI）| 資訊與通訊研究所（ICL）
**機器人軟體工程實習生** _(2026 年 7 月 - 2026 年 8 月)_
- 負責集中式無人機群避碰系統的端到端開發（PX4、ROS 2），設計新的 APF（人工勢場）演算法，在避免碰撞的同時維持隊形
- 在 Gazebo PX4 SITL 中以最多 50 架無人機驗證，在設定的運作條件下，所有測試情境皆無碰撞
- 將系統從模擬推進到 10 架無人機的實機飛行測試

### 👨‍💻 工業技術研究院（ITRI）| 電子與光電系統研究所（EOSL）
**工程師實習生** _(2023 年 11 月 - 2024 年 8 月)_
- 整合並維護無 GPS 環境的四旋翼平台（飛控、機載電腦、深度相機），使用視覺慣性里程計（VIO）進行定點懸停
- 測試並除錯視覺跟隨（follow-me）功能，讓無人機自主追蹤操作者選定的目標；執行飛行測試並回報問題給感知團隊

### 🏫 國立臺東大學 | 智慧能源管理實驗室
**研究助理** _(2023 年 8 月 - 2024 年 2 月)_
- 指導 4 位實驗室新成員學習啟發式演算法（Metaheuristic Algorithms），提升其問題解決與實作能力
- 優化粒子群演算法（PSO）於 3D 路徑規劃的應用，運算效率提升 32%
- 執行實驗與數據分析，參與智慧能源管理相關學術論文

### 🏫 國立臺東大學 | 智慧綠能控制課程
**課程助教** _(2022 年 2 月 - 2022 年 6 月)_
- 帶領超過 34 位學生完成無人機控制專題，教授 MATLAB 程式設計與 Tello 無人機控制技術
- 介紹無人機原理與群飛概念，啟發學生的創新專題設計

### 🏫 國立臺東大學 | 智慧控制實驗室
**研究助理** _(2021 年 7 月 - 2021 年 12 月)_
- 研究 GA-PID、模糊控制與 PID 等無人機控制方法，並發表研討會論文〈Impact of control strategies on altitude control in indoor quadcopter〉
- 協助教授撰寫科技部研究計畫，主題為無人機控制與避障技術；同時指導實驗室成員無人機組裝、維護與技術應用

## 🔭 專案

### 🚁 Vision-DPPO
> 以 Diffusion Policy 實現端到端無人機控制

設計端到端的視覺運動控制框架，以 Diffusion Policy 取代串級 PID，透過 CNN 編碼器與 Conditional 1D U-Net，將原始 FPV 影像序列直接映射為 4 軸馬達推力。

- 🛠️ **技術**：Python、PyTorch、CNN、PPO
- 🗓️ **期間**：2026 年 2 月 - 2026 年 6 月
- ⚙️ **成果**：自建 6 自由度四旋翼模擬器（RK4 積分，200Hz）、基於狀態的 PPO 專家策略，以及 HDF5 合成資料收集流程

### 🏭 工廠 ERP 系統
> 製造業正式上線的 ERP

部署正式上線的 ERP，取代製造商原本的 MS Access 系統，整合成一條從報價到出貨的流程，供管理層與 4 個產線站點使用。

- 🛠️ **技術**：Django REST Framework、React、PostgreSQL
- 🚩 **狀態**：已上線
- 📋 [API 文件](https://github.com/Ben0126/factory-erp/tree/main/ERP)

### 🍽️ 食來運轉 FoodFate
> 餐廳推薦 App

開發餐廳推薦 App，提供個人化篩選、輪盤式隨機選擇，並整合 Google Maps。

- 🛠️ **技術**：Flutter、Python Flask、PostgreSQL、Google Maps API
- 📋 [專案說明](https://github.com/Ben0126/food_fate)

### 🌐 其他小專案

- ⌨️ **英文打字與聽力練習**
  > 提升英文打字速度與聽力理解的網頁應用。
  - 🔗 [前往 App](https://ben0126.github.io/english_typing_practice/)

- ☕ **Corvallis 咖啡廳與餐廳地圖**
  > Corvallis 地區咖啡廳與餐廳的互動式推薦地圖。
  - 🔗 [前往 App](https://ben0126.github.io/corvallis-coffee-map/)

- 💰 **記帳網站（App）**
  > 簡單實用的個人記帳應用。
  - 🔗 [前往 App](https://bookkeeping-app-three.vercel.app/)

## 💻 技術能力

### 程式語言與工具
<div>
  <img src="https://img.shields.io/badge/-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/-MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white" />
  <img src="https://img.shields.io/badge/-ROS%20/%20ROS%202-22314E?style=for-the-badge&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/-PX4-00A1DE?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-Gazebo%20SITL-F58113?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/-PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/-CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/-OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/-Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/-React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/-Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</div>

### 專業領域
- 🚁 **機器人** - ROS 2 / ROS、PX4、Gazebo SITL、視覺慣性里程計（VIO）、群體避碰（APF）、飛行測試
- 🤖 **AI / ML** - 強化學習（PPO、DDPG）、**Diffusion Policy**、PyTorch、CUDA、OpenCV、啟發式演算法（PSO、GA）
- 🔧 **軟體** - Python、C++、MATLAB、Git、Linux、Django、React、Flutter、PostgreSQL

## 📚 論文發表

### 期刊論文
- Liu, C.H., **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Shen, S.C., Ding, Z.A., Chu, L.M.* (2023). "Design of Reinforcement Learning Controller for Quadcopter in Flight Environment with Random Disturbance," *Green Science & Technology Journal (ISSN: 2223-6961)*, Vol. 13, No. 1, pp.45-54.

### 研討會論文
- Liu, C.H.*, **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Luo, G.Y., Shen, S.C., Ding, Z.A., Chu, L.M. (2023). "Performance Evaluation of Proximal Policy Optimization Algorithm in Controlling Quadcopters," *IEEE International Symposium on Computer, Consumer and Control (IEEE-IS3C)*, Taichung, Taiwan.

- Liu, C.H.*, **Yeh, S.P.**, Wang, Y.C., Lai, W.L., Luo, G.Y., Chu, L.M.* (2023). "Analysis of Various Control Strategies for Indoor Quadcopter Applications," *Conference of Research and Development in Technology Education (CRDTE)*, Kaohsiung, Taiwan.（口頭發表）

- Liu, C.H.*, Lai, W.L., Shen, S.C., **Yeh, S.P.**, Wu, P.C., Wang, Y.C., Luo, G.Y. (2022). "Impact of control strategies on altitude control in indoor quadcopter," *IET International Conference on Engineering Technologies and Applications (IET ICETA)*, Changhua, Taiwan.（海報發表）

## 🏆 獲獎與榮譽

- 🎓 **大專學生研究計畫** - 科技部（共同作者）
- 🥇 **SOS-IPO**（第一名）- 院級創新創業提案競賽
- 🥇 **創業實習成果展**（第一名）- 院級競賽

## 📊 開發者概覽

<div align="center">

  <a href="https://github.com/Ben0126">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=Ben0126&theme=tokyonight" alt="GitHub Streak" />
  </a>
</div>

<div align="center">

  <img src="https://skillicons.dev/icons?i=python,cpp,matlab,pytorch,ros,django,react,flutter,postgres,git,linux&perline=6" alt="Skills" />
</div>

<details>
  <summary>📈 GitHub 統計</summary>
  <div align="center">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Ben0126&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ben0126&layout=compact&langs_count=7&theme=tokyonight"/>
  </div>
</details>

## 🔗 聯絡方式

歡迎聯繫 2027 年暑期機器人軟體與自主系統相關的實習機會：

- 📧 Email：[spyeh26@gmail.com](mailto:spyeh26@gmail.com)
- 💼 LinkedIn：[linkedin.com/in/benyeh26](https://www.linkedin.com/in/benyeh26/)
- 📱 美國電話：[(+1)541-250-2269](tel:+15412502269)
- 🌐 個人網站：[https://my-web-gules.vercel.app/](https://my-web-gules.vercel.app/)

---

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Ben0126&color=blue&style=flat-square&label=Profile+Views" alt="Profile Views Counter" />
</div>
