# Codenter_Car_Damage
딥러닝 모델을 통한 Car damaged detection project

- Damage가 labeling 된 image data가 부족하여 via tool을 통해 직접 dataset을 추가로 만듬
- 데이터 추가 및 noise data로 overfit을 방지하기 위해 albumentaion 라이브러리를 통한 data augmentation 진행
- json 파일에 저장된 label 정보를 모델에 적용시키기 위해 이미지로 변환하는 작업 진행
- 파손 여부 및 위치만 판단하는 binary classification와 어떤 파손인지도 판별하는 multi classification 두 방면으로 진행
- 파손 위치와 영역을 정확하게 판단할 수 있도록 Semantic Segmentation 모델을 사용함
  - Deeplab v3
  - Unet
