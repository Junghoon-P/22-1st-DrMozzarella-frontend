# 🧀 ***Dr. Mozzarella***

### 개발 기간 : 2021년 7월 5일 ~ 7월 16일

### 개발 인원 : 프론트엔드 3인, 백엔드 3인

### 사용 기술
    
    Front-End : React, SCSS
    
    Back-End : Python, Django
    

## 프로젝트 영상
    
   - [Dr.Jart Clone Project / 닥터 자르트 클론 프로젝트](https://youtu.be/lqHxD3Zq770)
    
약 2주간 Dr.Jart를 모티브로 Dr. Mozzarella 사이트를 제작했습니다.
세계 각국의 치즈를 판매하는 컨셉의 사이트로 기획하였습니다.
프론트엔드로 프로젝트에 참여해 **공용 컴포넌트, 메인페이지를** 구현했습니다.

***

### 개발과정
   - React Class Components 를 사용하여 각 컴포넌트들을 제작했습니다.
   - SASS를 활용한 Style 적용을 하였습니다.
    
### Pages
    
   - 메인페이지
        
        ![ezgif com-video-to-gif-2](https://user-images.githubusercontent.com/77766769/146684997-1d233f9e-81ab-4f29-a55d-d97569cb5ccc.gif)
        
        라이브러리를 사용하지 않고, 캐러셀을 구현했습니다.
        
        ![Jul-19-2021_02-03-49](https://user-images.githubusercontent.com/77766769/146685006-453a8a8d-f392-40bd-a9a5-ed5d90a5a5ee.gif)

        
        치즈를 구매할때 선택할 옵션이 있는 경우 드롭다운 형식으로 선택창이 추가되도록 카드 컴포넌트를 구현했습니다.
        
        ![Sep-03-2021_23-20-33](https://user-images.githubusercontent.com/77766769/146685015-e11286f6-0da9-47ca-96c7-11a39c363d3c.gif)

        
        Nav에서 드롭다운시 나오는 카테고리를 선택하게 되면 해당 페이지로 동적라우팅을 통해 이동하도록 구현했습니다.
### 기억에 남는 코드
    
```jsx
    //ex
    handleClickPrev() {            //지양
    
    handleClickPrev = () => {.     //권장
```
    
   - 이벤트에 콜백 함수로 넘겼을 때 this가 동적으로 바뀌면서 문제가 될 수 있습니다.
        따라서 class 컴포넌트에서는 가급적 화살표 함수로 써주는걸 권장합니다.
        +@ 바인드와 같은 원리라 .bind()를 써주는 것도 가능하지만 굳이 쓸 이유는 없습니다.
        
    
```jsx
    <i className="fas fa-chevron-left fa-4x" 
    		onClick={() => this.handleClickPrev()} />
                  
    <i className="fas fa-chevron-left fa-4x"
        onClick={this.handleClickPrev} />
```
    
   - 새로 함수 인스턴스를 만들지 않고 함수를 직접 넘겨주는 것이 좋습니다.
    - 해당 부분이 실행될 때마다 기존에 **생성해놓은 함수를 호출** 하는것이 아니라 **새로운 함수를 생성해서 실행하는 방식** 이라서 비효율적이라고 할 수 있습니다.


**🧀 [프로젝트 후기 Velog 링크](https://velog.io/@park_kyo_su/Project-1-Clone-Dr.Jart)**

***
     
#### Reference
이 프로젝트는 화장품 회사 Dr.Jart 사이트를 참조하여 학습 목적으로 만들었습니다.
실무수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
