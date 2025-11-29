# 🖊️ Basic Study for MNIST
> **MNIST Image Classification using Multi-Layer Perceptron (MLP) with PyTorch**

이 프로젝트는 **PyTorch**를 사용하여 딥러닝의 가장 기본적인 벤치마크 데이터셋 중 하나인 **MNIST 손글씨 이미지**를 분류하는 **다층 퍼셉트론(MLP)** 모델을 구현하고 학습시키는 예제입니다.

## 🛠️ Tech Stack

| Category | Technology |
| :--- | :--- |
| **Language** | Python 3.x |
| **Framework** | PyTorch (Model, Training) |
| **Dataset** | Torchvision (MNIST) |
| **Libraries** | NumPy, Matplotlib (Visualization), torchsummary, tqdm |

## ✨ Key Features

* **🔥 PyTorch 기반 구현**: 널리 사용되는 딥러닝 프레임워크인 PyTorch를 사용하여 모델 구축부터 학습까지의 전체 파이프라인을 실습합니다.
* **🧠 다층 퍼셉트론 (MLP)**: 784차원(28x28 픽셀)의 이미지를 입력받아 0부터 9까지 10개의 클래스로 분류하는 완전 연결 네트워크(Fully Connected Network)를 구현합니다.
* **📊 성능 분석 및 시각화**: 학습 곡선(Loss & Accuracy)을 시각화하여 학습 과정을 모니터링하고, 최종 테스트 데이터셋에 대한 정확도를 측정합니다.
* **📝 모델 요약**: `torchsummary` 라이브러리를 활용하여 모델의 레이어 구성과 전체 파라미터 수를 직관적으로 확인합니다.

## 🏗️ Model Architecture

구현된 MLP 모델은 **3개의 선형 레이어(Linear Layers)**와 **ReLU 활성화 함수**, 그리고 오버피팅 방지를 위한 **Dropout**으로 구성되어 있습니다.

| Layer Type | Configuration |
| :--- | :--- |
| **Input Layer** | Flatten (28x28 → 784) |
| **Hidden Layer 1** | Linear + ReLU + Dropout |
| **Hidden Layer 2** | Linear + ReLU + Dropout |
| **Output Layer** | Linear (10 Classes) |

## Sample Prediction Analysis

모델의 학습 전과 후, 예측 성능의 변화를 시각적으로 비교 분석합니다.

### 1. Before Training (학습 전)
모델이 학습되지 않은 상태에서는 무작위로 숫자를 판단하거나 낮은 신뢰도를 보입니다.
<img width="80%" alt="Before Training" src="https://github.com/user-attachments/assets/36a68433-f4a2-4004-98f2-053c8e41deb1" />

### 2. After Training (학습 후)
학습이 완료된 후, 모델은 손글씨 숫자를 높은 정확도로 판별합니다.
<img width="80%" alt="After Training" src="https://github.com/user-attachments/assets/0aac0467-4b93-4a6c-bf13-d79efcb0db17" />

## How to Run

### 1. 라이브러리 설치
필요한 Python 패키지들을 설치합니다.

```bash
pip install torch torchvision torchaudio numpy matplotlib torchsummary tqdm
