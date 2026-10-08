# study

딥러닝 공부 기록입니다. 이론은 「모두를 위한 딥러닝」 시즌1, 실습은 시즌2 PyTorch를 따라갑니다. 최종 목표는 ResNet-18을 직접 구현해 Stanford 40 Actions 분류에서 정확도 70% 이상을 내는 것입니다.

## 3주 계획 (하루 4~5시간)

시즌1은 이론(lec) 영상만 봅니다. lab 영상은 옛 TensorFlow라 건너뜁니다. 각 주의 7일차는 밀린 것을 따라잡거나 복습하는 날입니다.

### 1주: 기초 다지기 → 머신러닝 기초

| 일차 | 할 일 | 상태 |
|---|---|---|
| 1 | 클래스 노트북 A·B (점프 투 파이썬 05-1 먼저 읽기) | |
| 2 | 클래스 노트북 C, NumPy 노트북 A·B | |
| 3 | NumPy 노트북 C·D, PyTorch 튜토리얼 "텐서" | |
| 4 | Lec 00~03, Lab 01-1·01-2·02·03 | |
| 5 | Lec 04~05, Lab 04-1·04-2·05, wandb 가입 후 Lab 05 기록해 보기 | |
| 6 | Lec 06~07, Lab 06·07-1·07-2 (MNIST를 wandb로 기록) | |
| 7 | 여유 / 복습 | |

### 2주: 신경망 → CNN → ResNet-18 구현

| 일차 | 할 일 | 상태 |
|---|---|---|
| 8 | Lec 08~09 (lec9-x 미분 영상을 lec9-2보다 먼저), Lab 08-1·08-2 | |
| 9 | Lec 10, Lab 09-1~09-4 | |
| 10 | Lec 11, Lab 10-1·10-2 (MNIST CNN) | |
| 11 | Lab 10-4 (ImageFolder), Lab 10-6 (ResNet), ResNet 논문 읽기 | |
| 12 | ResNet-18 직접 구현 (층 이름을 torchvision과 같게) | |
| 13 | 구현 검증: 파라미터 수 비교, ImageNet pretrained 가중치 로드, CIFAR10으로 짧게 학습 | |
| 14 | 여유 / 복습 | |

### 3주: Stanford40 분류 → 분석 → 정리

| 일차 | 할 일 | 상태 |
|---|---|---|
| 15 | Stanford40 내려받아 구글 드라이브에 저장, 공식 split으로 `Dataset` 만들기 | |
| 16 | pretrained ResNet-18 학습 (fc만 40으로 교체), wandb 기록, **70% 달성** | |
| 17 | 처음부터(scratch) 학습해 비교, 70% 미달이면 lr·augmentation 조정 | |
| 18 | wandb confusion matrix, 클래스별 정확도 | |
| 19 | Grad-CAM으로 맞힌 사진과 틀린 사진 분석 | |
| 20 | 결과 정리 (교수님 보고용) | |
| 21 | 여유 | |

### 주의할 점
- 시즌2 코드는 PyTorch 1.0 기준이라 최신 버전에서 에러가 납니다. MNIST의 `test_data`·`test_labels`는 `.data`·`.targets`로, CIFAR10의 `train_data`는 `.data`로 바꿉니다.
- Lab 09-4는 `Sequential`에 linear1~3만 넣어서 출력이 512가 되는 버그가 있습니다. 직접 칠 때 고칩니다.
- GPU는 10일차부터 필요합니다. Colab에서 **런타임 → 런타임 유형 변경 → T4 GPU**로 켭니다.

## 폴더

| 주차 | 내용 | 폴더 |
|---|---|---|
| 0 | 파이썬 클래스 + NumPy (1~3일차) | [`week0/`](week0/) |

## 자료
- 이론: 모두를 위한 딥러닝 시즌1 https://www.youtube.com/playlist?list=PLlMkM4tgfjnLSOjrEJN31gZATbcj_MpUm
- 실습: 모두를 위한 딥러닝 시즌2 PyTorch https://deeplearningzerotoall.github.io/season2/lec_pytorch.html
- 실습 코드: https://github.com/deeplearningzerotoall/PyTorch
- ResNet 논문: https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf
- Stanford 40 Actions: http://vision.stanford.edu/Datasets/40actions.html
- 학습 로그: https://wandb.ai/site/
- 시각화: https://github.com/jacobgil/pytorch-grad-cam
