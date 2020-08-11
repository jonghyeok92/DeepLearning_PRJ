
1. 프로젝트 명 : A deep learning approach for foot-type classification using heterogeneous pressure data
    - this is a project with paper : 'A deep learning approach for foot-type classification using heterogeneous pressure data'
    - 이 프로젝트의 과정, 결과의 상세 내용은 위 논문에 상세히 내용이 서술 되어 있으며, 코드 자료를 남기기 위해 Git에 저장하였습니다.
----------------------------------------------------------------
2. 설치
    - 본 프로젝트에 사용된 Deep learning 환경은 다음과 같습니다.
    - The learning environment for training and testing is based on Python 3.7 on PCs running Windows 10 with a 64-bit operating system and an x64-based processor, Intel (R) Xeon (R) CPU E5-2650 v4 @ 2.20 GHz processor, 8 GB RAM, and an Intel Xeon v4 processor. It was performed using a tensorflow2.0 GPU (GeForce GTX 1070) and the cuda compilation tool (Release 10.0, V10.0).
------------------------------------------------------------------
3. 참고 방법
    - 본 프로젝트의 모든 과정을 참고 할 필요는 없다고 생각합니다. 연구에서 주장하려 하는 것은 'Numerical data'와 'Image data'의 결과 데이터를 혼합(Stacking Ensemble) 하였을 때, 단일 종류의 데이터를 사용한 결과보다 높은 '정확도'와 모델 정확도의 편차를 줄여(강건성 확보) 좋은 결과를 발생시켰다는 것 입니다.
    - 역시, 동일한 방법으로 데이터를 수집하는 과정에서 '낮은 정확도'가 예측되는 모델 구축과정에서 '데이터 결과의 혼합'을 통해서 모델의 정확도와 강건성을 개선할 수 있을것으로 보입니다.
    - Ex. 동일한 제품으로 부터 얻을 수 있는 데이터의 종류가 많지만, 획득할 수 있는 데이터의 수는 작을 때, 연구 방법을 차용할 수 있습니다.
------------------------------------------------------------------
4. 프로젝트 과정 및 결과
    - 논문 순서에 맞추어 과정을 설명하겠습니다.
    - 데이터 수집 : 장비로 부터 수집되는 데이터를 'Numerical data'와 'Image data'로 한정하였습니다.
    - 데이터 전처리 : 각 데이터 type별로 일반적인 머신러닝, 딥러닝을 위한 전처리 과정이 수행되었습니다.
    - 인공지능 알고리즘 : 
        - 특성 데이터 : 특성 데이터를 학습하는 경우, 새로운 모델과 비교하기 위해 표준 모델로서 사용되는 K-NN(K-Nearest Neigbor)과 CART(Classificaiton and Regression Tree)를 사용했습니다. 
        - 이미지 데이터 : 적은 이미지 데이터의 학습 정확도를 높이기 위해 '전이학습'을 사용했습니다. 전이학습에 참고된 모델은 VGG-16net과 Inception V3모델을 사용했습니다. 전이 데이터는 이미지넷의 분류 데이터를 사용했고, 

사용 방법 (Header 2)
이 부분에 대해 작성할때는 최대한 간결한 설명이 될 수 있도록 하자
또한 다음에 대해 설명할 수 있어야 할 것이다.
어떤 Step을 밟아야 할까?
프로그램을 사용하기 위해 어떤 패키지/프로그램이 설치/설정 되어있어야 할까?
프로젝트에 대해 바로 이해하기에 어려운 점은 어떤 것들이 있을까?
Contribute

다른사람들이 코드에 contribute하기 쉽도록 설명하는 부분을 추가하도록 하자!
이 부분을 위해서 LICENSE를 기입해야할 필요가 있다.
어떤 LICENSE를 사용할지 모르면 아래 사이트를 참조하면 쉽게 선택할 수 있다!

https://choosealicense.com/

Code Status

Shield라고 불리는 것을 사용해보자
[build | passing]과 같은 정보를 줄 수있다.
일단 막 README를 작성한다면 이 부분에 대해서는 크게 신경쓰지말자
프로젝트가 커질수록 도움이 되는 부분
주의점

README를 처음부터 너무 복잡하게 작성하지 말자
코드를 작성하면서 프로젝트가 커질수록 README를 디테일하게 작성할 수 있도록 하는편이 바람직하다