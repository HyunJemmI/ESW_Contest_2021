# HappyNewEar

2021 ESW(Embedded Software Contest) 자유공모 부분 출전
- 입선작

# 프로젝트 목표
시각 및 청각 장애인이 도로에서 위험 상황을 마주했을 때 대처할 수 있도록 돕는 디바이스 개발 

4-array mic와 ODAS 라이브러리를 사용하여 음원의 위치(방향, 거리)를 파악한다

* ODAS : https://github.com/introlab/odas

도로 상황에서 발생할 수 있는 타입의 소리만을 골라 유의미한 데이터셋을 생성
yamnet_Class_map_csv

출력 장치로 골전도 스피커와 라즈베라파이 모니터를 사용

input data가 사전에 설정한 8가지의 상황에 속하면 다음 2가지 방법으로 출력 

1. 모니터에 img를 사진과 함께 text를 출력해 위험 상황 알림
2. 골전도 스피커로 해당 상황에 대한 음성녹음 파일 재생

* Classification.py - 소리 분류를 위한 모듈
* HappyNewEar.sh - 프로그램의 실행 파일