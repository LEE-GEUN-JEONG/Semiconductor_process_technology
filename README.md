# 대학원강의 / 반도체공정기술 / 2020년도 / 1학기 / 박홍식
## 실제 HW 구현은 공정을 통해서 이루어진다. 본 강의를 통해 실제적으로 어떻게 Chip이 생산되는지 공부하였다.
### 본 과제의 프로젝트로 본인이 회사의 포토공정 엔지니어라고 가정하고, 최신 DUV, EUV 장비에 대한 성능 보고서를 의뢰받았다고 가정한다. 
### 본 과제를 하단에 첨부하였고, 첨부 파일은 수업에 대한 과제를 정리한 것이다.

### PROJECT 
반도체공정기술 중간고사 대체 과제
2017117986 이근정
[1] ASML사와 Nikon사의 최신 DUV photolithography 장비들의 성능을 비교하고, 어느 장비를 10대
구매해서 기존 장비를 교체하는 것이 좋은지에 대해 보고서를 작성하시오.
1) ASML TWINSCAN NXT:2000i
• 2018년에 ASML사에서 출시됨.
• Projection Printing 방식의 일종으로 Step-and-Scaner system을 사용하는 Scanner임.
• Single-pass와 Multi-pass 두 가지 방식 모두 가능함.
• dual-stage Immersion Photo lithography 장비로 5nm, 7nm의 Technical node에 사용됨.
• ASML의 “Twinscan NXE:3400B EUV”와 Overlay 성능이 일치하여 mix-and-match 방식으로 호환이
가능함.
• in-line catadioptric lens design을 통해 업계 최고의 Numerical Aperture 값을 가짐. 
• 하루에 4,600장 이상의 Wafer를 처리할 수 있음. (높은 생산성)
• 이전 장비가 150시간의 Reliability를 달성하는데 6개월이 걸린 반면, 현재 장비는 단 2개월만 소요됨.
(향상된 maturity)
2) Nikon NSR-S635E
• 2018년에 Nikon사에서 출시됨.
• ASML사와 마찬가지로 Scanner 형태의 장비임.
• Immersion and Double Patterning lithography 장비로 최소 5nm의 Technical node patterning에
사용할 수 있음.
• Multiple patterning을 위해 향상된 Overlay 성능을 가짐.
• 시간당 175개의 wafer를 처리할 수 있는 높은 생산성을 가짐. (scan speed of 900 mm/sec and a
120 watt laser.)
• S635E autofocus (AF) system으로 uniformity를 향상시켜 처리된 wafer가 낮은 defect를 가짐.
• nozzle의 발전으로 Immersion시 낮은 defect를 가짐.
(참고)
Step-and-Scanner stepper : 일반적인 Conventional Stepper와 달리 reticle과 wafer가 optical
column에 의해 동시에 scanning 된다. 렌즈의 중앙부를 주로 이용하여 light exposure 되므로 더 정확
한 Patterning이 가능하며 Stepper 대비 향상된 를 얻을 수 있다. 게다가 Scanning 방식으로 인해
더 큰 field size를 처리하므로 throughput이 향상된다.


![image](https://user-images.githubusercontent.com/58419421/99421326-9c7d4300-2941-11eb-8d99-12a2a7884b08.png)

![image](https://user-images.githubusercontent.com/58419421/99421352-a1da8d80-2941-11eb-861f-f388d2e03d96.png)
![image](https://user-images.githubusercontent.com/58419421/99421366-a69f4180-2941-11eb-872c-aad805ce6e56.png)
![image](https://user-images.githubusercontent.com/58419421/99421381-aacb5f00-2941-11eb-90e0-2becf53130f7.png)
![image](https://user-images.githubusercontent.com/58419421/99421409-b028a980-2941-11eb-9eb6-45ca961e7bdd.png)
![image](https://user-images.githubusercontent.com/58419421/99421425-b454c700-2941-11eb-981f-497bf89de6e6.png)
![image](https://user-images.githubusercontent.com/58419421/99421435-b880e480-2941-11eb-9ab1-80282cb1f222.png)
![image](https://user-images.githubusercontent.com/58419421/99421455-bd459880-2941-11eb-978b-45929d528272.png)
![image](https://user-images.githubusercontent.com/58419421/99421479-c3d41000-2941-11eb-8039-f80baf20270c.png)


 
![image](https://user-images.githubusercontent.com/58419421/99421609-ea924680-2941-11eb-84d5-efa4ba9acb1e.png)


-
- Reduction Ratio : 본 EUV 장비는 DUV 장비와 마찬가지로 Projection printing의 일종인 Step-and-Scanning
Company ASML
Model name
TWINSCAN NXE:3400C
Wafer size 300mm
Resolution ≤13nm
NA 0.33
Light source EUV (13.5nm) by LPP
Reduction ratio 4X
Maximum exposure field 26mm×33mm
Overlay SMO≤1.4nm, MMO≤1.5nm
Throughput ≥170 wafers/hour (96shots)(Dose:20mJ/cm2)
- 7 -
방식의 Scanner이다. 일반적으로 사용되는 4X의 Mask pattern size : wafer pattern size의 비를 가진다.
- Maximum exposure field : Scanner 이므로 DUV 장비와 마찬가지로 큰 값의 field size를 가진다.
26mm*33mm
- Overlay : 종전의 DUV 장비보다 개선된 Overlay 성능을 가진다. 이는 수율 향상에 직접적인 이점을
가져온다.
- Throughput : DUV 장비가 시간당 275개의 wafer를 처리할 수 있었던 반면 EUV를 이용한
lithography 장비는 시간당 170개의 wafer를 처리할 수 있다. 이는 기존의 장비가 24시간 내내 가동할
수 있었던 반면 현재 EUV 장비의 가동률은 75% 밖에 되지 않기 때문이다. EUV 장비가 적극적으로 상용
화 되기 위해서는 Throughput 문제를 꼭 해결해야 한다.
3) Conclusion
더 작은 선폭의 반도체 공정을 위해 EUV 공정은 향후 반도체 산업에 필수 불가결한 기술이다. 하지만
그럼에도 불구하고 아직 EUV 공정에는 여러 한계들이 존재하며 이는 꼭 풀어야할 숙제이다. EUV 공정을
향후 차세대 반도체 공정에 적용하기 위해선 다음과 같은 문제점들이 해결 되어야 할 것이다.
1) Throughput
종전의 장비와 달리 EUV lithography 장비의 가동률은 75% 밖에 되지 않는다. 이는 throughput에 치
명적인 결과를 가져오고, 곧 제품 cost의 상승으로 이어진다. 따라서 현재는 EUV 공정이 DUV 공정과 함
께 같이 쓰이고 있다. EUV가 Photo 공정의 주류가 되려면 곡 장비의 가동시간 문제를 해결해야 할 것이
다.
2) Light Source Brightness
매우 짧은 파장의 light source를 사용하므로 light source의 enegy는 매우 높을 것이다. 이러한 강한
에너지의 light source를 만들어 내는 것은 쉬운 일이 아니다. 실제 양산에 투입하려면 light source의
power는 250W 수준은 되어야 한다. (125wafers/hour throughput 기준)
3) Mirror / Mask structure
EUV 공정은 많은 Reflective한 Mirror를 이용하여 light를 굴절시키고, Mask는 수십 층의 multi-layer
로 제작된다. 따라서 각 Mirror와 layer에서의 defect는 반드시 작아야할 것이다. 그렇지 않다면 defect
로 인해 올바른 pattern이 wafer에 전사되지 않을 것이다.
4) EUV용 Inspection tool
회로 pattern이 점점 미세해짐에 따라 defect를 찾기가 더욱더 힘들어졌다. 따라서 EUV를 위한 새로운
Inspection tool이 개발되어야 할 것이다.
5) Pellicle
EUV photomask contamination을 막는 용도로 사용되는 Pallicle은 EUV 에너지를 흡수하기 위한 매
우 얇은 shielding film이 필요하다. 하지만 EUV light source의 매우 높은 에너지로 인한 온도 상승과
물리적 손상을 견뎌내야 하기 때문에 내성이 더욱더 강한 pallicle 재료를 찾아야 한다.
- 8 -
6) Vacuum condition
EUV light는 매우 에너지가 크므로 모든 물질에 잘 흡수된다. 따라서 chamber 내를 항상 vacuum 상
태로 유지해야한다.
끝.
