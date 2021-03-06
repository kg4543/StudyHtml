# CSS 기본학습
CSS를 활용한 기본 구조 및 스타일링 지정

-----------------------
## 1. 기본 선택자

* 선택자{스타일 속성: 스타일 값;}
  - 전체 선택자: *로 표기
  - 태그 선택자: 태그 그래도 표기
  - 아이디 선택자: '#id' 형태로 표기
  - 클래스 선택자: '.class' 형태로 표기
  - 자손 선택자: 선택자 > 선택자
  - 후손 선택자: 선택자 선택자

### 구현 및 코드
<kbd>![selector_id](/02_CSS/CSS_실행화면/selector_id_test.PNG "기본선택자")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_id_test.html)

-----------------------
## 2. 반응/상태 선택자

* 반응선택자
  - :active : 마우스로 클릭 시 이벤트 발생
  - :hover : 마우스 커서가 올라가면 이벤트 발생

* 상태선택자(input 태그에 사용)
  - :checked: check 상태의 input 태그 선택
  - :focus: 현재 focus 상태의 input 태그 선택
  - :enabled: 사용가능한 상태의 input 태그 선택
  - disabled: 사용불가능 상태의 input 태그 선택

### 구현 및 코드
<kbd>![selector_child](/02_CSS/CSS_실행화면/selector_child_test.PNG "반응&상태")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_child_test.html)

-------------------------
## 3. 구조 선택자

* :first-child: 형제 관계에서 첫번째
* :last-child: 형제 관계에서 마지막
* :nth-child(n): 형제관계에서 'n-1'번째
* :nth-last-child(n): 형제관계에서 거꾸로 'n-1'번째    

### 구현 및 코드
<kbd>![selector_struct](/02_CSS/CSS_실행화면/selector_struct_test.PNG "구조")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/selector_struct_test.html)

-----------------------------
 ## 4. 박스속성

<kbd>![Box_attr](/02_CSS/images/박스속성.PNG "박스속성")</kbd>

### 구현 및 코드
<kbd>![selector_struct](/02_CSS/CSS_실행화면/box_test.PNG "box_test")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/box_test.html)

-----------------------------
## 5. 가시 속성

* display: @
  - none: 화면에 보이지 않음
  - block: 하나의 상자와 같은 block형식으로 표시
  - inline: 인라인(가로열거)형식으로 표시
  - inline-block: 인라인 형식으로 열거되면 내부는 block처럼 표시

------------------------------
## 6. 배경 속성

* background-image: url('#'): 배경 이미지 삽입
* background-size: 배경이미지 사이즈 지정
* background-repeat: @
  - initial: 기본값 설정
  - repeat: 가로,세로 전체 반복
  - no-repeat: 반복 안 함
  - repeat-x: 가로줄 반복
  - repeat-y: 세로줄 반복
  - inherit: 부모의 속성값으로 설정

* background-attachment: @
  - initial: 기본값 설정
  - Scroll: 스크롤따라 배경이미지가 같이 움직임
  - fixed: 배경이미지 고정
  - inherit: 부모의 속성값으로 설정

* background-position: 배경이미지 위치 지정
* background { }: 여러 속성 입력

### 구현 및 코드
<kbd>![background_test](/02_CSS/CSS_실행화면/background_test.PNG "background_test")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/background_test.html)

--------------------------------
## 7. 글자 속성

* font-size: 글자 크기 지정
* font-family: 글꼴 지정
* text-align: 글자 정렬

### 구현 및 코드
<kbd>![text_test](/02_CSS/CSS_실행화면/text_test.PNG "text_test")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/text_test.html)

--------------------------------
## 8. 위치 속성

* position: @
  - absolute: 절대 위치로서 부모를 기준으로 위치 지정 (부모가 위치 지정이 되어 있지 않을 경우 'body'로 위치 기준이 잡힘)
  - fixed: 스크롤이 내려가도 지정된 위치에 고정
  - relative: 자신의 static 상태 기준(초기 위치)에서 위치 지정
  - stacic: 기본위치

* overflow: @
  - hidden: 영역에서 벗어나는 부분을 감춤
  - scroll: 영역을 벗어나는 부분을 스크롤로 만듦

### 구현 및 코드
<kbd>![position_overflow](/02_CSS/CSS_실행화면/posiont_overflow_test.PNG "position_overflow_test")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/position2_test.html)

----------------------------------
## 9. 유동 속성

* float: 웹 브라우저 크기와 상관없이 일정한 위치에 요소를 고정시킴

### 구현 및 코드
<kbd>![float_test](/02_CSS/CSS_실행화면/float_test.PNG "float_test")</kbd>

[코드보기1](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/float_test.html) <br>
[코드보기2](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/layout1_test.html)

-----------------------------------
## 10. 레이아웃의 구성 및 기능

<kbd>![one_true](/02_CSS/CSS_실행화면/onetrue.PNG "one_true")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/layout_onetrue.html)

```
.ellipsis{
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }
```
 * text-overflow: ellipsis: Text가 길 경우 뒷부분 생략처리
 
 -----------------------------------
## 반응형 웹
<kbd>![responsive_web](/02_CSS/CSS_실행화면/responsive_web.PNG "responsive_web")</kbd>
<kbd>![responsive_web2](/02_CSS/CSS_실행화면/responsive_web2.PNG "responsive_web2")</kbd>

[코드보기](https://github.com/kg4543/StudyHtml/blob/main/02_CSS/responsive_test.html)<br>
[Javascript 상세](https://github.com/kg4543/StudyHtml/tree/main/03_JavaScript)

-----------------------------------
## 본문으로

[이전](https://github.com/kg4543/StudyHtml)

