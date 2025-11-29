# basic_study_for_MNIST
MNIST Image Classification using Multi-Layer Perceptron (MLP) with PyTorch
이 프로젝트는 PyTorch를 사용하여 가장 기본적인 벤치마크 데이터셋 중 하나인 MNIST 손글씨 이미지 분류를 수행하는 다층 퍼셉트론(MLP) 모델을 구현하고 학습시키는 예제입니다.

주요 특징 (Features)
PyTorch 기반: 널리 사용되는 딥러닝 프레임워크인 PyTorch를 사용하여 모델을 구축하고 학습시킵니다.다층 퍼셉트론(MLP): 784차원(28x28 픽셀)의 MNIST 이미지를 입력받아 10개의 클래스(0부터 9)로 분류하는 간단한 완전 연결 네트워크(Fully Connected Network)를 사용합니다.

성능 분석
: 학습 곡선(손실 및 정확도) 시각화를 통해 모델의 학습 과정을 모니터링하고, 최종적으로 테스트 데이터셋에 대한 정확도를 측정합니다.

모델 아키텍처 요약
: torchsummary 라이브러리를 사용하여 모델의 레이어 구성과 전체 파라미터 수를 확인할 수 있습니다.

모델 아키텍처 (Model Architecture)
구현된 MLP 클래스는 3개의 선형 레이어(Fully Connected Layer)와 ReLU 활성화 함수, 그리고 오버피팅을 방지하기 위한 Dropout을 포함합니다.

샘플 예측 분석 (Sample Prediction Analysis)학습 후 모델의 예측 결과를 시각적으로 분석한 이미지입니다. 
<img width="1061" height="685" alt="image" src="https://github.com/user-attachments/assets/36a68433-f4a2-4004-98f2-053c8e41deb1" />
모델 학습 전 모델이 판단한 숫자 정답
<img width="1134" height="716" alt="image" src="https://github.com/user-attachments/assets/0aac0467-4b93-4a6c-bf13-d79efcb0db17" />
모델 학습 후 모델이 판단한 숫자 정답

사용된 기술 스택 (Tech Stack)
Python 3.xPyTorch (for model, training)
Torchvision (for MNIST dataset)
NumPyMatplotlib (for visualization)

실행 방법 (How to Run) 
라이브러리 설치
:Bashpip install torch torchvision torchaudio numpy matplotlib torchsummary tqdm

노트북 실행
:MNIST_classification.ipynb 파일을 Jupyter Notebook 또는 Google Colab 환경에서 엽니다.모든 셀을 순서대로 실행하여 데이터 로드, 모델 정의, 학습 및 평가를 진행합니다.


