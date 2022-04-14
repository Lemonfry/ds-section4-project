# ds-section4-project

딥러닝을 이용한 교통사고 이미지 분류

1. 데이터

  * Kaggle Accident detection from CCTV footage - training 및 validation
    
    (https://www.kaggle.com/ckay16/accident-detection-from-cctv-footage/code)
  
  * Uncertainty-based Traffic Accident Anticipation with Spatio-Temporal Relational Learning 논문 데이터 - training, validation 및 test
    
    (https://github.com/Cogito2012/CarCrashDataset)

  * 유투브의 교통사고 동영상 2개 - test
  
    * 유투브 (1) https://www.youtube.com/watch?v=0YiNGdodbX0
  
    * 유투브 (2) https://www.youtube.com/watch?v=bzBWISpd09Q


2. 모델
이미지 분석을 위해 CNN 모델을 사용하고자 하였고 직접 만든 CNN 및 2개의 기존에 있던 모델(Resnet50, MobilenetV2)을 비교

3. 결론
모델의 분류 정확도는 자작 모델 0.65, Resnet50 0.73, MoblienetV2 0.62로 나타났습니다.

*주의*

*처음 프로젝트는 section4 project_1 파일로 젠체 모델을 진행하다가 연결이 끊어져서 section4 project_2로 진행했습니다.
이후 모델을 조금 수정하여 코드를 실행한 최종 파일은 section4 project_3_resubmit 입니다.*

 4/14 변경점

Kaggle의 사고/비사고 이미지 분류는 한 영상에서 사고가 난 지점 이전을 비사고, 사고 이후부터 사고로 분류하고 있으며, 처음 진행한 코드는 기존엔 2번째 있는 Car Crash Dataset(CCD)의 영상에서 사고 영상은 모두 사고로, 비사고 영상은 모두 비사고로 분류했습니다.

이후 kaggle처럼 CCD 또한 사고 영상에서 사고 전 부분은 비사고, 사고 이후는 사고로 분류하도록 변경했습니다.

또한 직접 만든 CNN 모델의 parameter 조정으로 결과를 비교해 보고, 위의 기존 2개 모델에 InceptionV3를 추가해 비교하였습니다.

Input 이미지를 변경하고 난 후 정확도는 자작 모델이 0.52, Resnet50 0.56, MobilenetV2 0.46, InceptionV3 0.57 입니다.
