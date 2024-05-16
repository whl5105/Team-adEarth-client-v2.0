

<div align="center">
    <img src="https://github.com/whl5105/Team-adEarth-client-v2.0/assets/73993670/cb51ea0a-8a63-4735-a831-dc3c14ce9549" width="1000"/>
    <br />
    <h2> CPC 키워드 광고를 적용한 이커머스 플랫폼
      <img src="https://github.com/whl5105/Team-adEarth-client-v2.0/assets/73993670/8deb8b8f-54dc-4ffc-abfb-45954fc0850f" width="25" height="25"/>
    </h2>
    <p>
        ‘기존 키워드 클릭 광고주 페이지의 문제점들을 개선해<br />
        광고 입찰에 꼭 필요한 기능들만 선별해 사용자의 경험을 개선해 보았어요. <br />
    </p>
    <p>
        <a href="[https://zellodraw.com](https://adearth.shop)" target="_blank">사이트 보러가기(id: testuser / password: aaa1111!)</a> 
        <br/>
        <span>현재 해당사이트는 운영중이지 않습니다.</a>
    </p>

</div>

## 프로젝트 소개

## 기술적 도전
#### 기능적 개선
- 에러 및 알림 메시지를 공통 Toast UI로 처리하여 인터페이스의 일관성 유지
- Skeleton UI를 적용해 유저 반응성 향상
- 유저 편의성을 고려해 회원가입 시, 기본 프로필 이미지 제공
- React-router-dom의 ScrollRestoration 컴포넌트를 사용한 scroll top 처리로 사용성 개선
- 정렬과 페이지 처리를 query string으로 변경하여 뒤로 가기 시에도 유저가 선택한 필터가 유지되도록 개선

#### 기술적 개선
- 동일한 QueryKey로 받아온 데이터를 custom hook으로 모듈화해 데이터 관리와 유지보수가 용이하도록 개선
- 폴더 구조를 개선하고 컴포넌트를 모듈화하여 재사용성을 높임
- Axios Response Type을 미리 지정해 데이터 타입 사전 체크
- 유저 권한 속성을 추가한 라우터 정보를 목록화하고 선택적 렌더링을 적용해 유저 권한별 접근이 제어되는 웹으로 개선
- 이미지를 lazy loading 하고 압축률이 높은 이미지 형식(WebP)으로 변환하여 웹 성능을 최적화
- 상품 목록 정렬과 pagination의 페이지 처리를 state에서 query string으로 변경
- React Portal을 사용해 독립적인 Modal DOM 선언

<br/>

## 페이지 주요 기능
### 회원가입 및 로그인 페이지 
<img alt="회원가입 및 로그인 페이지" 
  src="https://user-images.githubusercontent.com/105091138/231611197-778c05c4-ffc0-4099-b21e-861bcf7a8add.gif" />
▪︎ 아이디 & 비밀번호 & 연락처 중복검사, 실시간 유효성 검사 <br /> ▪︎ 아이디 & 비밀번호 찾기

<br/>

### 메인 페이지 
<img alt="메인 페이지"
src="https://user-images.githubusercontent.com/105091138/231608589-842124e8-0c00-4100-926e-70fad42525f4.gif"/>
▪︎ BEST 상품(누적 판매량 6위 이내의 6개 상품) 확인 <br /> ▪︎ NEW 상품(최신 등록 순 9개 상품) 확인

<br/>

 ### 상품 목록 페이지 
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231609516-ad1f46ae-e9b5-4fd4-b7cd-1f77bafb7cba.gif" />
▪︎ 카테고리 별 상품 조회 <br /> ▪︎ 상품 목록 등록순, 인기순 정렬 <br /> ▪︎ 관심 상품 등록 

### 광고 검색 목록 페이지 
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/232265920-aca2f3ce-4dcd-418f-9ff8-5a47a8ed165b.gif" />
▪︎ 키워드 검색 시, 광고 키워드로 등록된 상품 확인 <br /> ▪︎ 광고 상품과 일반 상품을 구분하여 제공 <br /> ▪︎ 관심 상품 등록

<br/>

### 상품 상세 페이지 
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231612055-86e68d3a-7c1e-4a59-9ce3-dbbcf5c8a732.gif" />
▪︎ 상품 상세 정보 제공 <br /> ▪︎ 관심 상품 등록  <br /> ▪︎ 구매평 확인 및 삭제

<br />

### 장바구니 페이지 
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231612433-1660c955-10fe-4fba-a3ba-6cdb6657867f.gif" />
▪︎ 장바구니 상품과 옵션 정보 제공 <br /> ▪︎ 상품별 옵션과 수량 수정 및 삭제  <br /> ▪︎ 전체 & 선택 상품 구매 및 삭제

<br />

### 결제 페이지  
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231612934-9036cd3e-749b-44bf-bc23-8874ccfd9e85.gif" >
▪︎ 결제 상품 정보 제공 <br /> ▪︎ 기본 정보(배송지, 이름, 연락처) 제공 <br /> ▪︎ 이전 배송지 목록 선택 & 신규 배송지 추가 

<br />

###  결제 제품 주문배송 확인 및 취소 
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231613382-c3bc49c9-290d-49e4-b65f-6bac2fc31fc0.gif"/>

[주문조회]
- 사용자가 주문한 정보를 간편하게 확인할 수 있어요
- 주문한 상품을 클릭하면 배송지 정보와 결제금액이 확인가능해요.
- 주문한 상품의 배송상태를(주문완료, 주문확인,배송중,배송완료) 바로 확인 할 수 있어요.

[주문취소]
- 배송 출발전 제품이라면 주문취소가 가능해요.
- 여러개상품을 주문했다면 개별로 주문삭제가 가능해요.
- 주문취소시 실시간으로 환불금액을 확인할 수 있어요
- 주문취소가 접수되면 토스트 메세지로 알려줘요.

<br />
  
###  위시리스트
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231614054-bff7551b-041c-4431-a4d9-545c3fb481f0.gif"/>

- 상품을 둘러보며 좋아요한 상품을 한눈에 확인할 수 있어요.
- 위시리스트 삭제가 바로 가능해요.
- 상품 선택시 상품 상세페이지를 확인할 수 있어요.
- 상단에 좋아요를 누른 상품의 총 갯수를 바로 확인할 수 있어요.

<br />

### 주문취소 확인
<img alt="" 
  src="https://user-images.githubusercontent.com/105091138/231614032-d5718ac4-e047-483c-9742-d61dfda084ef.gif" />

- 주문취소한 내역을 한번에 확인할수 있어요.
- 취소상품의 상세내역에서 주문했던내역과 취소내역을 함께 확인할 수 있어요.

<br/>

## 기술 스택
<table>
    <thead>
        <tr>
          <td align="center"><b>분류</b></td>
          <td align="center"><b>스택</br></td>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td align="center"><b>FrontEnd</b></td>
            <td>
                <img src="https://img.shields.io/badge/React-18.2.0-61DAFB?logo=react&logoColor=white&color=5C5C5C&labelColor=61DAFB"/>
                <img src="https://img.shields.io/badge/TypeScript-4.9.5-3178C6?logo=typescript&logoColor=white&color=5C5C5C&labelColor=3178C6"/>	
                <img src="https://img.shields.io/badge/React Query-3.39.3-FF4154?logo=ReactQuery&logoColor=white&color=5C5C5C&labelColor=FF4154"/>	
                <img src="https://img.shields.io/badge/reduxTk -8.0.5-764ABC?logo=redux&logoColor=white&color=5C5C5C&labelColor=764ABC"/>	
                <img src="https://img.shields.io/badge/Styled Components-5.3.6-DB7093?logo=styledComponents&logoColor=white&color=5C5C5C&labelColor=DB7093"/>	
            </td>
        </tr>
        <tr>
            <td align="center"><b>BackEnd</b></td>
            <td>
                <img src="https://img.shields.io/badge/javascript-F7DF1E?logo=javascript&logoColor=white"/>
                <img src="https://img.shields.io/badge/nodedotjs-5FA04E?logo=nodedotjs&logoColor=white"/> 
                <img src="https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white"/>
                <img src="https://img.shields.io/badge/expressJs-000000?logo=express&logoColor=white"/>		
            </td>
         </tr>
         <tr>
             <td align="center"><b>Infra</b></td>
             <td>
                 <img src="https://img.shields.io/badge/Github_Action-2088FF?logo=githubactions&logoColor=white"/> 
                 <img src="https://img.shields.io/badge/amazonec2-FF9900?logo=amazonec2&logoColor=white"/> 
                 <img src="https://img.shields.io/badge/amazons3-569A31?logo=amazons3&logoColor=white"/> 
                 <img src="https://img.shields.io/badge/amazonroute53-8C4FFF?logo=amazonroute53&logoColor=white"/>
             </td>
        </tr>
        <tr>
            <td align="center"><b>Collaboration</b></td>
            <td>
              <img src="https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white"/>
              <img src="https://img.shields.io/badge/Notion-000000?logo=Notion"> 
              <img src="https://img.shields.io/badge/Figma-F24E1E?logo=Figma&logoColor=ffffff"> 
              <img src="https://img.shields.io/badge/Discord-5865F2?logo=Discord&logoColor=ffffff">
            </td>
        </tr>
    </tbody>
</table>


<br/>

## 아키텍처 구조도 
![광고지구아키텍쳐](https://user-images.githubusercontent.com/105091138/195766564-08299428-e979-49f0-97c8-7a130a7b106c.jpeg)

<br/>

## Git Flow 
![gitFlow](https://github.com/whl5105/Team-adEarth-client-v2.0/assets/73993670/3ab09e53-9618-4184-bef5-73eba7b45740)


- master : 제품으로 출시될 수 있는 브랜치
- hotfix : 출시 버전에서 발생한 버그를 수정 하는 브랜치
- develop : 다음 출시 버전을 개발하는 브랜치
- feature : 기능을 개발하는 브랜치
- refactoring develop  : 코드 리팩토링 작업을 수행하는 브랜치
- refactoring feature  : 리팩토링 과정에서 해당 기능에 수행하는 브랜치  

<br/>

## Development Setup

```bash

# Move to your workspace
cd your-workspace

# Clone this repository:
$ git clone https://github.com/whl5105/Team-adEarth-client-v2.0.git

# Enter in directory:
$ cd Team-adEarth-client-v2.0

# Install dependencies:
$ yarn install

# Run the development server:
$ yarn start

# Open the project in your browser
$ http://localhost:3000
```

<br/>

## Team Members
  <table>
  <tr>
      <td align="center">FrontEnd</td>
      <td align="center">FrontEnd</td>
      <td align="center">FrontEnd</td>
      <td align="center">BackEnd</td>
    </tr>
    <tr>
      <td align="center"><img src="https://github.com/whl5105.png" width="160"></td>
      <td align="center"><img src="https://github.com/damiiya.png" width="160"></td>
      <td align="center"><img src="https://github.com/sol-pine.png" width="160"></td>
      <td align="center"><img src="https://github.com/huitopia.png" width="160"></td>
    </tr>
    <tr>
      <td align="center">최수인</td>
      <td align="center">이담</td>
      <td align="center">해솔</td>
      <td align="center">김다희</td>
    </tr>
    <tr>
      <td align="center"><a href="https://github.com/whl5105" target="_blank">@whl5105</a></td>
      <td align="center"><a href="https://github.com/damiiya" target="_blank" width="160">@damiiya</a></td>
      <td align="center"><a href="https://github.com/sol-pine" target="_blank">@sol-pine</a></td>
      <td align="center"><a href="https://github.com/huitopia" target="_blank">@huitopia</a></td>
    </tr>
  </table>



