---
layout: post
title: 'Styled Components'
categories: react
tags: react
comments: true
---


## styled components

### 설치 및 적용

터미널에 npm install styled-components 를 입력해줍니다.

~~~javascript
import styled from 'styled-components';
~~~
그리고 사용하고 싶은 파일에 import를 해줍니다.
그러면 세팅 끝 


### 사용법
**App.js**
~~~javascript
import React from "react";
import styled from "styled-components";

let Box = styled.div`
  padding: 10px;
  color: grey;
`;

let YellowBtn = styled.button`
  background: lightyellow;
  color: black;
  padding: 100px;
`;

const App = () => (
  <div>
    <Box>
      <YellowBtn />
    </Box>
  </div>
);

export default App;
~~~
만약 <div>에 css를 적용하고 싶으면 styled.div뒤에 ``(따옴표 아니고 backtick 기호임)을 붙이고 이 안에 적용하고 싶은 css 적으면 됩니다. button에 css를 적용하고 싶으면 styled.button 

<img src = "../../image/styled-components 1.png" width = 80%/>
콘솔창에 npm start를 입력해주면 위와 같은 사각형이 생깁니다.



