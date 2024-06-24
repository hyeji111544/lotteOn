# LotteON 쇼핑몰 프로젝트
![slice](https://capsule-render.vercel.app/api?type=slice&color=auto&height=200&text=LotteOn&fontAlign=70&rotate=13&fontAlignY=25&desc=make%20Shoppingmall%20Project.&descAlign=60&descAlignY=44)

## 프로젝트 개요

| 항목 | 내용 |
| --- | --- |
| 프로젝트 소개 | 쇼핑몰의 기본 기능 개발을 목표로 실제 업무와 유사한 환경에서 설계 및 구현 |
| 개발 인원 | 총 4명 (프론트/백엔드 동시 작업) |
| 당담 역할 | ERD 구성 및, 상품 관련 기능 구현 |
| 개발 기간 | 총 33일 (2024-04-15 ~ 2024-05-17) |
| 성과 및 결과 | 기한 내 목표 기능 구현 완료, 서비스 테스트 완료. |

## 사용 기술

**Frontend** `HTML` `CSS` `JavaScript`

**Backend** `Spring Boot` `JPA` `QueryDSL` `MyBatis`

**Database** `MySQL`

**Deploy** `AWS (EC2, S3, CodeDeploy)`

**Version Control** `Git`

**CI/CD** `GitHub Actions`

## 프로젝트 구조
![Untitled](https://github.com/hyeji111544/lotteOn/assets/154953972/f31cabdb-1832-4bd0-b003-c662d549ddb2)


## 주요 기능

### 1. 메인페이지
![-Clipchamp33-ezgif com-video-to-gif-converter](https://github.com/hyeji111544/lotteOn/assets/154953972/5cfc2518-f8e8-4a2c-acb7-ef345fbec57c)
- 상품 카테고리 마우스 hover 시 1,2,3 차 카테고리 출력
- 히트, 추천, 최신, 인기, 할인 상품 페이지 출력
- 상단의 히트, 추천, 최신, 인기, 할인 상품 클릭 시 해당 위치로 이동

### 2. 회원
![-Clipchamp31-ezgif com-video-to-gif-converter](https://github.com/hyeji111544/lotteOn/assets/154953972/8de2f0d2-c652-4b30-93f4-c671e63248d7)
- 로그인, 자동 로그인, 아이디 기억하기 기능
- 회원가입 클릭 시 일반, 판매자 회원가입 구분
- 선택한 회원 종류에 따른 이용약관 출력
- 일반 회원가입 기본정보 입력 후 유효성 검사
- 판매자 회원가입 회사명, 대표자 명, 사업자 등록번호 등 입력 후 가입
- 아이디/비밀번호 찾기 가입시 입력한 이메일 사용하여 발송된 메일의 인증번호
기입 후 아이디 찾기, 비밀번호는 재설정한다.

### 3. 고객서비스 (CS)
![-Clipchamp32-ezgif com-video-to-gif-converter](https://github.com/hyeji111544/lotteOn/assets/154953972/eeb3b093-4ec4-41dc-a7df-2e541f5af0ee)
- 메인
    - 공지사항, 문의하기 최신글 출력, 자주하는 질문 카테고리 별 아이콘 출력
    문의글 작성 클릭 시 작성 화면 이동.
- 자주묻는 질문
    - 유형별로 3개씩 출력 하고 아코디언 설정하여 더보기 가능하게 함.
- 공지사항
    - 공지사항 메뉴 (전체, 고객서비스 등) 카테고리별로 출력함.
- 문의하기
    - 문의하기 메뉴 (회원, 배송 등) 카테고리 별로 출력 하며 문의하기글 작성 가능함.
    답변이 있는 경우 `답변완료` 답변이 없으면 `검토중` 출력
    - 문의글 작성 시 문의 유형에 따른 1,2차 카테고리 설정

### 4. 상품
![-Clipchamp34-ezgif com-video-to-gif-converter](https://github.com/hyeji111544/lotteOn/assets/154953972/96fb17fc-7a34-4adb-a77d-b9df96f3f1ae)

- 상품 목록
    - 1,2,3차 카테고리 별로 등록된 상품 조회
    - 판매 많은 순, 낮은 가격 순 등 선택한 조건대로 상품 정렬
    - 상품 정보 출력하며 무료배송 시 아이콘 출력
- 상품 검색
    - 상품명, 설명, 가격 으로 검색 중복으로 선택 가능.
    - 검색된 상품 내에서 판매많은순, 낮은가격순 등 정렬 가능.
- 상품 상세
    - 상품 정보 출력, 별점 및 상품평 보기
    - 장바구니 / 구매하기 / 찜하기 기능
- 장바구니
    - 상품 정보 출력 및 상품 체크 후 삭제, 수량 변경 및 선택한 항목만 구매가능
- 주문하기
    - 구매할 상품 정보 출력 및 로그인 된 유저 기본 정보 출력,
    수령자 정보 입력 가능 및 포인트 사용 가능.
    최종결제 정보 확인 가능.
- 주문완료
    - 주문된 상품 및 금액, 주문자와 입력된 배송 정보 확인가능
      
### 5. 마이페이지
![-Clipchamp31-ezgif com-video-to-gif-converter (1)](https://github.com/hyeji111544/lotteOn/assets/154953972/47efbf3b-a8c1-42a8-8068-7d9b7db5756a)

- 메인
    - 최근 주문내역, 포인트 적립내역, 상품평, 문의내역, 기본 정보 확인 가능
- 전체주문내역
    - 기간별 조회 및 수취확인, 상품평 작성, 반품신청, 제품 문의 가능
- 관심상품
    - 장바구니 담기, 관심상품 삭제, 해당 상품 페이지로 이동 가능
- 포인트 내역
    - 기간별 조회 가능
- 쿠폰
    - 보유 쿠폰 정보 확인 가능
- 나의 리뷰
    - 작성한 리뷰 확인 및 해당 상품으로 이동
- 문의하기
    - 작성한 고객문의, 상품 문의 답변 확인
- 나의 설정
    - 비밀번호, E-mail, 휴대폰, 주소 변경
  
### 6. 상점 관리(Seller)
- 메인
    - 쇼핑몰 총 운영 현황 출력(주문 건수, 주문 금액, 배송 관리, 주문관리)
    - 공지사항, 고객문의 확인 가능
- 상품관리
    - 상품 목록 : 본인이 등록한 상품 검색 조회 및 삭제, 수정 가능(+옵션설정)
    - 상품 등록 : 상품 등록 가능
- 주문관리
    - 주문 현황 : 한달 주문건수 출력 및 주문 상태(배송준비, 배송중) 에 따른 조회 가능
    - 매출 현황 : 일일 매출, 전체/일년/한달/일주일 에 따른 매출, 주문취소, 환불 조회
    - 배송 관리 : 배송현황, CS현황(취소, 환불, 교환 요청) 조회
- 고객센터
    - 공지사항 : 카테고리에 따른 조회 가능
    - 고객문의 : 본인이 등록한 상품에 대한 문의 조회 및 답변 등록, 수정, 삭제 가능
  
### 7. 관리자(admin)
- 메인
    - 쇼핑몰 총 운영 현황 출력(주문 건수, 주문 금액, 배송 관리, 주문관리)
    - 공지사항, 고객문의 확인 가능
- 환경설정
    - 기본 환경 정보 : 쇼핑몰 이용약관 수정 가능
    - 배너관리 : 배너 등록, 활성화 여부, 시작&종료 날짜 시간 조절 가능
- 상점관리
    - 가입한 모든 판매자 현황조회, 검색, 정보 열람 가능
- 회원관리
    - 회원 현황 :  가입한 모든 유저 현황 조회, 등급, 권한, 활동상태 수정 가능
    - 포인트 관리 : 유저 포인트 지급 및 회수 가능
- 상품관리
    - 상품 목록 : 사이트에 등록된 모든 상품 검색 조회 및 삭제 가능
    - 상품 등록 : 상품 등록 가능
- 주문관리
    - 주문 현황 : 한달 주문건수 출력 및 주문 상태(배송준비, 배송중) 에 따른 조회 가능
    - 매출 현황 : 일일 매출, 전체/일년/한달/일주일 에 따른 매출, 주문취소, 환불 조회
    - 배송 관리 : 배송현황, CS현황(취소, 환불, 교환 요청) 조회
- 고객센터
    - 공지사항 : 카테고리에 따른 조회 및 글 등록, 삭제, 수정
    - 자주묻는 질문 : 카테고리에 따른 조회 및 글 등록, 삭제, 수정
    - 문의하기 : 카테고리에 따른 조회 및 답변 등록, 삭제, 수정
      
### 8. 회사 소개(company)
- 메인, 기업문화, 소식과 이야기, 채용, 미디어 회사 소개 페이지

### 9. 이용 약관(terms)



## 프로젝트 버전 업데이트 내역
<details>
<summary>상세보기</summary>
0.0.1-SNAPSHOT / 24.04.15
 - 메인 화면 구현
 - 프로젝트 페이지 CSS 디자인 작업

0.0.2-SNAPSHOT / 24.04.16
 - 회원 가입 기능 추가
 - 상품 등록 기능 추가

0.0.3-SNAPSHOT / 24.04.17
 - 카테고리 분류 기능 추가
 - 회원 가입 유효성 검사 추가
 - 고객센터 글 등록, 수정 기능 추가

0.0.4-SNAPSHOT / 24.04.18
 - 판매자 회원가입 기능 추가
 - 고객센터 글 삭제, 목록 보기 추가
 - 상품 옵션 등록 기능 추가

0.0.5-SNAPSHOT / 24.04.19
 - 메인 화면 상품 출력 추가
 - 마이페이지 기능 추가

0.0.6-SNAPSHOT / 24.04.22
 - 장바구니 상품 목록 출력
 - 마이페이지 쿠폰 목록 출력

0.0.7-SNAPSHOT / 24.04.23
 - 마이페이지 주문 목록 출력
 - 장바구니 수량 변경시 가격 변동 로직

0.0.8-SNAPSHOT / 24.04.24
 - 판매자 관리 화면 상품 목록 출력
 - 마이페이지 포인트 내역 출력

0.0.9-SNAPSHOT / 24.04.25
 - 장바구니 기능 구현 완료
 - 판매자 관리 화면 답변 등록, 수정, 삭제 완료
 - 고객정보 페이지 완료

0.1.0-SNAPSHOT / 24.04.26
 - 아이디 찾기 기능 구현
 - 3차 카테고리를 통한 상품 등록 기능 추가
 - 고객센터 검색기능 추가

0.1.1-SNAPSHOT / 24.04.29
 - 비밀번호 찾기 기능 구현

0.1.2-SNAPSHOT / 24.04.30
 - 회원정보 수정 기능 추가
 - 주문내역, 포인트 내역 조회 검색기능 추가

0.1.3-SNAPSHOT / 24.05.01
 - 회사소개 페이지 추가
 - 주문하기 기능 구현

0.1.4-SNAPSHOT / 24.05.02
 - 배너 이미지 등록 기능 추가
 - 판매자 정보 수정 기능 추가
 - 회사소개/소식과 이야기 페이지 추가

0.1.5-SNAPSHOT / 24.05.03
 - 아이디 저장 / 자동로그인 기능 추가

0.1.6-SNAPSHOT / 24.05.07
 - 관리자 주문현황 기능 구현
 - 관리자 배송관리 기능 구현

0.1.7-SNAPSHOT / 24.05.08
 - 마이페이지 리뷰작성 기능 추가
 - 관리자 매출현황 기능 구현
 - 배너 이미지 관리 기능 구현

0.1.8-SNAPSHOT / 24.05.09
 - 상품 문의하기 작성 기능 추가
 - 배너 이미지 출력 기능 구현

0.1.9-SNAPSHOT / 24.05.10
 - 상품 정보 수정 기능 추가
 - 상품 검색 페이지 추가

1.0.0-RC / 24.05.13
 - 상품 개별 삭제 기능 추가

1.0.1-RC / 24.05.14
 - 마이페이지 주문내역 관리 기능 추가

1.0.2-RC / 24.05.16
 - 최종 점검

1.0.0-RELEASE / 24.05.17
 - 최종 배포

</details>
