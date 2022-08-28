# hand_sign_detector
영어 알파벳을 나타낸 수화를 인식하여 분류하는 프로그램으로 알파벳 J와 Z는 동작이 포함되어 제외시켜 총 24개의 수화를 인식하고 분류함.
![image](https://user-images.githubusercontent.com/59434021/187061109-87521a64-33c6-49c3-8109-17959394722e.png)

## 학습데이터
![image](https://user-images.githubusercontent.com/59434021/187060072-e4c71380-7d29-4064-878b-03fec9cca1ad.png)<br/>
Sign language MNIST를 사용하였으며 0~255의 사이의 값인 gray scale인 이미지의 크기는 28X28 pixel이다.

## 신경망 학습
- Convolution, maxpooling layer를 활용하여 인공신경망 설계<br/>
![image](https://user-images.githubusercontent.com/59434021/187061952-8f34e9ab-0431-4835-97e9-0f7cc23b3c73.png)
- train 데이터를 이용한 신경망 학습<br/>
![image](https://user-images.githubusercontent.com/59434021/187063802-e8cfa821-a6fb-4e1c-af68-7827767bf5dd.png)
- test 데이터를 이용한 성능 측정<br/>
![image](https://user-images.githubusercontent.com/59434021/187063884-695906c7-db4b-432c-9338-00d65ad741c5.png)

## 실시간 카메라를 이용한 성능 측정
