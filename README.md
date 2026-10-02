# 곽정우 (Jeongwoo Kwak)

AI engineer focused on image processing and computer vision. Also worked on clinical time series and LLM evaluation.

영상처리 중심의 AI 엔지니어입니다. 의료 영상(흉부 X선, 뇌 MRI)과 비전 모델을 주로 다뤘고, 임상 시계열과 LLM 평가
프로젝트도 했습니다. 성능 숫자를 믿어도 되는지 결과를 보기 전에 정한 기준으로 검증하고, 학습부터 ONNX, TensorRT
배포까지 직접 만듭니다.

## 주요 프로젝트

### 의료 AI 검증

- [Sepsis Early Warning](https://github.com/KJWoo99/sepsis-early-warning): MIMIC-IV ICU 시계열로 패혈증 조기예측.
  배양, 항생제 같은 처치 흔적 9개만으로 생리 지표 48개와 같은 성능이 나옴(AUPRC 0.0306 대 0.0308)을 사전등록 기준으로
  보임. LightGBM, GRU-D, Mamba 세 구조 모두 지름길 비율이 높음.
- [Clinical LLM Memorization Audit](https://github.com/KJWoo99/clinical-llm-memorization-audit): 공개 LLM 16개로
  퇴원요약에서 약물 목록 추출. 노트를 지우면 16개 중 11개가 F1 0.000 이 되어 외워서 답하지 않음을 확인했고,
  의료 특화 모델은 같은 계열 기반 모델보다 대체로 낫지 않음(사전등록 짝 2쌍 모두 기반 우세).
- [MIMIC Multimodal Readmission](https://github.com/KJWoo99/mimic-multimodal-readmission): 흉부 X선과 EHR 로 30일
  재입원 예측. 영상은 단독으로는 신호가 있지만 EHR 에 더해도 늘지 않음. 누수 컬럼이 AUROC 를 0.70 에서 0.83 으로
  부풀리는 것을 측정하고 뺌.
- [Hippocampal Volumetry](https://github.com/KJWoo99/hippocampal-volumetry): MONAI 3D 해마 분할과 부피 정량화.
  Dice 0.888, 부피 일치도 ICC 0.897 이지만 측정 오차(+/- 9.2%)가 연간 위축보다 커서 종단 추적에는 못 씀을 밝힘.
  TensorRT FP16 으로 PyTorch 대비 3.07배.

### 배포와 비전

- [Media Lens](https://github.com/KJWoo99/media-lens): CLIP, SigLIP2, DINOv2 기반 이미지 의미 검색과 중복 탐지.
  PyTorch, ONNX, TensorRT FP16 추론 경로, VRAM 기반 동적 배치와 OOM 복구.
- [Medical Image Classification](https://github.com/KJWoo99/Medical-Image-Classification): 폐암, 피부암, 위 용종,
  치아 질환 영상 분류.
- [YOLO Object Detection](https://github.com/KJWoo99/YOLO-Object-Detection): 안전모, 도로 균열, 차량 파손 검출과
  분할.
- [KJWADAS](https://github.com/KJWoo99/KJWADAS): 차선(UNet++)과 객체(YOLOv8) 검출 기반 실시간 ADAS.
- [AutoAware](https://github.com/KJWoo99/AutoAware): OpenCV 기반 운전자 졸음, 부주의 감지.

## 연구

- [AI in Healthcare: Concerns & Strategies](https://github.com/KJWoo99/Paper-AI-in-Healthcare-Concerns-Strategies):
  의료 분야 AI 적용의 우려와 전략 분석.

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
