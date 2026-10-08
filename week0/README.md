# 0주차: 파이썬 클래스 + NumPy

시즌2 PyTorch 실습을 시작하기 전에, 모델(`nn.Module`)과 데이터셋(`Dataset`)을 만드는 데 필요한 **클래스**와, 텐서를 다루는 데 필요한 **NumPy**를 연습합니다.

## 파일

| 파일 | 내용 | 일정 |
|---|---|---|
| `week0_1_class.ipynb` | 클래스 기초 → 상속과 `super()` → `nn.Module`, ResNet 잔차 블록, `Dataset` 미리보기 | 1~3일차 |
| `week0_2_numpy.ipynb` | 배열과 shape → 슬라이싱 → 연산·axis·브로드캐스팅 → PyTorch 텐서와 자동 미분 맛보기 | 4~6일차 |
| `solutions/` | 위 두 노트북의 정답 | 막혔을 때만 |

## 푸는 방법

1. Google Colab(https://colab.research.google.com)을 열고 **파일 → 노트북 업로드**로 노트북을 올립니다. GitHub 탭에서 이 저장소를 열어도 됩니다.
2. 맨 위 준비 셀을 실행합니다.
3. `# TODO` 부분을 채우고 실행한 뒤, 바로 아래 채점 셀을 실행합니다. ✅가 나오면 통과입니다.
4. 정답 노트북을 봤다면, **닫고 안 보고 다시 써보기**까지 해야 합니다.

## 같이 볼 자료

### 클래스 (1~3일차)
- 점프 투 파이썬 (무료, 한국어): https://wikidocs.net/book/1
  - **05-1 클래스**: https://wikidocs.net/28 (상속, 메서드 오버라이딩까지)
- 파이썬 공식 튜토리얼 9장 클래스 (한국어): https://docs.python.org/ko/3/tutorial/classes.html
- PyTorch 한국어 튜토리얼 "신경망 모델 구성하기": https://tutorials.pytorch.kr/beginner/basics/buildmodel_tutorial.html

### NumPy (4~6일차)
- NumPy 공식 "완전 초보자를 위한 NumPy": https://numpy.org/doc/stable/user/absolute_beginners.html
- NumPy 공식 Quickstart: https://numpy.org/doc/stable/user/quickstart.html

### PyTorch로 넘어가기 (6일차 또는 1주차 시작 전)
- PyTorch 한국어 튜토리얼 "텐서(Tensor)": https://tutorials.pytorch.kr/beginner/basics/tensorqs_tutorial.html
- "Dataset과 DataLoader": https://tutorials.pytorch.kr/beginner/basics/data_tutorial.html
- "60분 만에 끝장내기": https://tutorials.pytorch.kr/beginner/deep_learning_60min_blitz.html

## 다 끝나면

1주차로 넘어갑니다: 시즌1 Lec 1~2 영상과 시즌2 Lab 01~02 노트북 (https://github.com/deeplearningzerotoall/PyTorch)
