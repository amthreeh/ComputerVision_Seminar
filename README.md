# ComputerVision_Seminar
_ _ _ 

2023년 DNA STUDY를 통해 이미지 돌고래, 상어, 고래 3가지 동물을 분류하는 프로젝트를 진행했습니다.

## week1


## week2 


## 데이터 파일 생성하기

+ original 폴더 안에 있는 dolphin, shark, whale의 하위 폴더에서 train, valid, test 폴더를 만든 후 각 클래스 별 폴더를 생성합니다.
+ 3가지 동물 폴더에 각각 7:2:1로 train, valid, test로 image 재배치

![image](https://user-images.githubusercontent.com/103898937/222076254-4e94ac1d-aa6b-4541-8022-ffb20e9f605d.png)


3 * 3형태로 dolphin, shark, whale을 3개씩 프린트하기 
![image](https://user-images.githubusercontent.com/103898937/222054173-ee309e3f-634e-4082-9e24-4a559d228da9.png)


## pytorch 데이터셋 클래스 실습
### 진행과정
1. pytorch 데이터셋 클래스 직접 만들기
  init, getitem, len 특수 메소드 필요
  root_path, mode(train/validation/test), transform(전처리&Augmentation)
2. 이미지 전처리하기
  2-1. resize, tensor화 
3. albumentation을 사용하여 Image Augmentation하기

![image](https://user-images.githubusercontent.com/103898937/222055876-d2c7227e-d2d1-4c13-b076-758c41a375ec.png)

# resnet50 모델 학습
## 진행 과정

1. dataset 클래스를 py파일로 변환
2. 바꾼 py파일을 모듈로 불러옴
3. 데이터 불러오기, albumentation에 필요한 과정 가져오기
4. resnet50을 사용

#week5

##GoogLeNet
- 1*1 filter
- Global average pooling
##ResNet


##week7
# Semantic Segmentation
Segmentation의 목적은 원본 이미지의 각 픽셀에 대해 클래스를 구분하고 인스턴스 및 배경을 분할하는 것입니다.
##FCN(Fully Convolution Network)
이미지 분류에서 우수한 성능을 보인 cnn 기반 모델을 semantic segmentation task를 수행할 수 있도록 변형시킨 모델
![image](https://user-images.githubusercontent.com/103898937/224943385-380e8f25-3b90-4b14-bded-eb6f28e2ee81.png)

Key point

- convolutionalization
- Deconvolution( upsampling)
- Skip architecture


##U-Net : Convolutional Networks for Biomedical Image Segmentation
- 이미지 분할을 목적으로 제안된 End to End 방식의 Fully Convolutional Network 기반 모델
- 저차원 뿐만 아니라 고차원 정보도 이용하여 이미지의 특징을 추출함과 동시에 정확한 위치 파악도 가능하게 하고자 했습니다.

![image](https://user-images.githubusercontent.com/103898937/224943982-4c90f4cb-9971-4ac1-8763-3ac39df68262.png)
