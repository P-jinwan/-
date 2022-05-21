# 테마별 제주도 관광지 추천 시스템</br>(Recommended tourist attractions in Jeju Island by theme)
- 수행 기간(period): 22.04.07 ~ 22.04.22 (16일)
---

## 팀 구성 및 역할(Teaming and Roles)
- `프로젝트 매니저(PM)` - 민경태(min-moon-sick)
- `데이터 수집 및 전처리(Data collection and preprocessing)` - 박진완(P-jinwan)
- `챗봇 개발(chatbot)` - 민경태(min-moon-sick), 김인성(khdbsfdk)
- `추천 시스템 개발(Recommended system)` - 손찬우(son556), 박진완(P-jinwan)
- `웹 개발(Web)` - 김동현
---

## 최종 시연 영상(Final demonstration video)
![ezgif com-gif-maker](https://user-images.githubusercontent.com/96413630/169300654-96758426-43b4-4cf9-be07-f75f752ca6a8.gif)  

---

## 목차(Contents)
1. [프로젝트 개요](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/README.md#%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EA%B0%9C%EC%9A%94)
2. [프로젝트 수행 절차](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/README.md#%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%88%98%ED%96%89-%EC%A0%88%EC%B0%A8)
3. [출처 및 참고 사이트](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/README.md#%EC%B6%9C%EC%B2%98-%EB%B0%8F-%EC%B0%B8%EA%B3%A0-%EC%82%AC%EC%9D%B4%ED%8A%B8)
4. [개선 사항 및 어려웠던 점과 느낀 점](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/README.md#%EA%B0%9C%EC%84%A0-%EC%82%AC%ED%95%AD-%EB%B0%8F-%EC%96%B4%EB%A0%A4%EC%9B%A0%EB%8D%98-%EC%A0%90%EA%B3%BC-%EB%8A%90%EB%82%80-%EC%A0%90)
---

## 프로젝트 개요

### 1. 프로젝트 선정 배경
- 지인에게 관광지 추천을 해줬던 경험에서 아이디어를 얻어 프로젝트의 주제로 선정하게 되었습니다.

### 2. 프로젝트 기대 효과
- 사용자가 직접 관광지를 찾지 않고 원하는 테마를 입력해 주면 적합한 관광지를 추천해 주기 때문에 편리하며, 여행의 만족도를 높일 수 있습니다.

### 3. 구현 기능
- 사용자가 원하는 관광지 테마 입력을 받는 챗봇
- 입력된 테마에 가장 적합한 관광명소 상위 n 개를 추천해 주는 추천 시스템
- 과정과 결과를 시각화하는 GUI

### 4. 개발 환경
- 사용 언어 - Python 3.7 ~ 3.8
- 코드 편집기 - Jupyter notebook, Colab
- 운영 체제 - Window
---

## 프로젝트 수행 절차
1. [아키텍처](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/README.md#1-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%88%98%ED%96%89-%EC%A0%88%EC%B0%A8---%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98)
2. [웹](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/edit/master/README.md#2-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%88%98%ED%96%89-%EC%A0%88%EC%B0%A8---%EC%9B%B9)
3. [챗봇](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/edit/master/README.md#3-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%88%98%ED%96%89-%EC%A0%88%EC%B0%A8---%EC%B1%97%EB%B4%87)
4. [추천 시스템](https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/edit/master/README.md#4-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%88%98%ED%96%89-%EC%A0%88%EC%B0%A8---%EC%B6%94%EC%B2%9C-%EC%8B%9C%EC%8A%A4%ED%85%9C)

### 1. 프로젝트 수행 절차 - 아키텍처
![20220519_225642](https://user-images.githubusercontent.com/96413630/169311045-5a65df61-7646-45f3-be2d-9d426fe93d03.png)

### 2. 프로젝트 수행 절차 - 웹
- flask 학습 및 웹 페이지 구현 (최종 실패)
- 시간 이슈로 GUI로 대체

### 3. 프로젝트 수행 절차 - 챗봇

#### (1) 챗봇을 사용한 이유
- 사용자가 정확히 어떤 테마의 여행이 좋은지 갈피를 못 잡고 있을 때, 일상적인 대화를 통해 정보를 입력받아 적합한 테마의 관광지를 추천하고자 사용하게 되었습니다.

#### (2) 챗봇의 종류
- 챗봇을 크게 2가지로 나누었습니다.
  1. 일상적인 대화를 통해 키워드를 추출하여 추천을 해주는 **일상 대화 추천 챗봇**
  2. 목적이 추천이 아니어도 자연스럽게 흐름을 이어나가는 **자유 주제 챗봇**
- 본 프로젝트는 여행지 추천에 프로젝틔 의미가 있으며, 시간이 정해져있는 교육기관 프로젝트 특성상 시간 이슈로 인해 1번의 "문제 해결용 챗봇 개발"에 중점을 두었습니다.

#### (3) 챗봇 데이터 생성
- 추천 관련한 일상 대화 데이터를 구하지 못하여 코드를 짜서 데이터를 직접 생성하였습니다.
- 데이터를 생성한 코드는 다음과 같습니다.
``` python
dict_thema = {'관광 명소' : ['관광 명소', '리조트', '온천', '아쿠아리움', '제주시', '추자면', '조천읍', '구좌읍', '애월읍',
                            '한경면', '한림읍', '우도', '성산읍', '표선면', '남원읍', '서귀포시', '안덕면', '대정읍'],
              '주소' : [],
              '역사' : ['4.3', '너븐숭이', '문화', '문화 관광', '문화 유적지', '역사 유적지', '신나락 만나락', '사찰', '절', '토기', 
                       '제주4.3', '전통', '신화탐방로', '북촌'],
              '자연' : ['경관/포토', '생태', '생태문화', '야영장', '세계자연유산', '숲길', '캠핑장',' 일몰', '오름', '섬',
                        '일몰 명소', '일출', '제주 동백 수목원', '코스모스', '자연 경관', '유네스코', '산', '둘레길', '등산길',
                        '유채꽃', '폭포', '한옥', '캠핑', '해바라기', '계곡', '숲', '노천탕', '바다', '공원', '올레길',
                        '동굴', '글램핑', '동백나무', '동백', '매화', '억새','용천수', '휴양림', '자연'],
              '사진' : ['커플 스냅', '우정 스냅', '포토 스팟'],
              '도보' : ['도보','도보 여행', '마을 산책', '마을 관광', '산책로'],
              '예술' : ['미술관', '박물관', '미술', '미디어 아트', '예술', '아트', '전시', '행사',
                        '전시관', '전시와 행사', '뮤지컬', '연극'],
              '육상' : ['ATV', '골프', '산책', '걷기', '내창트레킹', '농촌 체험 마을', '드라이브', '동물 먹이주기', 
                        '등산', '레이싱', '메디컬 요가', '승마', '빈야사요가', '지질 트레일', '요가', 
                        '트레킹', '카트', '자전거', '체험', '체험관광', '체험여행', '테랍툴요가', 
                        '플라잉 요가','테마 파크', '테마 공원', '어트랙션', '체험전시'],
              '수상' : ['해변', '해수욕장', '수상 레저', '낚시', '물놀이', '수영장', '다이빙 체험', '마린 스포츠',
                        '스쿠버 다이빙', '스쿠버 교육', '액티비티', '차귀도 유람선', '해상 레저', '패들요가'],
              '공중' : ['라이딩'],
              '봄'   : ['벚꽃', '봄', '봄꽃'],
              '여름' : ['여름'],
              '가을' : ['가을', '단풍'],
              '겨울' : ['겨울'],
              '사계절' : ['사계절', '사계절'],
              '어린이' : ['아이들과', '애들과', '애들이랑', '애들 데리고'],
              '청년' : [],
              '중년' : [],
              '노년' : [],
              '혼자' : ['혼자서', '나 혼자서', '혼자', '홀로'],
              '친구' : ['친구들과', '친구와', '친구랑'],
              '커플' : ['애인과', '애인이랑', '여자 친구와', '남자 친구와', '여자 친구랑', '남자 친구랑'],
              '부모' : ['어머니와', '아버지와', '부모님과', '부모님과 함께'],
              '가족' : ['가족들과', '가족과']}
              
people = ['가족들과', '가족과', '친구들과', '친구와', '친구랑', '애인과', '애인이랑', '여자 친구와',
          '남자 친구와', '여자 친구랑', '남자 친구랑', '부모님과', '부모님과 함께', '아이들과',
          '애들과', '애들이랑', '애들 데리고', '어머니와', '아버지와', '혼자서', '나 혼자서', '혼자', '홀로']
place = ['오름', '둘레길', '숲', '공원', '섬', '휴양림', '계곡', '산', '등산길', '해수욕장', '해변', '리조트',
        '온천', '폭포', '박물관', '아쿠아리움', '테마 파크', '전시관', '미술관', '관광 명소', '올레길', '행사',
        '야영장', '산책로', '일몰 명소', '수영장']

# 라벨 지정
def find_thema(word, dict_thema) :
    dict_thema_list = ['관광 명소','역사', '자연', '사진', '도보', '예술', '육상', '수상', '공중', '봄', '여름',
                       '가을', '겨울', '사계절', '어린이', '혼자', '친구', '커플', '부모', '가족']

    for i in dict_thema_list :
        if word in dict_thema[i] :
            break
        else :
            continue
    return i

Q_data = []
key = []

# 예시1 -> {사람들과} 갈만한 {장소} 추천해줘
for p in people :
    for i in place :
        key_a = []
        sentence = f"{p} 갈만한 {i} 추천해줘"
        key_1 = find_thema(p, dict_thema)
        key_2 = find_thema(i, dict_thema)
        if key_1 != key_2 :
            key_a.append(key_1)
            key_a.append(key_2)
        elif key_1 == key_2 :
            key_a.append(key_1)
        Q_data.append(sentence)
        key.append(key_a)
print(Q_data)
print(key)
```
- 과정을 거쳐 생성된 데이터는 다음과 같습니다.
<img width="100%" src="https://user-images.githubusercontent.com/84302953/165202738-472c6e1d-0cf9-4fc9-b6d1-b4a84e44ce46.png"/>

#### (4) 챗봇 학습 진행
- 챗봇 개발에 사용된 모델은 transformers의 bert입니다.
``` python
model = SentenceTransformer('sentence-transformers/xlm-r-100langs-bert-base-nli-stsb-mean-tokens')
```
- 저장한 챗봇 데이터 프레임에 임베딩 값을 구한 후 코사인 유사도를 구합니다.
<img width="100%" src="https://user-images.githubusercontent.com/84302953/165212133-f03b723b-d3e9-443d-9a0e-6c6d266dd420.png"/>

- 질문 문장을 넣으면 학습 문장 중 가장 유사한 문장을 찾아 답변합니다.
<img width="80%" src="https://user-images.githubusercontent.com/84302953/165212338-c943ad19-318f-4ed3-bc38-e0bd1c7dbf46.png"/>

### 4. 프로젝트 수행 절차 - 추천 시스템

#### (1) 데이터 수집
- 관공서나 공공 포털에서 제주도와 관련된 모든 데이터를 수집하였습니다.
- [비짓 제주](https://www.visitjeju.net/kr)에서 Selenium 라이브러리를 사용하여 상점, 음식점, 관광 명소 데이터를 크롤링 하였습니다.

#### (2) 데이터 선정
- 테마와 관련된 관광지를 추천하기 위해서 먼저 **테마 태그**가 필요하였고 두 번째로 관광 명소의 주소지와 이름이 필요하였습니다.
- 수집한 데이터들 중 위 조건에 충족하는 데이터는 [이 짓 제주](https://www.visitjeju.net/kr)에서 크롤링 한 데이터로 최종적으로 크롤링 데이터를 학습 데이터로 선정하였습니다.
- 관공서나 공공 포털에서 수집한 데이터는 필요에 따라 가공하여 크롤링 데이터와 섞어서 사용하였습니다.
- 최종적으로 선정된 데이터는 다음과 같습니다.

![1](https://user-images.githubusercontent.com/96413630/169644332-1cceaa03-112c-423a-977f-a1808791525d.png)

#### (3) 데이터 정제
- 지역별로 데이터의 편차가 커 지역을 그룹화하였습니다. 그룹화 기준은 다음과 같습니다.

![지역 그룹 기준](https://user-images.githubusercontent.com/96413630/169644681-133f0881-edcd-453f-8c5b-94e268373007.png)
- 데이터의 특수문자를 제거한 뒤 테마 태그 유의어를 묶어서 사용하였습니다.
- 같은 의미의 테마 태그 유의어를 하나의 테마 태그로 묶습니다. 예를 들어 '아이'와 '어린이'는 아이 또는 어린이라는 같은 성격을 가지고 있기 때문에 굳이 둘로 나눌 필요 없이 하나의 테마 태그로 묶어서 처리합니다.

![2](https://user-images.githubusercontent.com/96413630/169644816-137fb862-fbd0-4bd8-8bb3-c9120cff2217.png)
- 유의어 처리가 끝난 뒤 각 테마의 큰 카테고리를 정의 한 후 관광 명소의 카테고리별 테마 태그 개수를 세어 데이터 프레임으로 변환합니다.

![3](https://user-images.githubusercontent.com/96413630/169644912-1e1dbf98-bc39-4992-8801-47bdcbaba95e.png)

#### (4) [모델 선정(ALS: Alternating Least Squares)](https://yeomko.tistory.com/8?category=805638)
- 추천 알고리즘으로 유저 협업 필터링 기반의 **ALS 알고리즘**을 사용하였습니다.
- **ALS 알고리즘**: 행렬 분해를 최적화하는 잠재 요인의 유저 협업 필터링 기반의 추천 알고리즘으로서, loss function이 최소가 되는 행렬 x, y를 추출하는 데 목적을 가진 알고리즘입니다.
- 선택 이유: 사용자가 선택하지 않은 테마에 대해서 유의미한 영향을 끼치지 않는다라고 판단하는 것은 옳지 않다고 생각했습니다. 따라서 선택하지 않은 태그, 잠재 요인도 고려하여 사용자가 선택한 테마에 가장 적합한 장소를 추천하기 위해 선정하게 되었습니다.
- https://github.com/P-jinwan/recommended_tourist_attractions_in_Jeju_Island_by_theme/blob/master/%EC%BD%94%EB%93%9C%20%EB%AA%A8%EC%9D%8C/%EC%B6%94%EC%B2%9C%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%BD%94%EB%93%9C/recommended_systems(ALS_final_version).ipynb

#### (5) 알고리즘 수행 절차
- 입력 데이터 + 학습 데이터 ALS 행렬 연산 수행
- 입력 데이터와 학습 데이터 간의 코사인 유사도 연산 수행
- 코사인 유사도를 기준으로 상위 10개의 데이터(행 인덱스 번호, 행렬) 추출
- 입력 데이터와의 태그 부합 개수를 기준으로 랭크 정렬
- 상위 n 개의 관광지 명과 상세 주소 출력
<img width="80%" src="https://user-images.githubusercontent.com/84302953/165258890-c627432a-a253-4730-bf7c-eb80856bebb0.png"/>

#### (6) 성능 평가
- 추천 시스템의 성능 평가 관련해서 다방면으로 찾아보았으나 평가용으로 적절한 방법을 찾지 못하였습니다. 그래서 직접 원본 데이터와 비교하여 입력 테마에 대해 적합한 장소를 추출하였는지 확인하였습니다. 아래 그림을 살펴보면 입력 테마(파란색 셀)에 대해 테마 개수와 유사도를 기준으로 적합한 장소를 추천(노란색 셀) 했음을 알 수 있습니다.

![4](https://user-images.githubusercontent.com/96413630/169645382-720f6f33-931e-4bc0-a0bf-18e7da4aae7d.png)

## 출처 및 참고 사이트
- 관광 데이터 -> [비짓 제주](https://www.visitjeju.net/kr/), [한국 관광 데이터랩](https://datalab.visitkorea.or.kr/datalab/portal/main/getMainForm.do)
- 챗봇 -> [송영숙님 깃허브](https://github.com/songys/Chatbot_data), [BERT의 문장 임베딩(SBERT)을 이용한 한국어 챗봇](https://wikidocs.net/154530)
- 추천 알고리즘 구현 -> [갈아먹는 머신러닝](https://yeomko.tistory.com/4?category=805638)

## 개선 사항 및 어려웠던 점과 느낀 점

### 1. 개선 사항
- 웹 페이지 구현을 통한 결과 시각화
- 추천 시스템 속도 개선
- 장소를 연결하여 경로 추천
- 별점, 리뷰등 참고 자료 추가
- 챗봇 성능 향상

### 2. 어려웠던 점
- 전체: 첫 팀 프로젝트로 데이터 선정부터 불협화음이 있었습니다.
- 챗봇: 챗봇 학습용 데이터가 없어 데이터 생성 과정이 힘들었습니다.
- 추천 시스템: 추천 시스템을 딥 러닝으로 구현하고 싶었으나 얕은 지식으로 구현의 한계가 있었습니다.
- 웹: 웹 페이지 구현이 어려웠습니다.

### 3. 느낀 점
- 민경태: 파이널 프로젝트를 경험하면서 구성원 간의 소통과 계획에 대한 중요성을 깨달을 수 있었던 유의미한 경험이었습니다.
- 김동현: 알려고 노력한다기보다는 모르는 것을 아는 과정을 체화하기 위해 노력해야 한다는 것이었습니다.
- 손찬우: 모은 데이터를 많이 살릴 수 없어서 아쉬웠습니다.
- 김인성: 미숙한 프로젝트였지만 데이터 수집, 시간 배분, 협업과 소통 등의 중요성을 깨달을 수 있는 시간이었습니다.
- 박진완: 프로젝트의 흐름을 알게 되었고 소통과 계획의 중요성을 깨달았습니다. 모르는 분야에 대해 공부할 수 있어 좋았고 다른 사람의 코드를 최적화하는 과정을 거치며 코딩 실력을 높일 수 있는 좋은 시간이었습니다.
