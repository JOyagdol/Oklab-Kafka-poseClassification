# PoseClassification Kafka Consumer

🧘 Kafka 기반 자세 분류 시스템의 데이터 수신 및 처리 컴포넌트입니다.

## 📌 개요

이 Kafka Consumer는 영상 기반 자세 분류 모델로부터 전송되는 실시간 데이터를 수신하고, 이를 분석하여 특정 동작/자세를 분류하거나 경고 조건을 감지하는 역할을 합니다.

---

## 📦 주요 기능

- Kafka 토픽(`pose-classification-event`)
- JSON 기반 자세 분류 데이터 파싱
- 데이터 정합성 검증
- 위험 자세 탐지 및 알림 연계

---

## ⚙️ 시스템 구조

```
Pose Classification Producer (영상 AI)
        ↓
[Kafka Topic: pose-classification-event]
        ↓
PoseClassification Kafka Consumer
        ↓
[분석 및 저장 / 알림 연동]
```
