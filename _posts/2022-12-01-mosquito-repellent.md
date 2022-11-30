---
title: mosquito repellent
author: Jeongeun Kim
date: 2022-12-1
categories: [Exhibition,2022년]
tags: [post,jeongeunkim]     # TAG names should always be lowercase, 띄어쓰기도 금지
---

------------------------------------------
# mosquito repellent

### 제작동기

 한여름의 적이라는 모기는 이제 더 이상 한여름에만 찾아오지 않습니다. 
 지구온난화로 인해 예전과 대비하여 봄과 가을은 더 짧아지고 따뜻해졌으며, 이로 인해 여름뿐만 아니라 
 봄과 가을에도 모기들의 공격은 계속되고 있습니다.
 그로 인해 사람들은 언제 어디서 찾아올지 모르는 모기들에게 많은 불쾌감을 받고 있습니다.  
 따라서 언제 찾아올지 모르는 모기들로 인한 피해를 직접 입고 나서야 모기향, 스프레이 등으로 모기를 대비할 것이 아니라,
 모기들이 좋아하는 환경일 때 스스로 모기들을 퇴치해 주는 기계가 있으면 어떨까 하는 생각을 하게 되었습니다.

---

### 작품소개

모기가 좋아하는 온도인 14°C~41°C 에서 자동으로 켜지는 모기 퇴치제 입니다. 모기가 이산화탄소를 마신 후에 특정 파장을 향해 날아간다는 실험 결과를 이용하여
모기를 유인하기 위해 파란색 LED를 연결하였습니다. 모기를 죽이는 방식은 전기 파리채와 동일합니다.
실용성을 위해 부가 기능으로 온도와 습도를 표시하는 기능도 추가하였습니다.
14°C~41°C 에서 전원이 켜지고 전원에는 전기 충격기, 초음파 센서, 파란색 LED가 연결되어 있습니다. 

---

### 작품구현 

1. DHT11 아두이노 온습도 센서를 이용하여 주변의 온도와 습도 측정값을 받습니다.
2. 센서로 얻은 온습도 측정값을 LCD에 표시합니다.
3. 모기가 좋아하는 온도 14°C~41°C, 습도 65%~75% 일 때는 모기가 좋아하는 파장인 365nm인 푸른빛을 RGB LED를 통해 방출하도록 합니다. 여기서 나오는 빛을 통해 모기들을 유인합니다.
4. HC-SR04 초음파 센서를 통해 모기 퇴치 기계 안의 움직임을 감지합니다.
5. 움직임이 감지된 경우 고전압 트랩을 작동시켜 모기를 퇴치합니다.

---

### 작품 동작 결과

<img src="/assets/img/post/mosquito repellent/LCD.PNG" width=90%>

Humidity: 39.00 %   Temperature: 24.00 *c 75.20 *F   Heat index: 23.47 *c 74.25 *Fdistance : 32.04 cm

---

### 결론 및 작품 후기

1. 사람들의 생활 방식이 도시화되며 겨울에도 따뜻한 온수 탱크와 같은 저수 시설과 지하주차장의 배수구 등을 통해 성충 상태로 겨울을 나는 모기들도 생겨나고 있습니다. 그러한 온도 설정값(14°C~41°C)을 벗어난 온도에서 발생한 모기는 잡기에 어려움이 있었습니다.
2. 모기의 움직임이 작아 초음파 센서로 감지 되지 않는 경우가 발생할 수 있어 아쉬움이 남습니다.
3. 이후 더 구체화된 조건에서 스프레이 분사형의 모기 퇴치기 등 더욱 발전된 모기 퇴치기 개발이 가능할 것으로 보입니다.
4. 하지만 아두이노의 여러 센서들과 엑츄에이터를 코딩을 통해 원하는 조건에서 사용하는 방법을 학습할 수 있었습니다.



---