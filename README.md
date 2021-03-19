# AIschoolforbeginner_2019
AI 스쿨 입문자 양성과정 2기, 2019.09~2019.11
- 최종 팀 프로젝트

## 딥러닝을 활용한 남녀 이미지 classification  
![남녀 얼굴 구분](https://user-images.githubusercontent.com/58945760/89788578-5bafaa00-db5a-11ea-9e05-5633040b78fa.jpg)
> 이미지 데이터를 INPUT 하였을 때 남자인지 여자인지 구분할 수 있는 모델을 구축, 정확도 향상에 주력 

### 01_데이터 수집
> 총 검증 데이터 70,000장을 수집하였다. 출처는 다음과 같다. 

![20191103_202029](https://user-images.githubusercontent.com/58945760/89788451-24d99400-db5a-11ea-8989-8f377702ffdb.png)
![20191103_202118](https://user-images.githubusercontent.com/58945760/89788622-6b2ef300-db5a-11ea-9de2-d01be0f14749.png)

### 02_데이터 전처리
> 데이터 전처리는 다음과 같은 과정으로 진행되었다.

1. 너무 어리거나(0~10대 초중반) 너무 나이가 많은(60대 이상) 이미지 제외 
2. 안경/선글라스/얼굴을 가리는 모자/페이스페인팅/마스크를 쓴 이미지 제외
3. 남/녀 data labeling 
4. labeling한 dataset을 확인하며 중성적/남녀 구분이 힘든 이미지를 제외

### 03_모델링 
> 자체적으로 층을 쌓아올린 CNN 모델을 사용하였다. 모델 구조는 아래와 같다.
![image](https://user-images.githubusercontent.com/58945760/111735390-49030d80-88bf-11eb-9221-cbc5e46b465b.png)


### 04_결과
> accuracy와 loss 변화 추이는 아래 그래프와 같다. 
<img width="898" alt="KakaoTalk_20191030_174256707" src="https://user-images.githubusercontent.com/58945760/89789617-ca413780-db5b-11ea-8990-64ce2faf502f.png">

