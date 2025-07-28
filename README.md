# 자율주행 시스템에 사용되는 PyTorch와 TenSort

자율주행 시스템은 고도의 인공지능(AI) 및 딥러닝 기술을 기반으로 하여 차량이 스스로 환경을 인식하고 주행하는 기술입니다. 이를 위해 다양한 라이브러리와 프레임워크가 사용됩니다. 특히, **PyTorch**와 **TenSort**는 자율주행의 핵심 기술들에 많이 사용됩니다. 본 문서에서는 PyTorch와 TenSort의 특징과 자율주행 시스템에서의 역할을 정리합니다.

## 1. PyTorch

### 개요
**PyTorch**는 Facebook AI Research(FAIR)에서 개발한 오픈 소스 딥러닝 프레임워크로, 주로 연구와 프로토타입 개발에 사용됩니다. 이 프레임워크는 동적 그래프 계산 방식을 채택하고 있어, 모델의 구조와 데이터 흐름을 직관적으로 설정하고 디버깅할 수 있다는 장점이 있습니다.

### 자율주행에서의 활용
자율주행 차량의 인공지능 모델에서는 다양한 딥러닝 알고리즘을 사용하여 차량의 환경을 인식하고 주행 계획을 세웁니다. PyTorch는 다음과 같은 자율주행 기술에서 활용됩니다:

- **객체 인식(Object Detection):** 자동차는 도로, 보행자, 신호등, 차선 등을 인식해야 합니다. PyTorch를 이용한 CNN(Convolutional Neural Networks) 모델은 이러한 객체 인식 작업을 수행하는 데 매우 유용합니다.
  
- **차선 인식(Lane Detection):** 차량이 도로에서 차선을 인식하고 주행하는 데 중요한 역할을 합니다. PyTorch의 딥러닝 모델은 영상 데이터에서 차선을 감지하고 차선을 추적하는 데 사용됩니다.

- **경로 계획(Path Planning):** PyTorch는 자율주행 차량의 경로를 계산하고 최적화하는 데 사용될 수 있습니다. 강화 학습(Deep Reinforcement Learning)을 이용한 자율주행 차량의 행동 계획에 적용될 수 있습니다.

🔍 TensorRT의 역할
<br>❌ TensorRT가 하지 않는 것
<br>🚫 딥러닝 훈련 (Training)
<br>🚫 가중치 학습
<br>🚫 역전파 (Backpropagation)
<br>🚫 모델 개발
<br>✅ TensorRT가 하는 것
<br>⚡ 추론만 (Inference Only)
<br>🔧 모델 최적화
<br>📦 엔진 변환
🚀 실행 가속
