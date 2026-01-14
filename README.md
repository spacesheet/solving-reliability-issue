# solving-reliability-issue

- 내부 대용량 트래픽 키워드 서버에서 데이터 실시간 스트리밍 처리 및 배치 보정

데이터 정합성 & 복구 책임 분리 모델
| 요소           |  담당 실패 유형        |
| ------------- | ------------------ |
| event_id      | 중복(At-least-once) |
| version / seq | 누락 / 순서          |
| event log     | 비가역 장애           |
| state DB      | 성능 병목            |
