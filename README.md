

<div align="center">
    <img src="https://github.com/whl5105/Team-adEarth-client-v2.0/assets/73993670/cb51ea0a-8a63-4735-a831-dc3c14ce9549" width="1000"/>
    <br />
    <h2> CPC 키워드 광고를 적용한 이커머스 플랫폼
      <img src="https://github.com/whl5105/Team-adEarth-client-v2.0/assets/73993670/8deb8b8f-54dc-4ffc-abfb-45954fc0850f" width="25" height="25"/>
    </h2>
    <p>
        광고지구 프로젝트는 소비자와 판매자를 위한 이커머스 환경을 구현하고, <br /> 디지털 마케팅 툴을 활용해 효과적인 이커머스 웹 플랫폼을 기획해보자는 의견에서 출발하였습니다. <br />
    </p>
    <p>
        <a href="https://adearth.shop" target="_blank">사이트 보러가기(id: testuser / password: aaa1111!)</a> 
        <br/>
        <span>현재 해당사이트는 운영중이지 않습니다.</a>
    </p>

</div>


## 이커머스 플랫폼(구매자) | 지구샵
1. 실제 이커머스와 동일한 쇼핑 경험을 할 수 있어요.
2. 검색 창에 원하는 상품이나 키워드를 입력하면 키워드 광고가 등록된 상품을 순위별로 확인할 수 있어요.
3. 마이페이지에서 주문 상품에 대한 정보를 상세하게 확인하고 관리할 수 있어요.


<br/>

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
### 회원가입 및 로그인
<kbd>
<img alt="회원가입 및 로그인" 
  src="https://user-images.githubusercontent.com/105091138/231611197-778c05c4-ffc0-4099-b21e-861bcf7a8add.gif" />    
</kbd>


[회원가입]
- 가입할 때는 필수 정보를 모두 기입하고 검증을 거쳐야 가입할 수 있어요.
- 기본 프로필 이미지를 제공하며, 원하는 이미지로도 등록할 수 있어요.
- 아이디, 비밀번호는 실시간으로 유효성 검사를 하며, 주소는 다음 API를 이용해 간편히 검색할 수 있어요.
- 가입에 성공하면 상단의 토스트 메세지로 확인할 수 있어요.

[로그인& 아이디/비밀번호 찾기]
- 로그인에 성공하면 메인페이지로 넘어가요.
- 로그인에 실패하면 상단의 토스트 메세지로 로그인 실패의 이유를 확인할 수 있어요.
- 아이디가 기억나지 않을 때는 가입할 때 입력한 개인정보를 통해 간편하게 아이디를 찾을 수 있어요.
- 비밀번호가 기억나지 않을 때는 가입할 때 입력한 개인정보로 인증한 후 새로운 비밀번호로 변경할 수 있어요.

<br/>

### 메인
<kbd >
<img alt="메인"
src="https://user-images.githubusercontent.com/105091138/231608589-842124e8-0c00-4100-926e-70fad42525f4.gif"/>
</kbd>

- 메인 홈 상단에는 상품의 홍보 배너를 슬라이드 형태로 제공해요.
- 누적 판매량이 6순위에 드는 베스트 상품을 구경할 수 있어요.
- 새롭게 등록된 상품 9개의 신 상품을 구경할 수 있어요.

<br/>

### 상품 목록 
<kbd>
<img alt="상품 목록" 
  src="https://user-images.githubusercontent.com/105091138/231609516-ad1f46ae-e9b5-4fd4-b7cd-1f77bafb7cba.gif" />
</kbd>

- 상단의 네비게이션 바의 장보기 버튼으로 커서를 옮기면 상품 카테고리를 드롭다운 메뉴로 확인할 수 있고, 클릭하면 상품 카테고리별로 상품 목록을 구경할 수 있어요.
- 상품 목록은 인기순, 등록순으로 정렬할 수 있어요.
- 상품마다 리뷰와 좋아요 개수를 확인할 수 있고, 마음에 드는 상품은 ‘좋아요’를 클릭해두고 마이페이지에서 확인도 가능해요.
- 신 상품이나 세일 상품은 상품에 붙은 배지로 확인하기가 쉬워요.
  
<br />

### 상품 검색 목록
<kbd>
<img alt="상품 검색 목록" 
  src="https://user-images.githubusercontent.com/105091138/232265920-aca2f3ce-4dcd-418f-9ff8-5a47a8ed165b.gif" />
</kbd>

- 상단의 네비게이션 바의 검색 창에 원하는 상품이나 키워드를 입력하면 검색 결과 페이지로 넘어가요.
- 검색 결과 중 광고 키워드가 등록된 상품은 광고 배지가 붙어 있고, 입찰 순위대로 상품 목록을 확인할 수 있어요.

<br/>

### 상품 상세
<kbd>
<img alt="상품 상세" 
  src="https://user-images.githubusercontent.com/105091138/231612055-86e68d3a-7c1e-4a59-9ce3-dbbcf5c8a732.gif" />
</kbd>
  
- 상품에 대한 상세 정보와 다른 고객이 등록한 리뷰를 확인할 수 있어요.
- 상품의 옵션이나 수량을 설정한 후 상품을 구매하거나 장바구니에 담아둘 수 있어요.(단, 상품 수량이나 옵션이 선택되지 않은 상태에서는 구매나 장바구니 담아두기가 불가능해요.)
- 상품이 마음에 들면 좋아요를 선택하고 마이페이지에서 확인할 수 있어요

<br />

### 장바구니
<kbd>
<img alt="장바구니" 
  src="https://user-images.githubusercontent.com/105091138/231612433-1660c955-10fe-4fba-a3ba-6cdb6657867f.gif" />
</kbd>

- 장바구니에 담긴 상품의 수량을 변경하거나 옵션을 수정할 수 있어요.
- 원하지 않은 상품은 선택해서 장바구니에서 삭제할 수 있어요.
- 상품 개별 주문을 할 수 있고, 여러 상품을 선택해 총 주문 금액을 바로 확인하고 주문할 수도 있어요.

<br />

### 결제
<kbd>
<img alt="결제" 
  src="https://user-images.githubusercontent.com/105091138/231612934-9036cd3e-749b-44bf-bc23-8874ccfd9e85.gif" >
</kbd>

- 결제할 상품의 정보와 총 주문 금액, 배송지 정보, 결제 수단 등을 확인할 수 있어요.
- 배송정보는 기본 배송지, 이전에 주문했던 배송지, 신규 배송지 중 선택해서 이용할 수 있어요.
- 결제에 필요한 정보를 모두 입력하고, 전체 동의 후 결제하기 버튼을 누르면 상단의 토스트 메세지와 함께 결제 완료 페이지로 넘어가요.

<br />

###  결제 제품 주문배송 확인 및 취소 
<kbd>
<img alt="결제 제품 주문배송 확인 및 취소 " 
  src="https://user-images.githubusercontent.com/105091138/231613382-c3bc49c9-290d-49e4-b65f-6bac2fc31fc0.gif"/>
</kbd>

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
<kbd>
<img alt="위시리스트" 
  src="https://user-images.githubusercontent.com/105091138/231614054-bff7551b-041c-4431-a4d9-545c3fb481f0.gif"/>
</kbd>

- 상품을 둘러보며 좋아요한 상품을 한눈에 확인할 수 있어요.
- 위시리스트 삭제가 바로 가능해요.
- 상품 선택시 상품 상세페이지를 확인할 수 있어요.
- 상단에 좋아요를 누른 상품의 총 갯수를 바로 확인할 수 있어요.

<br />

### 주문취소 확인
<kbd>
<img alt="주문취소 확인" 
  src="https://user-images.githubusercontent.com/105091138/231614032-d5718ac4-e047-483c-9742-d61dfda084ef.gif" />
</kbd>

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
![광고지구아키텍쳐](https://github.com/ad-earth/client-v2.0/assets/101298873/2d7b7c91-474f-4d97-876d-ac524f880326)

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



