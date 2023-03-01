# ComputerVision_Seminar
_ _ _ 

2023년 DNA STUDY를 통해 이미지 돌고래, 상어, 고래 3가지 동물을 분류하는 프로젝트를 진행했습니다.



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
