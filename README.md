# ImageRestoration_DeformableGAN [2022.09 ~ 2023.01]

## 졸업논문
### * **전체 요약**
![image](https://github.com/jihyeheo/ImageRestoration_DeformableGAN/assets/64202709/46aeaa70-4de0-4c2d-8d36-3bdfa39b0f42)


### * **잡음 종류**<br>
가우시안 잡음, 포아송 잡음, 스펙클 잡음

### * **비교 모형**<br>
1) 고전적인 잡음제거 기술<br>
   mean 필터, median 필터, BM3D 필터<br>
3) 기존의 딥러닝<br>
   CNN, DCGAN, DnCNN, RED-CNN<br>
 
### * **제안 모형**<br>
*RED-DGAN(residual encoder decoder - deformable generative adersarial network) 모형*
* 특징
1) deformable 연산이 가능한 convolutional layer 이용
2) generator 모형은 선행 논문 RED-CNN 모형의 encoder와 유사
    * input: 잡음이 추가된 영상
    * output : 원본과 유사한 복원 영상
4) discrimator 모형은 분류 성능이 뛰어난 resnet18 모형
     * input : generator의 output
     * output : real? or fake?
### * 데이터<br>
웃는 얼굴 데이터 이용
### * 결과

       
   
