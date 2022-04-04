# ds-section4-project

딥러닝을 이용한 교통사고 이미지 분류

1. 데이터

1) Kaggle Accident detection from CCTV footage - training 및 validation
(https://www.kaggle.com/ckay16/accident-detection-from-cctv-footage/code)

2) Uncertainty-based Traffic Accident Anticipation with Spatio-Temporal Relational Learning 논문 데이터 - training, validation 및 test
(https://github.com/Cogito2012/CarCrashDataset)

3) 유투브의 교통사고 동영상 2개 - test
유투브 1) https://www.youtube.com/watch?v=0YiNGdodbX0
유투브 2) https://www.youtube.com/watch?v=bzBWISpd09Q

2. 모델
이미지 분석을 위해 CNN 모델을 사용하고자 하였고 직접 만든 CNN 및 2개의 기존에 있던 모델(Resnet50, MobilenetV2)을 비교

3. 결론
모델의 분류 정확도는 자작 모델 0.65, Resnet50 0.73, MoblienetV2 0.62로 나타났습니다.

*주의
section4 project_1 파일로 젠체 모델을 진행하다가 연결이 끊어져서 section4 project_2로 진행했습니다.
최종 파일은 section4 project_2 입니다.
