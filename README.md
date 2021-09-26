# Red Blood Cell Transfusion Prediction in ICU

# I. Background

혈액제제는 제조되는 것이 아닌 헌혈자로부터 얻어야만 한다. 즉 한정된 양의 혈액제제를 효율적이고, 효과적으로 필요한 환자에게 수혈하는 것이 필수적이다. 따라서 수혈의 경우 객관적 기준과 지표가 마련되어야 한다.[1] 그러나 기존 수혈의 기준 지표는 아직 많은 논의가 이루어지고 있고, 임상상태를 완벽히 고려한 기준을 도출하지는 못했다. 특히 내과적 질환에서의 수혈 기준 지표는 더욱 미비하다.[2] 

본 연구는 수혈의 적정성을 인공지능으로 해결해보고자, 환자의 중환자실 입원 데이터를 활용하여, 주요 내과질환(Cadiology, Infection, Gastroenterology, Pulmonology)에서의 수혈 가능성 예측을 수행하였다.

# II. Methods

1. 데이터 : Medical Information Mart for Intensive Care III (MIMIC-III) 2001년부터 2012년까지 하버드 의대 교육 병원(Beth Israel Deaconess Medical Center)의 중환자실 입원 기록 데이터.
2. 전체 순서도

![Untitled](Red%20Blood%20Cell%20Transfusion%20Prediction%20in%20ICU%20acb773941a9c45888b306ca654a2ff90/Untitled.png)

// 마트다운 형식
![캡처](./캡처.PNG)
 
// 태그 형식
<img src="/uploads/1848994ad25765da30fa8ef3684c67bc/캡처.PNG"  width="700" height="370">


출처: https://cutemoomin.tistory.com/entry/Readme-파일에-이미지-넣기-마크다운-이미지 [무민은귀여워]
환자를 주요 진단 그룹으로 선별하고, 입력속성은 인구통계정보, 실험실 및 임상 검사 값을 활용함.

# III. Results

[The model performances](https://www.notion.so/c9465517529645c986ef358fa27464f0)

![Untitled](Red%20Blood%20Cell%20Transfusion%20Prediction%20in%20ICU%20acb773941a9c45888b306ca654a2ff90/Untitled%201.png)

LGBM Feature importance

# IV. Discussion

기존 선행 연구는 특정 질환이나 혹은 특정 수술에서의 수혈을 예측하는 경우가 많았다. 하지만 본 연구에서는 질환군을 확장하여 보편성을 넓히고자 하였고, 더하여 수술이 아닌 중환자 입원시 발생하는 수혈에 대해 예측을 수행하였다.

# V. References

[1] 양진혁, et al. "수혈 적정성 평가지표 개발." 주간 건강과 질병 12.41 (2019): 1696-1702.

[2] Yoon, Su Jin, et al. "Establishment of a Maximum Surgical Blood Order Schedule and Red Blood Cell Mean Transfusion Units Per Patient According to Adjacent Diagnosis Related Groups Patient Classification System." Laboratory Medicine Online 10.3: 235-241.
