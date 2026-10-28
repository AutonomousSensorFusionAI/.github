<p align="center">
  <img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/banner.svg" alt="Autonomous Sensor Fusion AI — 센서의 관측을 모아, 하나의 주행 인지로" width="100%">
</p>

<p align="center">
  <a href="https://github.com/AutonomousSensorFusionAI?tab=repositories"><img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/repositories-link.svg" alt="공개 저장소 보기" width="208" height="50"></a>
  <a href="#센서에서-통합-인지까지"><img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/architecture-link.svg" alt="구성 흐름 살펴보기" width="230" height="50"></a>
</p>

# Autonomous Sensor Fusion AI

**자율주행을 위한 센서융합·인지 소프트웨어**

Camera, LiDAR, Radar의 관측을 연결해 주변 객체를 인지하고 추적하는 소프트웨어를 개발합니다. 센서 데이터 전달과 시간 동기화, 객체 인지·융합, 모델 최적화와 차량 플랫폼 연계를 하나의 개발 흐름으로 다룹니다.

이 조직에서는 센서별 연동 코드와 인지·플랫폼 구성요소를 공개합니다. 설치 환경과 외부 SDK 요구사항은 각 저장소의 안내를 확인해 주세요.

Open-source building blocks for multi-sensor perception, inference deployment, and automotive software integration.

<img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/capabilities.svg" alt="센서 연결, 인지·융합, 실행 최적화, 차량 플랫폼 연계" width="100%">

## 센서에서 통합 인지까지

센서별 데이터를 연결하고, 객체 검출·추적·매칭을 거쳐 통합 인지 정보를 구성하는 흐름입니다. 모델 실행과 차량 런타임은 이 흐름을 뒷받침합니다.

<img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/architecture.svg" alt="Camera·LiDAR·Radar → 센서 데이터 연결과 시간 동기화 → 객체 검출 → 추적·매칭 → 센서 융합 → 통합 인지 정보. 모델 최적화·배포와 차량 플랫폼 연계가 실행을 지원합니다." width="100%">

## 개발·시험 장면

객체 검출, 다중 스트림 통신과 실차 탑재 환경을 함께 살펴봅니다.

<img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/development-scenes.png" alt="DDS 기반 객체 검출 실행 화면, 다중 센서 스트림 통신 시험, 센서 탑재 검증 차량" width="100%">

## 구성요소별 저장소

필요한 센서와 기능에서 시작하세요. 아래 역할은 현재 저장소의 README와 파일 구성을 기준으로 정리했습니다.

| 저장소 | 구분 | 역할 |
| --- | --- | --- |
| [Econ-camera](https://github.com/AutonomousSensorFusionAI/Econ-camera) | 센서 연결 | e-con 카메라 · DDS · 실행 관리 연계 |
| [Seyond_lidar](https://github.com/AutonomousSensorFusionAI/Seyond_lidar) | 센서 연결 | Seyond LiDAR · ROS 2/DDS 연동 |
| [Bosch-Radar](https://github.com/AutonomousSensorFusionAI/Bosch-Radar) | 센서 연결 | Radar CAN 데이터 수신·게시 |
| [perception-sw](https://github.com/AutonomousSensorFusionAI/perception-sw) | 인지 SW | 객체 인지 SW · YOLOv5 ROS 2 노드 |
| [sensor-data-publisher](https://github.com/AutonomousSensorFusionAI/sensor-data-publisher) | 데이터 전달 | Camera · GNSS · Radar 게시 코드 |
| [automotive-sw-platform](https://github.com/AutonomousSensorFusionAI/automotive-sw-platform) | 플랫폼 | AI · 미들웨어 · 예제 코드 |
| [AutomatedDrivingInterface](https://github.com/AutonomousSensorFusionAI/AutomatedDrivingInterface) | 인터페이스 | 자율주행 센서 인터페이스 설계·구현 |
| [adsp-adaptive-autosar](https://github.com/AutonomousSensorFusionAI/adsp-adaptive-autosar) | 통합 안내 | Adaptive AUTOSAR 통합 소개 |

## 개발 로드맵

클라우드·인프라 엣지 연계, 추론 워크플로우와 Adaptive AUTOSAR 통합, 차량 시나리오 검증으로 확장하고 있습니다. 아래 항목은 개발 방향이며, 제공되는 기능은 각 저장소와 릴리스 안내를 기준으로 합니다.

<img src="https://raw.githubusercontent.com/AutonomousSensorFusionAI/.github/main/profile/assets/roadmap.svg" alt="개발 로드맵: 클라우드·엣지 연계, 실행 환경 통합, 차량 적용·검증" width="100%">

## 시작하기

1. 사용할 센서 또는 기능에 맞는 저장소를 선택합니다.
2. 대상 하드웨어, 실행 환경, 외부 SDK·라이브러리 요구사항을 확인합니다.
3. 제공되는 예제와 실행 안내로 개별 구성요소를 확인한 뒤 연동 범위를 넓힙니다.

## 함께 개선하기

오류 제보와 기능 제안은 관련 저장소의 Issues를 이용해 주세요. 코드와 문서 개선은 Pull Request로 제안할 수 있습니다. 센서 종류, 사용 버전, 실행 환경과 재현 절차를 함께 남겨 주세요.

## 라이선스와 외부 구성요소

공개 코드의 이용 조건은 저장소별 LICENSE와 고지를 따릅니다. 일부 실행 경로에는 별도로 제공되는 SDK와 라이브러리가 필요하며, 모델·데이터·외부 구성요소에는 각각의 이용 조건이 적용됩니다.

<sub>본 프로젝트는 「자율주행을 위한 다중다종 센서 융합의 인공 신경망 구동 최적화 및 통합 인지 SW 기술 개발」 과제의 지원을 받아 개발되고 있습니다.</sub>
