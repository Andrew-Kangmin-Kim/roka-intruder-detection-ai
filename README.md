본연구는 국방부 및 해안 감시에 도움이 될 것이라 판단하여 저의 연구 의지를 보이고자 짧은 시간내에 완성한 프로젝트로서 현재로서는 프로토타입이자 알고리즘의 파이프라인을 테스트하는 수준의 연구임을 알립니다.
본연구는 classical computer vision technique, classical mathematical algorithm, modern llm technique 를 융합하여 비교적 적은 computing power 과 latency 를 사용하면서도 보다 정확한 cctv 영상내 침입자를 감지 할 수 있는 알고리즘을 모색한 내용입니다.
만약 이 연구를 추가적으로 진행할 수 있는 기회가 생긴다면 아래의 내용들을 중점적으로 수정 및 보완 하고자 합니다.
1. "motion" 감지 알고리즘 강화 + moving average based anomaly detection 로직 강화 (exponentially weighted moving average 사용 가능성, 다른 time series analysis 모델을 사용한 anomaly 감지 가능성 고려등)
2. event segmentation 로직 강화 (현재는 단순 가까운 time stamp 들을 하나의 segment로 분류하였으나 이 또한 다른 clustering algorithm이나 filtering layer를 통한 관리 필요)
3. 영상 프레임 단위에 대한 더 효윻적인 방안 모색 (현재는 0.2초당 프레임을 끊어서 관찰이지만 현실적으로 침입자의 파악을 위해서는 lower granularity 프레임 사용 가능, 가장 효윻적인 프레임 수 연구 필요)
4. Open AI API를 다른 로컬 모델로 교체 (보안성 및 latency 이슈)
5. 더 많은 영상 자료들을 통한 철저한 성능 점검 (현재는 사용가능한 영상 자료가 매우 한정적이라 알고리즘의 성능 확인에 한계가 있었으나 이를 국방부의 자료들로 강화하고자 함)
