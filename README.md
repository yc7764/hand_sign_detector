# hand_sign_detector
영어 알파벳을 나타낸 수화를 인식하여 분류하는 프로그램이다. A~Z까지의 알파벳을 나타내는 수화 중에서 알파벳 J와 Z는 동작이 포함되어 제외시켜 총 24개의 수화를 인식하고 분류한다. 각 알파벳을 나타내는 수화 동작은 아래의 그림과 같다.
![image](https://user-images.githubusercontent.com/59434021/187061109-87521a64-33c6-49c3-8109-17959394722e.png)

## 학습데이터
학습데이터로는 Sign language MNIST를 사용하였으며 CSV 파일 형태의 데이터를 읽어와 사용한다. 각 학습데이터는 label과 784개의 pixel 값으로 이루어져 있으며 한 개의 image size는 28X28 pixel이고 0~255의 사이의 값을 가지는 gray scale로 표현되어 있다. 총 데이터의 개수는 34,629개이며 train data는 27,456개이고, test data는 7,173개 이다.
- CSV 파일에서 읽어온 학습 데이터 출력<br/>
![image](https://user-images.githubusercontent.com/59434021/187090371-ef8484b6-2d40-4ae7-b4d7-3221c94c063d.png)<br/>
- pixel 값을 읽어와 28X28의 크기로 resize하여 출력한 이미지<br/>
![image](https://user-images.githubusercontent.com/59434021/187060072-e4c71380-7d29-4064-878b-03fec9cca1ad.png)
## 신경망 학습
- Convolution, maxpooling layer를 활용하여 인공신경망 설계<br/>
![image](https://user-images.githubusercontent.com/59434021/187061952-8f34e9ab-0431-4835-97e9-0f7cc23b3c73.png)
- train 데이터를 이용한 신경망 학습<br/>
![image](https://user-images.githubusercontent.com/59434021/187063802-e8cfa821-a6fb-4e1c-af68-7827767bf5dd.png)
- test 데이터를 이용한 성능 측정<br/>
![image](https://user-images.githubusercontent.com/59434021/187063884-695906c7-db4b-432c-9338-00d65ad741c5.png)
