# Grand-Challenge AI4Life Calcium Imaging Denoising Challenge 2025

---
## 🔬 個人研究貢獻與技術實踐 (My Research & Technical Implementation)

> **註：** 本專案為團隊協作作品，我主要負責將去噪理論轉化為具體的模型邏輯與數據處理策略。以下為我參與的核心任務與達成成果：

### 1. 掩碼影像訓練策略 (Masked Image Training)
* **方法與應用**：推動「掩碼重建」策略的研究，並參與在數據管線中實作多樣化的遮蔽模式（如 Gaussian 與 Local Surrounding）。
* **達成成果**：透過建議 75%-90% 的掩碼比例與 Blind-spot 機制，協助模型從空間上下文學習影像結構，有效應對過擬合特定雜訊與恆等映射（Identity Mapping）的技術挑戰。

### 2. 神經微分方程 (nmODE) 架構對標
* **方法與應用**：將 nmODE 概念導入 U-Net 的 Bottleneck 層，並協助對標 RK4 (Runge-Kutta) 數值積分邏輯的實作。
* **達成成果**：將特徵演化模擬為連續物理過程，強化模型對於鈣成像中具時間連續性訊號的捕捉與還原能力。

### 3. 多維度統計評估體系 (stSNR Evaluation)
* **方法與應用**：運用統計背景定義 stSNR (Spatio-Temporal SNR) 指標，並協同開發評測腳本。
* **達成成果**：從空間結構穩定性與時間訊號完整性雙維度量化去噪品質，為團隊的模型迭代提供量化依據。

---

# Installation

## Install uv 

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
source $HOME/.local/bin/env
```

## Install dependencies

```bash
uv sync
```

## Download Dataset

```bash
uv run ./download_data.sh
```

# Usage

## Jupyter Notebook

Open `notebook.ipynb` to execute block by block. MUST check the parameters block to setup constant variables.

## Python

**Not ready**

```bash
uv run main.py
```
