# 곽정우 (Jeongwoo Kwak)

AI engineer, mostly image processing and computer vision.

영상처리 위주로 AI 모델을 만들고 있습니다. 최근에는 공개 의료 데이터(MIMIC-IV, MIMIC-CXR, MSD)로 프로젝트를 하면서
모델 점수가 실제로 어디서 나오는지 확인하는 작업을 많이 했습니다.

## 프로젝트

### 의료 데이터

- [Hippocampal Volumetry](https://github.com/KJWoo99/hippocampal-volumetry): 뇌 MRI 해마 분할과 부피 측정.
  MONAI로 학습하고 ONNX, TensorRT FP16까지 배포했습니다. 부피 일치도(ICC)는 0.897이 나왔지만 측정 오차가
  1년 동안 줄어드는 부피보다 커서, 한 사람을 추적하는 용도로는 부족했습니다.
- [MIMIC Multimodal Readmission](https://github.com/KJWoo99/mimic-multimodal-readmission): 흉부 X선과 EHR로
  30일 재입원 예측. X선만으로도 약하게는 예측이 되지만 EHR에 붙이면 성능이 오르지 않았습니다. 누수 컬럼을 넣으면
  AUROC가 0.70에서 0.83까지 올라가는 것도 확인했습니다.
- [Sepsis Early Warning](https://github.com/KJWoo99/sepsis-early-warning): ICU 시계열로 패혈증 조기 예측.
  배양, 항생제 기록 같은 처치 흔적만으로도 생리 지표와 비슷한 성능이 나와서, 성능의 상당 부분이 처치 흔적에서
  온다는 것을 확인했습니다.
- [Clinical LLM Memorization Audit](https://github.com/KJWoo99/clinical-llm-memorization-audit): 공개 LLM 16개로
  퇴원 요약에서 약 목록을 뽑는 평가. 노트를 비우면 16개 중 11개가 0점이라 외워서 답하지는 않았고, 의료 특화
  모델이 기반 모델보다 낫다고 보기는 어려웠습니다.

### 비전, 배포

- [Media Lens](https://github.com/KJWoo99/media-lens): CLIP, SigLIP2, DINOv2로 사진 검색과 중복 사진 찾기.
  TensorRT FP16으로 추론하고 VRAM에 맞춰 배치 크기를 조절합니다.
- [Medical Image Classification](https://github.com/KJWoo99/Medical-Image-Classification): 폐암, 피부암, 위 용종,
  치아 질환 영상 분류
- [YOLO Object Detection](https://github.com/KJWoo99/YOLO-Object-Detection): 안전모, 도로 균열, 차량 파손 검출
- [KJWADAS](https://github.com/KJWoo99/KJWADAS): 차선 검출(UNet++)과 객체 검출(YOLOv8)로 만든 ADAS
- [AutoAware](https://github.com/KJWoo99/AutoAware): OpenCV로 운전자 졸음, 부주의 감지

## 연구

- [AI in Healthcare: Concerns & Strategies](https://github.com/KJWoo99/Paper-AI-in-Healthcare-Concerns-Strategies)

## 기술 스택

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=Python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=PyTorch&logoColor=white)
![MONAI](https://img.shields.io/badge/-MONAI-00A3E0?style=flat-square)
![Hugging Face](https://img.shields.io/badge/-Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LightGBM](https://img.shields.io/badge/-LightGBM-02569B?style=flat-square)
![Polars](https://img.shields.io/badge/-Polars-CD792C?style=flat-square&logo=polars&logoColor=white)
![OpenCV](https://img.shields.io/badge/-OpenCV-5C3EE8?style=flat-square&logo=OpenCV&logoColor=white)
![YOLO](https://img.shields.io/badge/-YOLO-00FFFF?style=flat-square&logo=YOLO&logoColor=black)
![ONNX](https://img.shields.io/badge/-ONNX-005CED?style=flat-square&logo=ONNX&logoColor=white)
![TensorRT](https://img.shields.io/badge/-TensorRT-76B900?style=flat-square&logo=NVIDIA&logoColor=white)

## 연락처

- Email: woo010487@gmail.com
- LinkedIn: [LinkedIn](https://www.linkedin.com/in/jeongwoo-kwak-7414a9290/)
- Portfolio (KOR): [Notion](https://kjwoo.notion.site/4f8f5d55abb2473db637b5de4dd758f6?pvs=74)
- Portfolio (ENG): [Notion](https://kjwoo.notion.site/Hi-I-m-Jungwoo-Kwak-8e58fc8f82d9437e884dc161bf823423?pvs=74)
