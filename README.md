# 한화시스템 beyond sw캠프 1기 [Delivery-active]
배달어플 데이터베이스 설계 프로젝트

## 🖥 프로젝트 소개
우리가 요즘 가장 많이 사용하는 어플인 배달의 민족의 데이터베이스를 설계해 보았습니다.

## 📅 프로젝트 기간
23.11.16 - 23.11.17

## 👨‍👦‍👦 멤버 구성
- 이동혁 (조장)
- 이영진
- 윤채영
- 주현성

## 프로젝트 구현
#### 1. 요구사항 분석 (※제한된 기간내에 구현 가능한 요구사항 추출)
- 사용자
    * 회원가입을 할 수 있다.
    * 회원가입 시 아이디,패스워드,이름,핸드폰번호,주소를 입력한다.
    * 고객은 회원정보 변경이 가능하다.
    * 고객은 배달 메뉴를 선택해 주문 할 수 있다.
    * 고객은 배달 주소를 변경가능하다.
    * 고객은 메뉴 검색, 매장 이름 검색을 통해 매장 검색이 가능하다. 
- 매장
    * 매장 등록을 할 수 있다.
    * 매장 등록 시 이름,  전화번호,  주소, 사업자 번호,  가게소개, 최소주문금액, 안내 및 혜택, 운영 시간, 주문 타입, 원산지 정보를입력하면 매장 번호가 부여된다.
    * 매장은 메뉴를 넣고 빼고 수정할 수있다.
    * 매장은 주문내역을 확인할 수 있다.
    * 매장은 매장 정보를 수정할 수 있다.
    * 매장은 영업 상태를 수정 할 수있다.
    * 매장은 주문한 회원의 주소, 전화번호, 주문메뉴를 확인할 수 있다.
    * 매장은 주문 상태를 주문 승인으로 변경할 수 있다.
    * 매장은 주문의 도착 예정 시간을 수정할 수 있다.
- 배달기사
    * 회원가입을 할 수 있다.
    * 회원가입 시 패스워드, 이름, 전화번호를 입력한다.
    * 배달원은 배달 요청 내역을 조회할 수 있다.
    * 배달원은 본인 상태를 등록할 수 있다.
    * 배달원은 본인 상태를 수정할 수 있다.
    * 배달원은 주문 상태를 배달중과 배달완료로 수정할 수 있다.
    * 배달원은 주문의 도착 시간을 수정할  수 있다.


#### 2.  USECASE 다이어그램
   
   ![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/51053337-bb0a-4343-a1bd-92a802364a1b)

#### 3. 개념적 데이터 모델링


![KakaoTalk_20231117_124854860](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/7e7f89fe-4e9b-46d9-b489-b1ce0af3024f)

#### 4. 논리적 데이터 모델링

 ![Untitled](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/e2fb6e68-ca88-4261-a06a-89223bb4be23)

#### 5. 테이블 생성 및 데이터 넣기

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/6e7b49f5-21bd-4738-ad73-a7e2e195cb08)

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/9c821f0d-a66c-4aaa-9c74-ae6779cef76e)

#### 6. 테이블을 활용하여 실제로 데이터 검색해보기

1. 해당가게에 주문한 회원의 배달주소/전화번호/주문메뉴 확인
   1번가게에 주문한 주문정보 확인

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/8d684bc3-d4e4-4707-b1c4-e7c7ae057b05)

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/d0ddf7ef-92cd-4520-9d45-f42c087f4df4)

2.  배달 매장 정보 조회
냠냠분식 매장정보 조회

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/49fd31a8-4b0b-4b71-95d7-07b970b22130)

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/ef9ffa73-fe7a-4b55-92e7-5ebd6007e9d7)

3. 라이더 본인 배달  내역 조회
5번 라이더 배달내역 조회

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/fe27c0bd-e603-406a-9467-6f29aca8aaa5)

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/7972c70b-38c4-4117-95a3-93122ea6308f)

4. 고객이 주문한 내역 확인
3번 회원 배달내역 조회

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/2a419409-0250-4b7b-9e6b-4bf4b188db88)

![image](https://github.com/beyond-sw-camp/be01-1st-2Team-delivery-active/assets/73848116/eaafcc05-a732-4901-8ed7-33dc32a06cb5)












