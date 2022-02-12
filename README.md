# 🏆 2021학년도 SW Idea 공모전

### 아이디어명
 - i - 로드맵 과목 추천시스템
### 팀원
- 김묘경 ( https://github.com/data04190 )
- 백수민 ( https://github.com/baeksumin )
- 강현구 ( https://github.com/hyunku )


<br>
<img src = "https://user-images.githubusercontent.com/77683645/153438329-fb74bbbe-6f6c-42b7-97b6-fea86d0e0de3.png" height = 420><br>
<hr>

### 목 차
<ol>
 <li><a href = "#01">i - 로드맵 과목 추천시스템 제안 배경</a>
  <ul>
   <li><a href = "#01-1">i - 로드맵이란?</a>
   <li><a href = "#01-2">아이디어 제안 배경 및 문제점</a></ul>
 <li><a href = "#02">i - 로드맵 과목 추천시스템</a>
  <ul><li><a href = "#02-1">학년, 전공, 졸업 필수학점, 선이수 과목을 고려한 추천 알고리즘</a></ul>
 <li><a href = "#03">i - 로드맵 과목 추천시스템 기대효과</a>
 </ol>
<br><br>

<h2 id = "01">1. i - 로드맵 과목 추천시스템 제안 배경</h2>
 <br>

> <h3 id = "01-1">i - 로드맵이란? </h3>
> <img src = "https://user-images.githubusercontent.com/77683645/153632201-72480782-2d37-4eae-a1f1-e979c00b2656.png"><br> 
>  
>- 학부/ 과에서 제공한 전공 진출 분야 맞춤형 통합표준학습로드맵에 근거하여 전공 이수 목표 계획에 따라 본인의 전공, 타전공 계획을 스스로 설계함으로써 진출하고자 하는 분야에서 요구되는 역량을 습득하고 교육 목표를 달성하는데 도움을 주는 프로그램입니다.
> 
>- 또한, i - 로드맵 설계 교과목 중 해당 학기에 수립된 전공 교과목에 한하여 우선 수강신청 기회를 줌으로써 필수 전공임에도 본 수강신청에 실패해서 듣지 못하는 경우를 예방해줍니다.

<br>

<h3 id = "01-2">1.1 아이디어 제안 배경 및 문제점</h3>

- 대학 각 전공 홈페이지에 전공 진출 분야 맞춤형 통합표준학습로드맵이 존재하지만 학생 개개인의 `졸업 필수학점`, `전공(심화전공, 복수전공, 다전공)상황` 등을 고려하여 과목 설계해야 하기 
  때문에 과목을 설계하는 데 많은 시간이 소모되어 학생들의 i - 로드맵 참여율이 저조하다.
-  2021학년도 이후 신입생들은 제1전공 이외에 다전공을 반드시 이수해야 하지만, 현재 선택한 `다전공을 이수할 때의 상황`에 맞는 학습 로드맵 정보를 제공하고 있지 않다.
-  공대 이론·실습수업, 실기수업에서는 `권장하는 선이수 교과목`이 존재하지만 이를 고려하지 않고 수강했을 시 학생들이 수업의 기초지식이 없어 응용수업 내용을 따라가는 데 어려움이 있다.<br><br><br>

<h2 id = "02">2. i - 로드맵 과목 추천시스템</h2><br>
<img src = "https://user-images.githubusercontent.com/77683645/153707723-0387dede-b4ca-4cab-a57d-e1d5242716ac.png"><br>

<a href = "#01-2"> `1.1 아이디어 제안 배경 및 문제점` </a> 의 문제를 해결하기 위해 `학년`, `전공`, `졸업 필수학점`, `선이수 과목` 을 포함한 과목 추천시스템을 기획하였습니다.<br><br>
- <b>`학년`에 따른 추천</b>
   + 1학년 때에는 졸업 필수학점인 기초과목, 전공기초 과목, 2학년 때에는 전공심화, 3학년때에는 전공핵심, 4학년때에는 전공 응용 수업을 들을 수 있도록 학년에 따라 다르게 추천시스템 구현한다.<br>
- <b>`전공`에 따른 추천</b>
   + 전공 선택(심화, 복수, 다전공) 상황과 본 전공과  복수전공 과목의 가능한 조합에 따른 각각의 추천시스템을 구현한다. 
- <b>`졸업 필수학점`에 따른 추천</b>
   + 계열교양, 전공기초, 기초과목, 전공필수 등 졸업에 필요한 각 계열 최저 학점이 요구됨에 따라 그에 맞는 추천시스템을 구현한다.
- <b>`선이수 과목`에 따른 추천</b>
   + 수업명만을 보고는 알기 어려운 권장 선이수 과목을 추천해주어 학생들이 선이수 과목을 듣지 않아 수업내용을 따라가기 어려운 것을 방지하도록 추천시스템을 구현한다.<br><br><br>


<h3 id = "02-1">2.1 학년, 전공, 졸업 필수학점, 선이수 과목을 고려한 추천 알고리즘</h3><br>

<img src = "https://user-images.githubusercontent.com/77683645/153730777-f0629f42-e121-4876-8afb-e6a8c39c395f.png"><br><br>
데이터사이어스와 소프트웨어를 복수 전공하며 현재 2학년 1학기 시간표를 설계하고 있는 학생A가 있다고 가정한다.<br><br> 


1. 학생의 `학년`, `전공` 상황에 맞게 추천해주기 위해 전체 학생들 중 과목추천을 해주는 학생과 `동일한 학년` 때, `동일한 전공 조합`을 듣고 있는 학생들의 수강 과목 목록을 추출해준다.   
 학생 A의 경우 데이터사이언스와 소프트웨어를 복수전공 하고 있으므로, 데이터사이언스+소프트웨어전공을 복전한 학생들의 2학년 1학기까지 수강한 전공 과목들을 다음과 같이 추출해준다.  
 
   <img src = "https://user-images.githubusercontent.com/77683645/153731041-522b99f0-d657-4edb-ac44-09ebf77bda0d.png"><br><br>
2. 수강 과목 목록 중 `선이수 과목`이 존재한다면 그룹으로 묶어 한 과목으로 인식되도록 한다.  


   <img src = "https://user-images.githubusercontent.com/77683645/153731244-f36919f1-2a5f-4243-991f-25da0b287b6d.png"><br><br>
3. 0과 1로 이루어진 Sparse Matrix (희소 행렬)로 변환해준다.

    <img src = "https://user-images.githubusercontent.com/77683645/153731366-f1990773-3635-41a3-b0bf-406738a550f6.png"><br><br>
4. 단일 항목집단을 생성하고 각 과목들의 지지도를 계산한 뒤, 최소 지지도 미만의 과목들은 추천 과목 리스트에서 제거한다.
   (이 때 최소지지도를 0.5라고 가정한다.)


    <img src = "https://user-images.githubusercontent.com/77683645/153731488-2d2808a3-bf65-4e6a-b17d-5e1a0e3a52b3.png"><br><br>
    <img src = "https://user-images.githubusercontent.com/77683645/153731534-76a4dece-d4f7-4d82-b18e-d4b784988f15.png"><br><br>
5. 많이 수강하는 과목들 순으로 정렬시켜 준 후, 루트 노드를 생성하여 첫 번째 부모 노드와 연결시켜주며 트리를 생성한다.
   이때, 새로운 과목이 추가된다면 기존의 노드에서 확장시켜준다.
   
   
   <img src = "https://user-images.githubusercontent.com/77683645/153731621-918814d6-dc4a-4bb5-bdec-78bb3ef260ac.png"><br><br>
   <img src = "https://user-images.githubusercontent.com/77683645/153731661-9e64bdff-affd-4105-8426-8a65367ce3b6.png"><br><br>
   - 위에서부터 데이터사이언스전공(9학점)이 필요하다면, 데이터사이언스 프로그래밍, 데이터통계분석, 데이터베이스기초 수업을 추천해준다.
   - 데이터사이언스전공(6학점), 소프트웨어전공(3학점)이 필요하다면 프로그래밍, 데이터통계분석, (C프로그래밍, 자료구조) 수업을 추천해준다.
   - 데이터사이언스전공(3학점), 소프트웨어전공(3학점)이 필요하다면 프로그래밍, (C프로그래밍, 자료구조) 수업을 추천해준다.

   이때 , 프로그래밍(프로그래밍1,2) , 데이터통계분석(데이터통계분석1,2), (C프로그래밍, 자료구조)는 프로그래밍 수업을 들은 적이 없다면 프로그래밍1을, 프로그래밍1을 수강한 적이 있다면 프로그래밍
   2를 추천해주는 방식으로 `선이수 과목`을 고려하여 힉생에 맞는 과목을 추천해주도록 한다.<br><br>
   
   <img src = "https://user-images.githubusercontent.com/77683645/153731793-649da9b9-ad1b-4c15-ba88-709fcb0ad4c6.png"><br>
   
   만일, 학생A가 프로그래밍1, 데이터통계분석1을 수강한 적이 있으며 현재 데이터사이언스전공(6학점), 소프트웨어전공(3학점)이 필요하다면 학생 A에게 프로그래밍2, 데이터통계분석2, C프로그래밍 과목    을 추천해준다.<br><br> 
   
6. 최종적으로 `졸업 필수학점` 고려하여 학생 A에게 필요한 과목을 추천해준다.


   <img src = "https://user-images.githubusercontent.com/77683645/153731915-d62e4000-a9c7-4cc5-b202-54a0b3f854ac.png"><br><br>
   학생 A가 `졸업 필수요건`인 계열교양 중 공학수학을 1학년 때 수강하지 않았더라면, 공학수학을 추가로 추천해주어 학생A가 `졸업 필수학점` 조건을 맞출 수 있도록 한다.<br><br>

   <img src = "https://user-images.githubusercontent.com/77683645/153731956-72e383bf-e024-4af5-8636-49ffc5c2e5e6.png"><br><br>
7. 위 1~6 과정을 학생A의 데이터사이언스, 소프트웨어 복수전공 뿐만 아니라 교내 재학생들의 상황에 맞게 진행하여 개개인에 맞는 과목 추천 시스템을 구축한다.<br><br>

<h2 id = "03">3. i - 로드맵 과목 추천시스템 기대효과</h2><br>

<img src = "https://user-images.githubusercontent.com/77683645/153732225-6f0ea7d2-f534-453d-997d-830d0219eebe.png"><br><br>
