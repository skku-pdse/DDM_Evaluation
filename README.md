# Data-driven models for forecasting multi-step ahead profiles of mammalian cell culture performance towards bioprocess digitial twins

Seo-Young Park, Sun-Jong Kim, Cheol-Hwan Park, Jiyong Kim, Dong-Yup Lee*

School of Chemical Engineering, Sungkyunkwan University, Suwon, Republic of Korea

*Correspondence: Dong-Yup Lee, School of Chemical Engineering, Sungkyunkwan University, Suwon, Republic of Korea.

Email: dongyuplee@skku.edu

**ABSTRACT**
Recently, the advancement in process analytical techniques (PAT) and artificial intelligence (AI) has enabled the generation of enormous culture datasets from biomanufacturing processes that produce various recombinant therapeutic proteins (RTP), such as monoclonal antibodies (mAbs). Thus, now it is very important to exploit them for the enhanced reliability, efficiency and consistency of the RTP producing culture processes and for the reduced incipient or abrupt faults. It is achievable by AI-based data-driven models (DDMs) which allow us to correlate biological and process conditions and cell culture states. In this work, we provide practical guidelines for choosing the best combination of model elements to design and implement successful DDMs for given hypothetical inline data sets during mAb-producing Chinese hamster ovary (CHO) cell culture, as such enabling us to forecast dynamic behaviors of culture performance such as viable cell density, mAb titer as well as glucose, lactate and ammonia concentrations. To do so, we created DDMs that balance computational load with model accuracy and reliability by identifying the best combination of multi-step ahead forecasting strategies, input features, and AI algorithms, which is potentially applicable to implementation of interactive DDM within bioprocess digital twins. We believe this systematic study can help bioprocess engineers start developing predictive DDMs with their own datasets and learn how their cell cultures behave in near future, thereby rendering proactive decision possible.

**KEYWORDS:** CHO cell culture, data-driven model, artificial intelligence, machine learning, culture performance prediction, bioprocess digital twin


# Evaluation Framework

<img src="docs/main_Figure.png" width="1000"/>

# Data Examples

>## File Names
>input_vcd.csv
>input_viability.csv
>input_glucose.csv
>input_lactate.csv
>input_ammonia.csv
>input_do.csv
>input_ph.csv
>input_igg.csv
>## Data Table Examples 
> shape: (81,4)
>|condition|t1|t2|t3|
>|---|---|---|---| 
>|P1|0|0|0|
>|P2|0|0|0|
>|⋮|⋮|⋮|⋮|
>|P4|0|0|0|

>## File Names
>output_vcd.csv
>output_glucose.csv
>output_lactate.csv
>output_ammonia.csv
>output_igg.csv
>## Data Table Examples 
> shape: (81,2)
>|condition|t4|
>|---|---|
>|P1|0|
>|P2|0|
>|⋮|⋮|⋮|⋮|
>|P4|0|

>## File Names
>vcd.csv
>viability.csv
>glucose.csv
>lactate.csv
>ammonia.csv
>do.csv
>ph.csv
>igg.csv
>## Data Table Examples 
> shape: (17,9)
>|condition|d0|d2|d4|d6|d8|d10|d12|d14|
>|---|---|---|---| ---| ---| ---| ---|---| 
>|P1|0|0|0|0|0|0|0|0|
>|P2|0|0|0|0|0|0|0|0|
>|⋮|⋮|⋮|⋮|⋮|⋮|⋮|⋮|⋮|
>|P4|0|0|0|0|0|0|0|0|

# Acknowledgement
This study was supported by the National Research Foundation of Korea (NRF) grant funded by Ministry of Science and ICT (2022R1A4A5032720), and the Korea Institute of Energy Technology Evaluation and Planning (KETEP) grant funded by the MOTIE (20214000000500, Training program of CCUS for the green growth).
