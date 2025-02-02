# 3D Object Detection Project on LiDAR Dataset
## 프로젝트 환경
### 1. Dataset : KITTI dataset
### 2. Framework : OpenPCDet
### 3. Model : PointPillars

  
## 프레임워크 관련
### Forked OpenPCDet
### 1. setup.py로 환경 세팅
### 2. train, test, demo 활용
### 3. 상세 내용 : https://github.com/open-mmlab/OpenPCDet/blob/master/docs/GETTING_STARTED.md

  
## 모델 학습 관련
### Experiment/Model 참조
### 1. 80 Epoch 학습 내용 및 Tensorboard 저장
### 2. Demo는 OpenPCDet 제공 최고 성능 PointPillar 체크포인트 사용(7728)
![image](https://github.com/HY-AI2-Projects/PointPillars_2020045296_SeongjunBaek/assets/16371108/a9f19807-782f-4976-ba37-e99a624e7e42)
![스크린샷, 2023-12-19 19-19-45](https://github.com/HY-AI2-Projects/PointPillars_2020045296_SeongjunBaek/assets/16371108/c57e2316-18e8-4f0f-a9f5-b65dc480685a)


  
## 라이다 실증 관련
### Expoeriment/Demo 참조
### 1. Ouster 64ch LiDAR 사용
### 2. Data Convert : .pcap -> .pcd -> .bin (model demo 사용)
### 3. .pcap -> .pcd는 제조사 제공 레퍼런스(https://static.ouster.dev/sdk-docs)
### 4. .pcd -> .bin은 변환 코드 환경에 맞춰서 수정함(Python 3.7)
### ※ .bin 변환 중 PCD 절반이 사라지는 버그 발견, 수정 보류
### 5. 첨부된 파일은 촬영한 장면 중 모델이 가장 잘 인식한 것(인식 대상 : 시험자, 택시)
![KakaoTalk_20231219_235101751](https://github.com/HY-AI2-Projects/PointPillars_2020045296_SeongjunBaek/assets/16371108/a69e0580-49d1-4b0b-a770-fedb6337fcc2)


  
## 향후 계획
### 1. 다른 데이터셋 추가 활용 ex. Waymo
### 2. Bug Fix (Convert, LiDAR ch 관련)
### 3. 다른 모델 추가 활용 ex. 현재 SOTA모델 등
### 4. 미니 자동차에 LiDAR 설치 후 주행하며 테스트
![KakaoTalk_20231220_003706731](https://github.com/HY-AI2-Projects/PointPillars_2020045296_SeongjunBaek/assets/16371108/8b5d9de4-97f7-4abb-ba64-47766a19ca87)

