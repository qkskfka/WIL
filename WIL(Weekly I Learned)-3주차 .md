# WIL(Weekly I Learned)-3주차

## Hooks

리액트에서 Hooks는 v16.8 에 새로 도입된 기능으로 함수형 컴포넌트에서도 상태 관리를 할 수 있는 useState, 그리고 렌더링 직후 작업을 설정하는 useEffect 등의 기능등을 제공하여 기존의 함수형 컴포넌트에서 할 수 없었던 다양한 작업을 할 수 있게 해준다.

### useState

가장 기본적인 Hook이다. 함수형 컴포넌트에서도 가변적인 상태를 지니고 있을 수 있게 해준다. 만약에 함수형 컴포넌트에서 상태를 관리해야 되는 일이 발생한다면 이 Hook 을 사용하면 된다.

## 라이프 사이클

라이프 사이클은 간단히 말하면 컴포넌트가 (생성 , 수정, 삭제) 이 세단계를 의미한다. 생성은 컴포넌트를 불러오는 것이고, 수정은 업데이트로 props가 바뀔때, state가 바뀔때, 부모 컴포넌트가 업데이트 되었을때 또는 강제로 업데이트를 했을때를 말한다.

## 클래스형 컴포넌트

```
import React, { Component } from 'react';

class App extends Component {
  render() {
    const name = '이종찬';
    return <h1>Hello, {name}</h1>
  }
}
```

클래스형 컴포넌트에서는 render() 함수를 이용하여, UI를 구성할 JSX 코드를 반환해주는 형식으로 구성되어야 한다.

## 함수형 컴포넌트

```
import React from 'react';

const App = () => {
  const name = '이종찬';
  return <h1>Hello, {name}</h1>
}
```

클래스형 컴포넌트보다 더 간결하며 리액트의 Hook을 이용한다. 현재 리액트는 클래스형보다 함수형을 더 선호한다.