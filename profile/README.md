# ⛵ Story Boat
### 공동 소설 제작 어플리케이션

| Notion Page | 프로젝트 팀 |
| --- | --- |
| [💡 아이디어 회의](https://www.notion.so/e2a75d5db39c432e95c096f2bf558460?pvs=21) <br> [🍎 기획 (전체적인 구조)](https://www.notion.so/fa33869faa9643719dfca196efa3a2e9?pvs=21) <br> [👩‍💻 구체적인 활동](https://www.notion.so/f167ad912d29416581839b5bef1c9717?pvs=21) <br> [📆 스케줄표 ](https://www.notion.so/fd50942fabb84e7e83a8be362de9f70b?pvs=21) <br> [👨‍🔧 필수 구현기능 ](https://www.notion.so/622185bd971042ea943d3159368d7ee3?pvs=21) <br> [📝 자료조사](https://www.notion.so/577d4a3bbcff4c1c9ccfefb92d5fec13?pvs=21) | 🙋 박보람 <br> 👩‍💼 김연지 <br> 👩‍🏫 정소영 <br> 🙆‍♂️ 서한빈 <br> 👨‍💻 이중현 <br> 👨‍🔧 김시온 <br> |

---
## 목차

### 🐱 I. 팀원 정보 및 업무 분담 내역

### 📊 II. 설계 내용 (아키텍처 등) 및 실제 구현 정도

### 📑 III. 데이터베이스 모델링(ERD)

### 💻 IV. 서비스 대표 기능들에 대한 기술적 설명

### 💁 V. 구현된 어플 DEMO 페이지 

### 🙇 VI. 느낀 점


---

## 🐱 I. 팀원 정보 및 업무 분담 내역

- 프로젝트 기간 : 2024.07.02(화) ~ 2024.08.16(금)

<table>
  <tr>
    <th rowspan="3">Front</th>
    <td>박보람</td>
    <td>Figma, UI/UX, React, 레이아웃</td>
  </tr>
  <tr>
    <td>김연지</td>
    <td>Figma, UI/UX, React, 로그인 & 로그아웃 기능</td>
  </tr>
  <tr>
    <td>정소영</td>
    <td>React, 이미지 생성 AI, 텍스트 생성 AI</td>
  </tr>
  <tr>
    <th rowspan="1">Full Stack</th>
    <td>서한빈</td>
    <td>WebRTC 기능구현, SpringBoot, UCC</td>
  </tr>
  <tr>
    <th rowspan="2">Back</th>
    <td>이중현</td>
    <td>JPA, SpringBoot</td>
  </tr>
  <tr>
    <td>김시온</td>
    <td>CI/CD 구축, 인프라</td>
  </tr>
</table>


---

## 📊 설계 내용 (아키텍처 등) 및 실제 구현 정도

- **기술 스택 🔧**
![Skill](https://github.com/Story-Boat/Ideathon/blob/main/ERD/%EA%B8%B0%EC%88%A0%EC%8A%A4%ED%83%9D2.png?raw=true)

|  | Front | Back | Infra |
| --- | --- | --- |  --- |
| Language | JavaScript | Python | ddd |
| Framework | Vue3<br>Pinia (+Pinia-plugin-persistedstate)<br>vuetify<br>axios<br>chart.js | django<br>django-rest-framework<br>django-rest-auth<br>drf-spectacular | ddd |

- 협업 도구

Jira, Git & Github, Mattermost
![📎 Jira  ](https://github.com/Story-Boat/Ideathon/blob/main/Jira/Cap%202024-08-08%2023-38-50-202.png?raw=true).
![📎 Jira  ](https://github.com/Story-Boat/Ideathon/blob/main/Jira/Cap%202024-08-08%2023-38-21-599.png?raw=true).
![📎 Jira  ](https://github.com/Story-Boat/Ideathon/blob/main/Jira/Cap%202024-08-08%2023-38-15-144.png?raw=true).


## 프런트엔드 화면 디자인 설계
### 🎨 Figma 
[📎 Figma Link  ](https://www.figma.com/design/I7G6UwDk6q77acJHXI0o4J/ssafy-%EA%B3%B5%ED%86%B5?node-id=0-1&t=9wMHmHweJ2Ckecuf-1).


![Figma](https://github.com/Story-Boat/Ideathon/blob/main/Figma/figma.png?raw=true)

메인 페이지, 로그인, 회원가입, 로그아웃, 프로필페이지(마이펫 포함), 금리 비교 (데이터 저장, 전체 조회, 상세 조회), 환율계산기, 은행검색, 커뮤니티, 금융 상품 추천 알고리즘 등 계획했던 기능을 모두 구현하였습니다.  

## 백엔드 데이터 설계
### 📑데이터베이스 모델링 (ERD)
📎 ERD Drawing 

![ERD 이미지](https://github.com/Story-Boat/Ideathon/blob/main/ERD/2.%EC%B9%BC%EB%9F%BC%EC%B6%94%EA%B0%80.png?raw=true)
![ERD 이미지](https://github.com/Story-Boat/Ideathon/blob/main/ERD/4.%EB%AA%BD%EA%B3%A0DB%EB%A5%BC%20%EA%B3%A0%EB%A0%A4%ED%95%9C%20ERD.png?raw=true)

📎 Architecture

![Architecture](https://github.com/Story-Boat/Ideathon/blob/main/ERD/%EC%95%84%ED%82%A4%ED%85%8D%EC%B3%90(%EA%B0%9C%EC%84%A0%EC%95%88).jpg?raw=true)

### 🗂️ API 명세서 
사용한 API : 카카오맵, 한국수출입은행 환율정보, 금융감독원, GPT OPEN AI
<br>
[API 명세서](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/%EA%B3%B5%ED%86%B5%20PJT%20%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%20%EC%A0%95%EB%A6%AC%20-%20API%20%20%EB%AA%85%EC%84%B8%EC%84%9C2.pdf)

요구사항 명세서 
![요구사항 명세서1](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%20%EB%AA%85%EC%84%B8%EC%84%9C1.png?raw=true)
![요구사항 명세서2](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%20%EB%AA%85%EC%84%B8%EC%84%9C2.png?raw=true)

기능 명세서 
![기능명세서1](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/REAME%EC%9A%A9/%EA%B8%B0%EB%8A%A5%EB%AA%85%EC%84%B81.png?raw=true)
![기능명세서2](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/REAME%EC%9A%A9/%EA%B8%B0%EB%8A%A5%EB%AA%85%EC%84%B82.png?raw=true)
![기능명세서3](https://github.com/Story-Boat/Ideathon/blob/main/%EB%AA%85%EC%84%B8%EC%84%9C/REAME%EC%9A%A9/%EA%B8%B0%EB%8A%A5%EB%AA%85%EC%84%B83.png?raw=true)

---
## 💻금융 상품 추천 알고리즘에 대한 기술적 설명
### 추천 알고리즘 1️⃣
동일하게 1만명의 유저 더미데이터를 생성합니다. 이 후에  나이, 자산, 연봉이 비슷한 유저가 많이 가입한 금융 상품을 추천해줍니다. 먼저는 코사인 유사도(cosine similarity)를 사용하여 비슷한 유사도를 가진 금융상품을 분석합니다. 이 후에 추천하는 상품을 1등부터 6등까지 보여줍니다. 

### 추천 알고리즘 2️⃣
동일하게 1만명의 유저 더미데이터를 생성합니다. 사용자가 선호하는 은행을 고려하여 해당 은행의 상품을 우선적으로 고려합니다. 사용자의 저축 성향을 분석하여 상, 중, 하로 나눕니다. (상 : 24개월 이상 저축, 중: 12개월~24개월 저축, 하: 12개월 이하) 이렇게 나눠진 그룹 그 중에서 가장 금리가 높은 상품을 추천합니다. 추가로 연봉과 자산을 고려하여 예금과 적금을 구별하고, 사용자에게 맞는 상품을 추천하게 설계가 되어있습니다. 이렇게 세심한 고려와 다양한 요소를 고려한 추천 알고리즘은 사용자에게 현명한 금융 결정을 돕는 데 큰 도움이 될 것입니다.
<br>
## 예상 질문
1. 사이킷런 라이브러리 코사인 유사도를 사용하여 추천 알고리즘을 만들었는데, 코사인 유사도 분석의 의미와, 사용된 자료는 연봉, 자산, 나이로 1차원 벡터인데 어떻게 하여 코사인 유사도 분석이 의미가 있을 수 있는지 답변하시오.
2. API를 사용하여 구현한 기능이 많은데, 카카오맵과 환율계산기는 front에서 직접 랜더링 시킬 경우 CROS 에러가 발생하는 데 이것에 대한 설명과 회피할 수 있는 방법을 설명하시오 
## 예상 질문 답변
### 1. 코사인 유사도 분석의 의미와 1차원 벡터의 유의미성

#### 코사인 유사도 분석의 의미

코사인 유사도(Cosine Similarity)는 두 벡터 간의 유사도를 측정하는 방법으로, 벡터가 이루는 각도의 코사인을 사용합니다. 코사인 값이 1에 가까울수록 두 벡터는 같은 방향을 가리키며, 0에 가까울수록 서로 직교하고, -1에 가까울수록 반대 방향을 가리킵니다. 주로 텍스트 마이닝, 추천 시스템, 클러스터링 등에서 사용됩니다. 유사도를 계산할 때 벡터의 크기보다 방향이 더 중요하게 고려됩니다.

#### 1차원 벡터와 코사인 유사도의 유의미성

일반적으로 코사인 유사도는 다차원 벡터 간의 유사도를 측정하는 데 사용됩니다. 그러나 질문에서는 연봉, 자산, 나이라는 1차원 벡터를 사용하여 코사인 유사도를 계산한다고 했습니다. 1차원 벡터에서 코사인 유사도를 사용하는 것은 의미가 없으며, 1차원 벡터의 경우 유사도는 항상 1이 됩니다. 따라서, 여기서 1차원 벡터가 아닌 3차원 벡터로 구성된 자료를 의미하는 것으로 해석할 수 있습니다.

만약 연봉, 자산, 나이를 각각의 축으로 하는 3차원 벡터라면, 이는 코사인 유사도 분석을 통해 개인 간의 유사성을 비교하는 데 유의미할 수 있습니다. 예를 들어, 벡터 A가 [연봉_A, 자산_A, 나이_A], 벡터 B가 [연봉_B, 자산_B, 나이_B]로 주어진다면, 두 벡터 간의 코사인 유사도는 다음과 같이 계산됩니다:

\[ \text{Cosine Similarity}(A, B) = \frac{A \cdot B}{\|A\| \|B\|} \]

이렇게 하면 연봉, 자산, 나이 간의 상관 관계를 통해 두 사람의 유사성을 평가할 수 있습니다. 예를 들어, 연봉이 높고 자산이 많으며 나이가 비슷한 두 사람은 유사도가 높게 나올 것입니다.

### 2. CORS 에러의 설명과 회피 방법

#### CORS 에러 설명

CORS(Cross-Origin Resource Sharing) 에러는 웹 브라우저에서 보안상의 이유로 발생하는 문제로, 한 도메인에서 실행 중인 웹 애플리케이션이 다른 도메인의 리소스에 접근하려 할 때 발생합니다. 이는 웹 페이지가 악의적인 요청을 보내는 것을 방지하기 위한 보안 기능입니다. 예를 들어, `http://example.com`에서 실행되는 스크립트가 `http://another-domain.com`의 API에 접근하려 하면 CORS 정책에 의해 차단될 수 있습니다.

#### CORS 에러 회피 방법

CORS 에러를 회피하는 방법은 여러 가지가 있습니다:

1. **서버에서 CORS 설정 변경**:
   API 서버에서 응답 헤더에 `Access-Control-Allow-Origin`을 설정하여 특정 도메인 또는 모든 도메인(`*`)에서의 접근을 허용할 수 있습니다.
   ```http
   Access-Control-Allow-Origin: *
   ```
   그러나 모든 도메인을 허용하는 것은 보안상 위험할 수 있으므로, 신뢰할 수 있는 도메인만 허용하는 것이 좋습니다.

2. **프록시 서버 사용**:
   프론트엔드에서 직접 API 서버에 요청하는 대신, 같은 도메인에서 운영되는 프록시 서버를 사용하여 API 요청을 전달합니다. 예를 들어, 프론트엔드에서 프록시 서버에 요청을 보내고, 프록시 서버가 API 서버에 요청을 보내는 방식입니다.

   ```javascript
   // 예: Node.js Express를 사용하는 간단한 프록시 서버
   const express = require('express');
   const request = require('request');
   const app = express();

   app.get('/proxy', (req, res) => {
     const apiUrl = 'http://another-domain.com/api';
     req.pipe(request(apiUrl)).pipe(res);
   });

   app.listen(3000, () => {
     console.log('Proxy server listening on port 3000');
   });
   ```

3. **JSONP 사용**:
   JSONP(JSON with Padding)를 사용하는 방법도 있지만, 이는 GET 요청만 지원하고 보안 문제가 있어 현대 웹 애플리케이션에서는 권장되지 않습니다.

4. **브라우저 확장 프로그램 사용**:
   개발 환경에서만 사용되는 방법으로, 브라우저 확장 프로그램을 통해 CORS 정책을 우회할 수 있습니다. 예를 들어, "CORS Unblock" 같은 확장을 사용하면 됩니다. 하지만 이는 배포 환경에서는 사용할 수 없는 방법입니다.
   <br><br>위의 방법들을 사용하여 CORS 에러를 회피할 수 있습니다. 배포 환경에서는 주로 서버 측에서의 CORS 설정 변경이나 프록시 서버 사용을 통해 해결하는 것이 일반적입니다.
---

## 💁 서비스 대표 기능들에 대한 설명
### 1️⃣ 메인페이지
![메인페이지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fl9nt6%2FbtsHy6Yq8Ym%2FbmJ3ewJbs1F2vIMFCXjQq1%2Fimg.jpg)
<br><br>네비게이션바를 사용해서 반응형으로 제작
<br>JavaScript 코드를 Vue 코드로 변환하여 애니메이션 기능 추가
<br>
### 2️⃣ 로그인, 회원가입 페이지 
![로그인 페이지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FPBBOW%2FbtsHyT53Ika%2FF8DoPYwrK31ARsZqSYZxz1%2Fimg.png)
![회원가입 페이지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fz9wQb%2FbtsHzHKDMlA%2FnioZDPveQioATwIrpDn6h0%2Fimg.png)
<br><br>회원 관리를 할 수 있는 기능(회원 가입, 로그인, 로그아웃 등)을 구성
<br>Django의 기본 User를 상속받아 커스텀 User를 구현함
<br>
### 3️⃣ 프로필 페이지
![프로필 페이지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FlCFPN%2FbtsHyDPYJDx%2FJxvZGltHMoWmV9NDOIWzp1%2Fimg.png)
![마이펫](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbmPiZc%2FbtsHxJi6fAV%2FDkLWkXQWaoeiD7gt5xiIu1%2Fimg.png)
<br><br>회원의 기본 정보를 출력할 수 있도록 적절한 화면 구성
<br> 

### 4️⃣ 금리비교 
![금리비교](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FDFI5H%2FbtsHyDvGm6l%2FNIZailKWbNAOvsuL8NbMXK%2Fimg.png)
<br>금융상품통합비교공시 API를 활용하여 금융 상품 정보 가져오기
<br> 상품 목록을 볼 수 있도록 적절한 화면을 구성
<br> 특정 상품 클릭 시 상세 정보를 볼 수 있도록 구현
<br>
### 5️⃣ 환율계산기
![환율계산기](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FkOoyP%2FbtsHzsAaEoT%2FcGMb7ydtzVTGUrJT0AKunk%2Fimg.png)
<br><br>한국 수출입은행 환율정보 API를 활용하여 현재 환율에 대한 정보 가져오기 
<br> 원화 입력 시 선택한 국가의 통화로 변환된 값을 출력하도록, 타국 통화 입력 시 해당 통화를 원화로 변환한 값 출력하도록 구성
<br>
### 6️⃣ 은행검색
![은행검색](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcEk7Ef%2FbtsHynzPWf3%2Fke9FK7mp8J5HiTeKASYlR0%2Fimg.jpg)
<br><br>Kakao Maps API를 활용하여 은행의 위치를 검색할 수 있도록 구현
 <br>
### 7️⃣ 커뮤니티 
![커뮤니티](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbrj0iv%2FbtsHAeuIAUT%2FVVAtlFGO2Qc11bPY2OxzM1%2Fimg.png)
<br>회원간 소통할 수 있는 커뮤니티게시판
<br> 조회, 생성, 삭제, 수정 기능 구현 (CRUD)
<br>
<br>
## 🙇 느낀점

<table>
  <tr>
    <th rowspan="3">Front</th>
    <td>박보람</td>
    <td>느낀점</td>
  </tr>
  <tr>
    <td>정소영</td>
    <td>느낀점</td>
  </tr>
  <tr>
    <td>김연지</td>
    <td>느낀점</td>
  </tr>
  <tr>
    <th rowspan="1">Full Stack</th>
    <td>서한빈</td>
    <td>느낀점</td>
  </tr>
  <tr>
    <th rowspan="2">Back</th>
    <td>이중현</td>
    <td>느낀점</td>
  </tr>
  <tr>
    <td>김시온</td>
    <td>느낀점</td>
  </tr>
</table>

<!-- ![로고](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbfQboG%2FbtsHw5Mluk1%2F0HfdpaLmjP8igs0TbvvoBk%2Fimg.png) -->
