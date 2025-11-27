# AttentionBubble for Apple Watch

AttentionBubble is a fast, lightweight, and iOS-native app designed for beginner runners who want a simple way to track distance, calculate critical speed (CS), and estimate realistic half-marathon performance.
This open-source version focuses on clean design, fundamental running analytics, and a distraction-free interface — without any AI or reinforcement-learning logic from the private production app.

---
✨ Key Features:
1. Simple & Fast Running Tracking
Record your running workouts with a clean, minimal UI — no ads, no noise, no unnecessary features.
2. Designed for Beginner Runners
See your monthly distance and test runs in one place, helping you build consistent habits with a friendly, minimal interface.
3. Critical Speed (CS) Calculation
Input at least three runs (distance + time), and the app computes your Critical Speed, a proven indicator for endurance and pacing.
4. Half-Marathon Time Estimation
Using gender and estimated body-fat percentage, the app predicts your half-marathon finish time with simple evidence-based formulas — giving beginners a healthy, realistic goal.

---
## 🏗️ Tech Stack
- **SwiftUI**  
- **CloudKit**  
- **HealthKit**  
- **CoreMotion / CoreLocation**  
- **WatchConnectivity**  
- **MVVM Architecture**  
- **Xcode 16+ / iOS 17+ recommended**

---
🧠 什么是 Critical Speed（CS）？
Critical Speed（CS）= 你的可持续极限速度。
运动生理学研究表明，CS 是“有氧稳态下可以长期维持的最高速度”（Jones & Vanhatalo, 2017）。
换句话说：
低于 CS → 依赖有氧能量，可长时间持续（Burnley & Jones, 2018）
高于 CS → 依赖无氧能量，会迅速力竭（Poole et al., 2016）
相比“配速”或“心率区间”，CS 更稳定、波动更小，也更能预测跑步表现（Jones, 2019）。
AttentionBubble 的设计，就是把原本需要实验室才能测试的变量 ——
变成跑步新手也能轻松获得的训练工具。
🚀 AttentionBubble 的功能
1. 通过 ≥3 组测试跑，计算你的 CS
CS 理论指出：
速度（Speed）– 极限时间（Tlim）之间存在稳定的双曲线关系（Monod & Scherrer, 1965）。
在跑步训练中，只需三组不同距离 + 不同时间的测试跑，就能求出：
Critical Speed（CS）
D′（冲刺能量储备）（Moritani et al., 1981）
这是目前运动科学界最可靠的耐力预测方法之一（Burnley & Jones, 2018）。
2. 月度跑量追踪（Monthly Distance）
研究显示，持续且逐渐增加的月跑量与耐力表现提升呈显著正相关（Esteve-Lanao et al., 2007）。
AttentionBubble 提供极简月度界面，让你清楚知道本月训练负荷是否够稳定。
3. 智能体能预测（Smart Predictions）
你的：
性别
体脂率（Body Fat %）
会影响：
跑步经济性（Running Economy）
最大摄氧量（VO₂max）
长时间维持配速的能力
研究指出：
体脂率越高 → 跑步经济性越差，半马/全马表现越受影响（Barnes & Kilding, 2015）。
因此 AttentionBubble 用这些变量来调整预测结果，让预估时间既科学又真实。
5. 沉浸式 Onboarding，引导理解 CS 科学性
引导页将展示：
为什么 CS 比心率更稳定？（Poole et al., 2016）
为什么 D′ 像一个“冲刺油箱”？（Moritani et al., 1981）
为什么只需要 3 组跑就能测试？（Jones & Vanhatalo, 2017）
为什么 CS 是预测半马成績的黄金指标？（Galbraith et al., 2011）

---
🧬 CS 与 D′：科学跑步的双引擎
指标	意义	文献支持
C - 决定你能“持续多久”的关键速度	Jones & Vanhatalo (2017)
D′ - 决定你能“冲多快”的能量储备	Moritani et al. (1981)
两者结合，可以几乎完整描述跑者的耐力能力（Burnley & Jones, 2018）。
🏃‍♂️ 如何用 CS 训练？
在训练计划设计中，CS 是最常用的疲劳阈值之一（Poole et al., 2016）。
CS−（<100% CS） → 有氧区间，提升基础耐力
CS+（103–110% CS） → 高强度区间，提高速度耐受性
这种训练区间划分已在大量耐力研究中验证（Jones, 2019）。

---
个性化半马训练（未来功能）
研究证明，CS 可以可靠预测半程马拉松完赛时间（Galbraith et al., 2011）。
AttentionBubble 将逐步加入：
- 周训练建议
- CS 趋势图（代表 VO₂max 和耐力变化）
- 长时间耐力区间预测
- 科学配速建议
- 这些模型均基于运动生理学的经典理论（Poole et al., 2016）。
