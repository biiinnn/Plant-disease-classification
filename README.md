# Project-Plant-disease-classification
2020 Spring - Project in Deep Learning Class - SeoulTech, Department of Industrial Information System Engineering

## 잎 사진을 통한 작물 질병 분류 (Plant Disease Classification)

### dataset 설명
33개의 class로 구분된 약 40000장의 이미지
![dataset](https://user-images.githubusercontent.com/46666833/163783617-4ec771a6-b699-4e85-a820-2b798e7010b4.PNG)  
9개의 작물과 24개의 질병으로 구성되어 있음 -> multi-class classification 

### 분석 과정
1. 데이터 전처리
- 전체 데이터를 6:2:2의 비율로 train, validation, test 나눔
- augmentation을 통해 클래스 별 분균형 해소
2. 모델 구축
- Baseline model: pre-trained 모델을 사용하지 않고 CNN 모델 구축
- Pretrained model: pre-trained 모델 사용 (ResNet50, DenseNet121)
3. 학습 진행 방향
- Baseline 모델 비교: split된 원본 데이터 사용, augmentation된 데이터 사용
- Pre-trained 모델 비교: augmentation 된 데이터 사용 (Baseline,DenseNet121,ResNet50 성능 비교)

### 결과
![result](https://user-images.githubusercontent.com/46666833/163784360-4ccbdebe-d457-497e-8ba0-43265f8aef14.png)
