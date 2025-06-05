# Korean-Sign-Language-KSL-Detection-Modeling-ML-Tensorflow-
Improving Deep Learning-based Korean Sign Language Recognition Performance via Landmark Optimization <br/>
딥러닝 기반의 한국 수어 인식 모델을 개발한 졸업 프로젝트입니다. 부족한 수어 데이터셋을 직접 촬영 및 보강하여 학습 정확도를 높였으며, 수어의 연속성 및 시공간적 특징을 반영하여 모델 성능을 향상시켰습니다.

[프로젝트 영상](https://youtu.be/W0w3K3NxXkQ?si=CU8WiGKR3jW8qP1j)

<br/><br/>

**Learning Env: Jupyter Notebook**
## Package Version: <br/>
absl-py                       1.4.0 <br/>
h5py                          3.7.0 <br/>
imbalanced-learn              0.10.1 <br/>
matplotlib                    3.7.0 <br/>
matplotlib-inline             0.1.6 <br/>
mediapipe                     0.10.7 <br/>
numpy                         1.23.5 <br/>
numpydoc                      1.5.0 <br/>
opencv-python                 4.8.1.78 <br/>
openpyxl                      3.0.10 <br/>
tensorboard                   2.13.0 <br/>
tensorboard-data-server       0.7.0 <br/>
tensorflow                    2.13.0rc0 <br/>
tensorflow-estimator          2.13.0rc0 <br/>
tensorflow-macos              2.13.0rc0 <br/>
QtPy                          2.2.0 <br/>
scikit-image                  0.19.3 <br/>
scikit-learn                  1.2.1 <br/>


<br/><br/>

## 📌 프로젝트 개요

* **프로젝트명**: 한국 수어 인식 성능 향상 프로젝트
* **기간**: 2023.03 \~ 2023.12
* **목표**: 기존 수어 인식 모델의 성능 한계를 극복하고, 한국 수어에 특화된 모델 설계 및 학습

<br/><br/>

## 🧠 사용 기술

* **언어**: Python
* **프레임워크**: PyTorch
* **딥러닝 모델**: CNN + BiLSTM + Attention
* **영상 전처리**: OpenCV, MediaPipe
* **데이터 시각화**: Matplotlib, Seaborn

<br/><br/>

## 🗂 데이터 수집 및 전처리

* **기존 데이터셋**: AI-Hub 한국 수어 데이터셋 사용
* **보강 데이터**: 자체 촬영 (카메라 + 조명 장비 세팅)
* **라벨링 도구**: CVAT 활용
* **전처리 작업**:

  * 배경 제거 및 프레임 정규화
  * 관절 좌표 및 손/팔 keypoint 추출 (MediaPipe)
  * 제스처 구간 분할 및 정렬

<br/><br/>

## 🏗 모델 구조 및 학습

### ▶ 모델 구조

1. **CNN**: 프레임 단위의 특징 추출
2. **BiLSTM**: 시계열 수어의 순서 정보 학습
3. **Attention Layer**: 의미 있는 프레임에 가중치 집중

### ▶ 학습 세부사항

* Optimizer: Adam
* Loss Function: Categorical Cross Entropy
* Epochs: 50\~100
* Batch Size: 32
* Accuracy: Top-1 Accuracy 기준 약 93%

<br/><br/>

## 🔍 주요 성과 및 특징

* 📈 **수어 인식 정확도 향상**: 자체 촬영 데이터 추가 시 정확도 10% 이상 향상
* 🧩 **모델 경량화**: 모바일 및 임베디드 환경 적용 고려한 최적화 모델 설계
* 🗣 **연속 수어 인식 대응**: 단어 단위가 아닌 문장 단위 수어 인식 실험 진행
* 🏆 **졸업 우수 프로젝트 선정**


<br/><br/>

## 🔗 참고 자료

* AI-Hub 한국 수어 데이터셋: [https://www.aihub.or.kr/aidata/307](https://www.aihub.or.kr/aidata/307)
* MediaPipe: [https://google.github.io/mediapipe/](https://google.github.io/mediapipe/)
* PyTorch Docs: [https://pytorch.org/docs/](https://pytorch.org/docs/)

<br/><br/>

