# D-Bugging

<h1>1. 개발 목적</h1>
1-1) 단백질 섭취 목적 식용 및 애완동물 사료 목적 등의 확장되는 곤충의 활용성<br>
1-2) 원만한 곤충 사육 환경 구성에 대한 불편함 해결<br>
<br>
<h1>2. 하드웨어 구성</h1>
① ESP32 Wi-Fi Cam Module<br>
② 가스 센서, 온습도 센서, 초음파 가습기, LED 조명<br>
③ 파워 서플라이, 배터리<br>
<br>
<h1>3. 시스템 구성</h1>
<h2>모듈 제어 구성</h2>
① ESP32 Wi-Fi Cam Arduino 프로그래밍<br>
② C# Winform GUI 및 각 센서 통신용 Node MCU 구성<br>
③ 안드로이드 GUI 및 각 센서 통신용 Node MCU 구성<br>
④ C# 으로 구성된 프로그램을 통한 통신 MySQL DB 데이터 축적<br>
⑤ DB 데이터 통신을 통한 모듈 제어<br>
⑥ 웹페이지로 구성된 딥러닝 모델 적용 이미지 C# GUI 및 안드로이드 GUI 내 확인<br>
<br>
<h2>웹 페이지 구성</h2>
① MacOS Node.js 웹소켓 서버 구성<br>
② ESP32 웹 서버 구성<br>
③ ESP32 프레임 별 이진데이터 웹소켓 서버로 전송<br>
④ Node.js 서버 내 딥러닝 학습 모델 적용(yolov8 → roboflow3.0)<br>
⑤ 이진데이터 상태로 인식된 객체 박스 표현 좌표 생성<br>
⑥ Html 및 Javascript 를 통해 웹캠 이미지 및 인식 객체 박스 표현<br>
⑦ 프레임 별 인식 객체 좌표 중앙값에 점 찍어 활동 경로 표현<br>
<br>
<h2>이미지 전처리</h2>
① yolov8 → roboflow3.0 모델 변경<br>
② grayscale 적용 : 처리 연산량 감소 목적<br>
③ Augmentation - Mosaic 적용 : Small Object 성능 향상 기대 목적<br>
<br>
<h1>4. 결론</h1>
- ESP32 Cam을 통한 실시간 모니터링 기능 구현<br>
- 영상데이터에 딥러닝 모델 적용<br>
- C#, 안드로이드를 통한 실시간 모듈 제어

