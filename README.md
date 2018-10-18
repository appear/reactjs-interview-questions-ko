# reactjs-interview-questions-ko

원작자인 [sudheerj](https://github.com/sudheerj) 의 동의를 구하고 진행하는 번역본 입니다 :)   
영어 원본: https://github.com/sudheerj/reactjs-interview-questions#what-is-reactjs

처음 해보는 번역이라 어색한 문맥이 많습니다 :) ..  

-------------------------------------------------------------------
| No. | Questions |
|---- | ---------
||**Core ReactJS**| |
|1  | [What is ReactJS?](#what-is-reactjs) |
|2  | [What are the major features of ReactJS?](#what-are-the-major-features-of-reactjs)|
|3  | [What is JSX?](#what-is-jsx)|
|4  | [What is the difference between Element and Component?](#what-is-the-difference-between-element-and-component)|
|5  | [How to create components in ReactJS?](#how-to-create-components-in-reactjs)|
|6  | [When to use a Class Component over a Functional Component?](#when-to-use-a-class-component-over-a-functional-component)|
|7  | [What are Pure Components?](#what-are-pure-components)|
|8  | [What is state in ReactJS?](#what-is-state-in-reactjs)|
|9  | [What is props in ReactJS?](#what-is-props-in-reactjs)|
|10 | [What is the difference between state and props?](#what-is-the-difference-between-state-and-props)|
|11 | [Why should not we update the state directly?](#why-should-not-we-update-the-state-directly)|
|12 | [What is the purpose of callback function as an argument of setState?](#what-is-the-purpose-of-callback-function-as-an-argument-of-setstate)
|13 | [What is the difference of event handling between HTML and React?](#what-is-the-difference-of-event-handling-between-html-and-react)|
|14 | [How to bind methods or event handlers in JSX callbacks?](#how-to-bind-methods-or-event-handlers-in-jsx-callbacks)|
|15 | [How to pass a parameter to an event handler or callback?](#how-to-pass-a-parameter-to-an-event-handler-or-callback)|
|16 | [What are synthetic events in ReactJS?](#what-are-synthetic-events-in-reactjs)|
|17 | [What is inline conditional expressions?](#what-is-inline-conditional-expressions)|
|18 | [What is Key and benefit of using it in lists?](#what-is-key-and-benefit-of-using-it-in-lists)|
|19 | [What is the use of create refs?](#what-is-the-use-of-create-refs)|
|20 | [How to create refs?](#how-to-create-refs)

## Core ReactJS

1. ### What is ReactJS? 
#### (React란 무엇인가요?)
[React](https://reactjs.org/docs/hello-world.html)는 SPA (Single Page Application) 즉, 단일 페이지 응용 프로그램에서 사용자 인터페이스를 구성는데 사용되는 오픈 소스 프론트엔드 JS 라이브러리 입니다.   
웹 및 모바일 앱의 Layer 를 다루는데 사용됩니다. 리액트는 페이스북의 소프트웨어 엔지니어 [Jordan Walke](https://twitter.com/jordwalke) 에 의해 만들어졌습니다.  
리액트는 2011 년 페이스북 뉴스피드에 발표되었고, 2012년 인스타그램에 처음 구축되었습니다.

2. ### What are the major features of ReactJS? 
#### (React의 특징은 무엇이 있을까요?)
React 의 주요 특징은 아래와 같습니다.
- RealDOM 을 조작하는데 많은 비용이 들어간다는 점을 고려하여 리액트는 RealDOM 대신 [VirtualDOM](https://www.youtube.com/watch?v=BYbgopx44vo)을 사용합니다.
- [서버 사이드 렌더링](https://subicura.com/2016/06/20/server-side-rendering-with-react.html)을 지원합니다.
- 단방향 데이터 흐름 또는 데이터 바인딩을 따릅니다.
- UI 구성 요소를 재사용할 수 있도록 개발할 수 있습니다.

3. ### What is JSX? 
#### (JSX란 무엇인가요?)
[JSX](https://reactjs.org/docs/introducing-jsx.html) 는 JS XML (ECMAScript로 XML 유사 구문 확장) 의 구문 표기법입니다. JSX 는 JS XML의 약자입니다.  
[HTML](https://ko.wikipedia.org/wiki/HTML)과 같은 문법과 함께 JS를 표현할 수 있습니다. 
예를 들면 아래의 h1 태그안에 text 는 render 함수에 의해 JS 함수로 반환됩니다. 

```js
render() {
  return (
    <div>
      <h1> Welcome to React world!!</h1>
    </div>
  );
}
```

4. ### What is the difference between Element and Component? 
#### (element와 component의 차이점은 무엇인가요?)
[element](https://ko.wikipedia.org/wiki/HTML_%EC%9A%94%EC%86%8C)는 DOM 노드 또는 다른 [component](https://reactjs.org/docs/react-component.html)들과 관련하여 화면에 표시 할 내용을 표현하는 일반 객체입니다. elements는 다른 elements 들을 포함할 수 있습니다.
[React element](https://reactjs.org/docs/rendering-elements.html)를 만드는 비용은 저렴합니다. element 는 생성되면 변형되지 않습니다. 리액트 element 의 표현은 아래와 같습니다.

```js
const element = React.createElement(
  'div',
  {id: 'login-btn'},
  'Login'
)
```

위에서 만들어진 element 는 아래와 같은 객체로 리턴됩니다.
```js
{
  type: 'div',
  props: {
    children: 'Login',
    id: 'login-btn'
  }
}
```

마지막으로 아래와 같이 [**ReactDOM.render**](https://reactjs.org/docs/react-dom.html) 를 이용하여 DOM 으로 렌더링합니다.

```js
<div id='login-btn'>Login</div>
```

반면 component 는 여러 방법으로 선언될 수 있습니다. render 메서드가 있는 class 일 수도 있습니다. 간단한 component 일 경우 function으로 정의 될 수 있습니다.
입력된 component 를 바탕으로 element 트리를 만듭니다. 마지막에 JSX 는 [createElement로 변환](https://reactjs.org/docs/jsx-in-depth.html)됩니다. 

```js
function Button ({ onLogin }) {
  return React.createElement(
    'div',
    {id: 'login-btn', onClick: onLogin},
    'Login'
  )
}
```

5. ### How to create components in ReactJS? 
#### (React에서 컴포넌트를 어떻게 생성하나요?)   
ReactJS 는 Components 생성하는 두 가지 방법이 있습니다.

1. **Functional components**
ReactJS 에서 component를 생성하는 가장 간단한 방법입니다. props 를 받을 수 있고 React elements 를 리턴할 수 있습니다. 
이런 방법을 pure 한 JS의 function 이기 때문에 functional한 생성법이라고 부릅니다.

```js
function Greeting(props) {  
  return <h1> Hello, {props.message}</h1> 
}
```

2. **Class components**
ES6 [Class](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Classes)를 사용하여 component 를 정의할 수 있습니다. 위에서 본 functional 선언법을 아래와 같이 적용할 수 있습니다.

```js
class Greeting extends React.Component {
  render() {
    return <h1>Hello, {this.props.message}</h1>;
  }
}
```

6. ### When to use a Class Component over a Functional Component? 
#### (언제 클래스 컴포넌트를 사용하고 언제 Functional 컴포넌트를 사용할까요?)
Component 에서 state 또는 [life cycle methods](https://reactjs.org/docs/react-component.html#the-component-lifecycle) 를 필요로 한다면 Class component를 사용하고 그렇지 않다면 Functional component를 사용할 수 있습니다.

7. ### What are Pure Components? 
####(순수 컴포넌트란 무엇인가요?)
[PureComponent](http://lucybain.com/blog/2018/react-js-pure-component)는 동일한 상태에서는 동일한 결과를 반환합니다. [shouldComponentUpdate](https://reactjs.org/docs/react-component.html#shouldcomponentupdate) 메서드를 다룰 수 있다는 점을 제외하고는 component와 동일합니다.   
props 또는 state 가 변경될 때 PureComponent 는 state 와 props 에 대해 [Shallow Compare](https://reactjs.org/docs/shallow-compare.html)을 수행합니다.  
반면 component는 현재 props와 변형될 state를 비교하지 않습니다. 그렇기 때문에 component는 shouldComponentUpdate가 호출 될 때 마다 다시 render 됩니다. (shouldComponentUpdate의 기본값은 true 이기 때문에)

8. ### What is state in ReactJS? 
#### (state란 무엇인가요?)
Component [State](https://reactjs.org/docs/faq-state.html) 는 component의 life cycle 동안 변경될 수 있는 정보를 담고 있는 객체입니다. 우리는 state를 가능한 단순하게 만들고 state 의 구성 요소의 수를 최소화하기 위해 노력해야 합니다.

message state를 가진 user component 를 생성해보겠습니다.

```js
class User extends React.Component {
   constructor(props) {
      super(props);

      this.state = {
         message: "Welcome to React world",
      }
   }
   render() {
      return (
         <div>
            <h1>{this.state.message}</h1>
         </div>
      );
   }
}
```

![state](./public/state.jpg)

9. ### What is props in ReactJS ? 
#### (props란 무엇인가요?)
[Props](https://reactjs.org/docs/components-and-props.html) 는 HTML 태그 속성과 유사한 규칙을 사용하여 React component 에 전달되는 값을 포함하는 단일 값 또는 객체입니다. 부모 component 에서 자식 component 로 전달되는 데이터 입니다.

React에서 props 의 목적은 아래와 같은 기능을 component에 제공하는 것 입니다.

1. 사용자 정의 데이터를 React component 로 전달할 수 있습니다.
2. State 변경을 Trigger 할 수 있습니다.
3. Component 의 render 메서드 안에서 this.props.reactProp 로 접근하여 사용할 수 있습니다.

예를 들어, reactProp를 받는 element 를 만들고 

```js
<Element reactProp = "1" />
```

이 "reactProp" (또는 사용자가 찾은 정의한) props는 React를 사용하여 생성된 ccomponent에서 접근이 가능하고, React의 native props 영역에 포함된 속성이 됩니다.

```js
props.reactProp;
```

10. ### What is the difference between state and props ? 
#### (state와 props의 차이점은 무엇인가요?)
props와 state는 모두 JavaScript 객체입니다. 두가지 다 렌더링 결과에 영향을 주는 정보를 가지고 있지만, component 와 관련된 기능면에서 차이가 있습니다.  
props는 함수 매개변수와 같이 component 요소로 전달됩니다. state 는 component 안에서 관리되고 사용할 변수 선언과 비슷합니다.

11. ### Why should not we update the state directly? 
#### (state를 직접 업데이트 하면 안되는 이유는 무엇인가요?)
state를 직접 업데이트 하려고 한다면 component 는 re-render 되지 않습니다.

```js
//Wrong
this.state.message =”Hello world”;
```

그 대신 setState 메서드를 사용해야합니다. setState는 component state 업데이트에 대한 예약을합니다. state 가 변경되면 component는 re-rendering 할 것 입니다.

```js
//Correct
this.setState({message: ‘Hello World’});
```

Note: 상태를 할당할 수 있는 곳은 constructor 가 유일합니다. (외부에서 다이렉트로 state를 할당하지 말라는 뜻 같습니다.)

12. ### What is the purpose of callback function as an argument of setState? 
#### (setState에서 callback의 역할은 무엇인가요?)
callback 함수는 setState가 끝난 후 그리고 component 가 re-rendering 된 후 호출됩니다. setState는 비동기적으로 동작합니다. callback 함수는 모든 작업이 마무리된 후 사용됩니다. 

```js
setState({name: 'sudheer'}, () => console.log('The name has updated and component re-rendered'));
```
 
#### Note: callback 함수를 이용하는 것보단 lifecycle 메서드를 이용하는 것이 좋습니다.

13. ### What is the difference of event handling between HTML and React? 
#### (HTML과 React의 이벤트 처리 차이점은 무엇인가요?)
아래는 HTML과 React 의 이벤트처리의 몇 가지 차이점입니다.

1. HTML 에서는 이벤트 이름이 소문자여야 합니다.

```html
<button onclick="activateLasers()">
```

반면 React는 camelCase 를 사용합니다.

```html
<button onClick={activateLasers}>
```

2. HTML 에서는 기본 이벤트 동작을 막기위해 false 를 반환할 수 있습니다.

```html
<a href="#" onclick="console.log('The link was clicked.'); return false"/>
```

반면 React는 preventDefault 메서드를 호출해야합니다.

```js
function handleClick(e) {
  e.preventDefault();
  console.log('The link was clicked.');
}
```

14. ### How to bind methods or event handlers in JSX callbacks? (Or) How to use this keyword in JSX callbacks? 
#### (This를 바인딩하는 방법은 어떤 것들이 있나요?)
3가지의 방법이 있습니다.

1. 생성자에서의 바인딩: JS 의 Class 에서 메서드는 기본적으로 바인딩 되지 않습니다. 클래스 메서드로 지정된 React의 event handlers 에서도 마찬가지 입니다.  
일반적으로 다음과같이 constructor 바인딩합니다.

```js
constructor(props) {
  super(props);
  this.handleClick = this.handleClick.bind(this);
}

handleClick() {
  // Perform some logic
}
```

2. 공통 클래스 필드 구문: 생성자에서의 바인딩 방법을 원하지 않는다면, 공용 클래스 필드 구문을 이용하여 callback 을 올바르게 바인딩할 수 있습니다.

```js
handleClick = () => { 
  console.log('this is:', this);
}

<button onClick={this.handleClick}> Click me </button>
```

3. [arrow function](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Functions/%EC%95%A0%EB%A1%9C%EC%9A%B0_%ED%8E%91%EC%85%98)을 이용한 바인딩
아래와 같이 바로 arrow function 을 이용하여 바인딩 해줄 수 있습니다.

```html
<button onClick={(e) => this.handleClick(e)}>
  Click me
</button>
```

Note: 만약 callback 이 하위 component 에 props 로 전달되면 component는 re-rendering 될 수 있습니다. 이럴 경우 성능을 고려하였을때 1번 또는 2번의 방식을 사용하는 것이 좋습니다.

15. ### How to pass a parameter to an event handler or callback? 
#### (이벤트 핸들러 또는 콜백에 매개변수를 어떻게 전달하나요?)
arrow function 으로 감싸서 event handler 에게 매개변수를 전달할 수 있습니다.

```js
<button onClick={() => this.handleClick(id)} />
```

위의 방법은 아래와 같이 method 를 사용하는 것과 같습니다

```html
<button onClick={this.handleClick.bind(this, id)} />
```
 
16. ### What are synthetic events in ReactJS? 
#### (React에서의 합성 이벤트는 무엇인가요?)
[synthetic event](https://reactjs.org/docs/events.html) 는 브라우저의 기본 이벤트를 감싼 cross-browser wrapper 입니다. API는 모든 브라우저에서 동작한다는 점을 제외하면, stopPropagation () 및 preventDefault () 를 포함해 브라우저 네이티브 이벤트와 같은 인터페이스를 가지고 있습니다.

17. ### What is inline conditional expressions? 
#### (인라인 조건식은 무엇인가요?)
조건부 표현식을 표현하기 위해 if 문 또는 삼항 연산자를 사용할 수 있습니다. 이런 표현법 외에도 중괄호로 묶은 다음 JS의 논리 연산자 (&&) 를 붙여 JSX 표현식에 포함시킬 수 있습니다.

```html
<h1>Hello!</h1>
 {messages.length > 0 &&
<h2>
  You have {messages.length} unread messages.
</h2>
```

18. ### What is Key and benefit of using it in lists? 
#### (list 에서 key를 사용했을 때의 이점은 무엇인가요?)
["Key"](https://reactjs.org/docs/lists-and-keys.html)는 목록을 만들때 포함시켜야하는 특수한 속성입니다. "Key"는 목록의 변경사항, 추가 또는 제거된 항목을 분별할 수 있도록 도와줍니다.  

예를 들어, 데이터의 키를 자주 목록의 "Key"로 사용합니다.

```js
const todoItems = todos.map((todo) =>
  <li key={todo.id}>
    {todo.text}
  </li>
);
```
What is ReactJS? (React란 무엇인가요?)
렌더링 된 목록에 안정적인 ID가 없을 경우 마지막 수단으로 index 값을 이용할 수 있습니다.

```js
const todoItems = todos.map((todo, index) =>
  <li key={index}>
    {todo.text}
  </li>
);
```

Note: 
1. 항목 순서가 변경 될 가능성이 있는 경우 index를 이용하는 것은 좋지 않습니다. 성능에 부정적인 영향을 미치고 component state에 문제가 발생할 수 있습니다.
2. list를 별도의 component로 뽑아 사용하는 경우 li 태그 대신 list component 요소에 key를 적용하세요

list 에 key 가 없으면 콘솔에 경고가 표시됩니다.

19. ### What is the use of create refs? 
#### (ref의 용도는 무엇인가요?)
두 가지의 접근법이 있습니다.

최근에 추가된 접근 방식입니다. [create ref](https://reactjs.org/docs/refs-and-the-dom.html)는 element 요소에 대한 참조를 반환하는데 사용할 수 있습니다. DOM의 요소나 compoennt 에 직접 접근해야 될 경우 유용할 수 있습니다.

20. ### How to create refs? 
#### (create refs를 어떻게 만드나요?) 
Ref는 React.createRef() 메서드를 사용하여 생성합니다. ref attribute 을 통해 React elements 에 첨부됩니다. component 전체에서 사용하고 싶다면 constructor에서 instance property 로 ref를 할당하면 됩니다.

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.myRef = React.createRef();
  }
  render() {
    return <div ref={this.myRef} />;
  }
}
```

2. React의 버전과 관계없이 ref callback 을 사용할 수 있습니다. 예를들어 serach bar component의 input element는 다음과 같이 접근합니다.

```js
class SearchBar extends Component {
   constructor(props) {
      super(props);
      this.txtSearch = null;
      this.state = { term: '' };
      this.setInputSearchRef = e => {
         this.txtSearch = e;
      }
   }
   onInputChange(event) {
      this.setState({ term: this.txtSearch.value });
   }
   render() {
      return (
         <input
            value={this.state.term}
            onChange={this.onInputChange.bind(this)}
            ref={this.setInputSearchRef} />
      );
   }
}
```

 
