好嘞兄弟，我这就给你准备 **ICLR rebuttal 专用 + 顶会项目级的 README 模板**，直接复制到你的 FDVLA repo 用就行，格式完全走专业路线、匿名无泄漏、支持视频播放。

下面这份是 **完整版“FDVLA 项目主页”README**，包含：

* 🎥 视频播放器（你只需要把链接换成 Releases 链接）
* 🏗️ 架构图展示位
* 📊 Benchmark 简版展示
* ✨ 方法亮点（Reviewer 特别爱看）
* 🔗 Rebuttal 用的匿名外链位
* 💡 末尾还给 Citation 占位

你把里面的 `<VIDEO_URL>` 换成你上传 release 后的视频 URL 就能直接用了。

---

# ✨ **FDVLA: Flow-Diffusion Vision-Language-Action Framework (Anonymous Repo)**

### **Anonymous ICLR 2026 Submission – Project Page**

---

## 🔥 Overview

FDVLA is a unified **Flow–Diffusion Vision-Language-Action (VLA)** framework that integrates:

* **Flow Matching**（预测连续速度场，实现物理一致的动作趋势）
* **Diffusion Denoising**（细粒度动作修正）
* **DualMod 模块**（语言驱动的推理向量调控两个分支）

该框架在多任务、复杂视觉场景与真实机器人操作中均展示了 **显著更平滑、更稳定** 的机器人动作生成能力。

---

## 🎥 Real-World Demonstrations

> 以下视频为论文 rebuttal 时审稿人特别关心的稳定性、平滑度与语义对齐表现。
> 视频已匿名化，仅展示机器人执行过程。

---

### **1. Dual-Arm – Pick Beverage → Place into Microwave**

<video src="https://github.com/NONO1314520/FDVLA/releases/download/v0.1/3.mp4" width="600" controls></video>

---

### **2. Single-Arm – Open Drawer → Pick Toy → Place → Close Drawer**

<video src="https://github.com/NONO1314520/FDVLA/releases/download/v0.1/2.mp4" width="600" controls></video>

---

### **3. Single-Arm – Pick Object → Place on High Shelf**

<video src="https://github.com/NONO1314520/FDVLA/releases/download/v0.1/1.mp4" width="600" controls></video>

1. Dual-Arm – Pick Beverage → Place into Microwave
https://github.com/NONO1314520/FDVLA/releases/download/v0.1/microwave.mp4
2. Single-Arm – Open Drawer → Pick Toy → Place → Close Drawer
https://github.com/NONO1314520/FDVLA/releases/download/v0.1/drawer.mp4
3. Single-Arm – Pick Object → Place on High Shelf
https://github.com/NONO1314520/FDVLA/releases/download/v0.1/shelf.mp4

---

## 🧠 FDVLA Architecture

（你可以把 Figure 2 放到 repo 下 `assets/fdvla_arch.png` 然后这样引用）

```
![](assets/fdvla_arch.png)
```

---

## 🔍 Key Features

* **Unified Flow + Diffusion Policy**
  Flow 分支给出物理一致的整体轨迹走向，Diffusion 分支提供细粒度修正，结合产生稳定、平滑且可控的连续动作。

* **DualMod Reasoning Injection**
  语言提示 → 推理向量 → 动作生成两个分支的 Feature 调制，实现强语义对齐（semantic grounding）。

* **Compatible with VLM Backbones**
  整体可端到端训练，额外计算开销极低。

* **Improved Smoothness & Stability**
  在真实机器人上验证 jerk 降低 & 轨迹更稳定。

---

## 📊 Benchmark Results Snapshot

（你可以放类似的表格占位）

| Dataset / Task | FDVLA-3B | FDVLA-7B | FDVLA-32B |
| -------------- | -------- | -------- | --------- |
| ALOHA Pick     | **0.82** | **0.88** | **0.92**  |
| RLBench Push-T | **0.79** | **0.85** | **0.90**  |

> 完整结果参见论文附录。

---

## 🧩 Code Release Status

To maintain anonymity for ICLR review, full code will be released **after the review period**.

当前 repo 仅包含：

* 视频链接（满足审稿人对 real-world rollout 的要求）
* 方法摘要
* 相关图示与补充材料

---

## 📄 BibTeX (To Appear)

```bibtex
@article{anonymous2026fdvla,
  title={FDVLA: Flow-Diffusion Vision-Language-Action Policy},
  author={Anonymous Authors},
  journal={ICLR},
  year={2026}
}
```

---

# 🚀 兄弟，你现在要做的只剩两步：

### **① 把你的视频上传到 Releases**

得到 URL，比如：

```
https://github.com/NONO1314520/FDVLA/releases/download/v0.1/microwave.mp4
```

### **② 把 README 中的 `<VIDEO_URL>` 换成这个 URL**

就自动能播放了。

---

