# [프로젝트] 챗봇 MeU

- 팀원: 강규현, 김광현, 김희준, 정찬오, 조민재 

<br>

## 1. 소개

![](https://user-images.githubusercontent.com/58925328/88359326-39253f00-cdad-11ea-8526-271914452f18.PNG)

- 사용기술: 자연어처리(딥러닝), Python, Django, jQuery
- 서비스: 일상대화 챗봇, 감정일기, 60가지 질문카드
- URL: 준비중..
- 설명: 딥러닝기반 자연어처리 모델을 이용하여 챗봇을 구현하였습니 다. 본 챗봇은 심리적으로 불안한 사람들을 위로해주기 위한 목적으로 1인가구와 독거노인을 대상으로 하고 있습니다. 챗봇과 대화하며 감 정일기를 작성할 수있고, 60가지 질문카드를 진행하면서 자신에 대 해 돌아볼 수 있게 해줍니다.

<br>

(1) 생성 챗봇

![](https://user-images.githubusercontent.com/58925328/88359358-50642c80-cdad-11ea-89e8-9c7cf4452682.PNG)

(2) 감정일기 & 60가지 카드 서비스

![](https://user-images.githubusercontent.com/58925328/88359360-522df000-cdad-11ea-9787-27845d57116e.PNG)

<br>

<br>

## 2. 코드설명

>자연어처리 모델로 SEQ2SEQ와 Attention 기법, Transformer를 이용하였고, 데이터 정제, 단어 임베딩, 형태소 분석기를 바꿔가며 13개의 모델을 학습하고 평가하였다.



- `attention_training.ipynb`: SEQ2SEQ에 Attention기법을 적용한 한글 생성 챗봇 모델로, keras를 통해 모델 학습
- `transformer_training.ipynb`: transformer 모델을 적용한 한글 생성 챗봇 모델로, keras를 통해 모델 학습
- `attention_load.ipynb`:  attention 모델을 로드하고, 아래와 같은 코드를 포함함.
  - MAPE를 이용한 모델 평가
  - attention 가중치 시각화
  - Encoder 모델의 context 벡터 시각화



