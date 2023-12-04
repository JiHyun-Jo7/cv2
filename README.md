# 🎥 Open CV2 
---
### 🤖 개발 환경
- NVIDIA Jetson Nano Development Kit-B01
- Ubuntu 18.04.6 LTS
- python 3.6.9
---
### 01. Open Video
---
- Output mp4 file in samba folder
- samba 폴더에 있는 mp4 파일 출력
---
### 02. Nano Camera 📸
---
- Video Output using CSI, USB camera
- CSI, USB 카메라를 사용하여 영상 출력
---
### 03. RTSP (Real Time Streaming Protocol)
---
- video Output from RTSP 
- RTSP 영상 출력
---
### 04. Open Image 🖼️
---
- Position and resize the image to be output
- 이미지를 출력할 위치, 크기 조절
---
### 05. Gray Scale 🐼
---
- Convert Image to Gray
- 이미지를 흑백으로 변환
---
### 06. Get Info 📃
---
- Get Informations in Image
- 이미지의 정보 확인
---
### 07. Draw Polygon ✏️
---
- Draw line, polygons, circle, text
- Select location, Color, Tickness, Size
- 선, 다각형, 원, 텍스트를 입력
- 도형(텍스트)를 입력할 위치, 색상, 두께 선택
---
### 08. Canny 01
---
- Video Edge Detection using Canny
- Canny를 사용한 동영상의 edge 추출
---
### 09. Video Recoding 📹
---
- Recode the Video and Print
- 동영상 녹화 및 출력
---
### 10. Gaussian Blur
---
- Output Gaussian blur in 4 steps
- Display steps as text
- 가우시안 블러 4단계 출력, 단계를 텍스트로 표시
---
### 11. Color Palette 🎨
---
- Make color palette using trackbar
- 트랙 바를 사용한 컬러 팔레트
---
### 12. Threshold
---
- Use various thresholds
- 여러 종류의 threshold를 사용
```
cv2.threshold(img, threshold_value, value, flag)
```
||value<th_value|value>th_value|
|:---:|:---:|:---:|
|THRESH_BINARY|0|value|
|THRESH_BINARY_INV|value|0|
|THRESH_TRUNC|img|th_value|
|THRESH_TOZERO|0|img|
|THRESH_TOZERO_INV|img|0|
---

---
### 13. Threshold 02
---
- Use various adaptivethresholds
- 여러 종류의 adaptivethresholds를 사용
```
cv2.adaptiveThreshold(img, value, adaptiveMethod, thresholdType, blocksize, C)
```
- img: Grayscale image
- value: adaptiveMethod에 의해 계산된 문턱값과 thresholdType에 의해 픽셀에 적용될 최대값
- adaptiveMethod: 사용할 Adaptive Thresholding 알고리즘
- cv2.ADAPTIVE_THRESH_MEAN_C: 적용할 픽셀 (x,y)를 중심으로 하는 
- blocksize x blocksize 안에 있는 픽셀값의 평균에서 C를 뺀 값을 문턱값으로 함
- cv2.ADAPTIVE_THRESH_GAUSSIAN_C: 적용할 픽셀 (x,y)를 중심으로 하는 
- blocksize x blocksize안에 있는 Gaussian 윈도우 기반 가중치들의 합에서 C를 뺀 값을 문턱값으로 함
- blocksize: 픽셀에 적용할 문턱값을 계산하기 위한 블럭 크기. 적용될 픽셀이 블럭의 중심이 됨. 따라서 blocksize는 홀수여야 함
- C: 보정 상수로, 이 값이 양수이면 계산된 adaptive 문턱값에서 빼고, 음수면 더해줌. 0이면 그대로.
---
### 14. Blur 01
---

---
### 15. Blur 02
---

---
### 16. Keyboard ⌨️
---

---
### 17. Canny 02 
---
```
edge = cv2.Canny(img, minVal, maxVal)
```
- Image comparison according to minVal, maxVal difference
- minVal, maxVal 값에 따른 이미지 결과 비교
---
### 18. Color Mask
---

---




