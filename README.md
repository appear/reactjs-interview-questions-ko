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
|21 | [What are forward refs?](#what-are-forward-refs) |
|22 | [Which is preferred option with in callback refs and findDOMNode()?](#which-is-preferred-option-with-in-callback-refs-and-finddomnode) |
|23 | [Why are String Refs legacy?](#why-are-string-refs-legacy) |
|24 | [What is Virtual DOM?](#what-is-virtual-dom) |
|25 | [How Virtual DOM works?](#how-virtual-dom-works) |
|26 | [What is the difference between Shadow DOM and Virtual DOM?](#what-is-the-difference-between-shadow-dom-and-virtual-dom) |
|27 | [What is React Fiber?](#what-is-react-fiber) |
|28 | [What is the main goal of React Fiber?](#what-is-the-main-goal-of-react-fiber) |
|29 | [What are controlled components?](#what-are-controlled-components) |
|30 | [What are uncontrolled components?](#what-are-uncontrolled-components) |
|31 | [What is the difference between createElement and cloneElement?](#what-is-the-difference-between-createelement-and-cloneelement)|
|32 | [What is Lifting State Up in ReactJS?](#what-is-lifting-state-up-in-reactjs)|
|33 | [What are the different phases of ReactJS component lifecycle?](#what-are-the-different-phases-of-reactjs-component-lifecycle)|
|34 | [What are the lifecycle methods of ReactJS?](#what-are-the-lifecycle-methods-of-reactjs)|
|35 | [What are Higher-Order components?](#what-are-higher-order-components)|
|36 | [How to create props proxy for HOC component?](#how-to-create-props-proxy-for-hoc-component)|
|37 | [What is context?](#what-is-context)|
|38 | [What is children prop?](#what-is-children-prop)|
|39 | [How to write comments in ReactJS?](#how-to-write-comments-in-reactjs)|
|40 | [What is the purpose of using super constructor with props argument?](#what-is-the-purpose-of-using-super-constructor-with-props-argument)|

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

21. ### What are forward refs?
#### (forward refs 란 무엇인가요?)

Ref Forwarding 은 ref를 받아 child component 에게 전달하는 기능을합니다.

```js
const ButtonElement = React.forwardRef((props, ref) => (
  <button ref={ref} className="CustomButton">
    {props.children}
  </button>
));

// Create ref to the DOM button:
const ref = React.createRef();
<ButtonElement ref={ref}>{'Forward Ref'}</ButtonElement>
```

22. ### Which is preferred option with in callback refs and findDOMNode()?
#### (callback refs 와 findDOMNode 중에 어떤것을 더 선호하나요?)

findDOMNode API 보다 callback refs를 사용하는 것이 좋습니다. [findDOMNode](https://reactjs.org/docs/react-dom.html#finddomnode)는 향후 개선사항에서 React의 특성을 막기 떄문입니다.

findDOMNode 를 사용하는 legacy 한 방식입니다.

```js
class MyComponent extends Component {
  componentDidMount() {
    findDOMNode(this).scrollIntoView()
  }

  render() {
    return <div />
  }
}
```

권장하는 방법입니다.

```js
class MyComponent extends Component {
  componentDidMount() {
    this.node.scrollIntoView()
  }

  render() {
    return <div ref={node => this.node = node} />
  }
}
```

23. ### Why are String Refs legacy?
(왜 String Refs 는 legacy가 되었나요?)

만약 예전 React에서 ref 를 다뤄봤다면, ref={'textInput'} 과 같은 ref 의 속성이 string 이고 DOM Node가 refs.textInput 으로 접근하는 API 방식에 익숙할 것 입니다.  
String refs 는 아래와 같은 문제들이 있기 떄문에 legacy 를 고려하였습니다. React v16 에서 String refs는 제거되었습니다.

1. String refs 는 실행중인 component 요소를 추적하도록 강제화합니다. 또 react module 을 stateful 하게 만듭니다. bundle시 react module 들이 중복될 때
 이상한 오류를 발생시킵니다.
2. 라이브러리를 추가하여 String Refs를 Child component 에 전달하면, 사용자는 다른 ref를 추가할 수 없게됩니다. Callback refs를 이용한다면 이런 문제를 해결할 수 있습니다.
3. Flow 와 같은 static 분석에서는 동작하지 않습니다. Flow 는 string refs를 this.refs 같은 형태로 표시하도록 만드는 마법을 추측할 수 없습니다. callback ref는 String refs 보다 Flow 와 친밀합니다. 
4. 대부분의 사람들이 "render callback" 패턴으로 동작하기를 기대하지만 그렇게 동작하지 않습니다.

```js
class MyComponent extends Component {
  renderRow = (index) => {
    // 이것은 동작하지 않습니다. Ref는 MyComponent가 아닌 DataTable 에 연결될 것입니다. 
    return <input ref={'input-' + index} />;

    // 이것은 동작합니다. Callback refs는 굉장합니다.
    return <input ref={input => this['input-' + index] = input} />;
  }

  render() {
    return <DataTable data={this.props.data} renderRow={this.renderRow} />
  }
}
```

24. ### What is Virtual DOM?
#### (가상돔이란 무엇인가요?)
가상돔이란 in-memory 즉 Real DOM의 메모리상에서의 표현입니다. UI의 표현은 메모리에 유지되고 Render함수와 화면을 표시하는 사이에 Real DOM 과 동기화됩니다. 이런 단계를 reconciliation 라고 부릅니다.

25. ### How Virtual DOM works?
#### [(가상돔은 어떻게 동작하나요?)](https://www.youtube.com/watch?v=BYbgopx44vo)
가상돔은 세 가지의 간단한 단계로 동작합니다.

1. 데이터가 변경될 때 전체 UI 는 가상돔안에서 re-rendered 됩니다.   

![vdom](./public/vdom1.png)

2. 그런 다음 변경되기전 DOM 과 새로운 변경된 DOM 의 변경점을 계산합니다.   

![vdom](./public/vdom2.png)

3. 계산이 완료되면 실제 DOM 에서 계산된 변경점들만 업데이트됩니다.     

![vdom](./public/vdom3.png)

26. ### What is the difference between Shadow DOM and Virtual DOM?
#### (Shadow DOM과 Virtual DOM의 차이점은 무엇인가요?)
Shadow DOM은 web component의 scope 및 CSS scope 지정을 위해 설계된 web browser 기술입니다. Virtual DOM 은 browser API를 기반으로 JS 라이브러리에서 구현되는 개념입니다.

27. ### What is React Fiber?
#### (React Fiber란 무엇인가요?)
React Fiber란 React v16 에서 핵심 알고리즘을 재구현 한것입니다. React Fiber 의 목표는 애니메이션, 레이아웃, 제스처, 작업을 일시정지하고, 중단 또는 재사용, 여러 유형의 업데이트 우선순위 조절, 동시성등 여러 기본사항에 대한 성능을 높이는 것 입니다.

28. ### What is the main goal of React Fiber?
#### (React Fiber의 주요 목표는 무엇인가요?)
React Fiber 의 목표는 애니메이션, 레이아웃, 제스처등의 성능을 높이는 것 입니다. 주요 목적은 incremental rendering 입니다.

**incremental rendering:** 렌더링 작업을 청크로 쪼개고 여러 프레임으로 분산 시키는 기능입니다.

29. ### What are controlled components?
#### (controlled components 란 무엇인가요?)
입력 요소를 제어하는 component를 controlled components 라고 부릅니다. 모든 상태 변경에는 연관된 handler funciton 이 있습니다.

예를 들어, 이름을 대문자로 쓰려면 아래 handleChange을 이용할 수 있습니다.

```js
handleChange(event) {
  this.setState({value: event.target.value.toUpperCase()})
}
```

30. ### What are uncontrolled components?
#### (uncontrolled components 란 무엇인가요?)
uncontrolled components란 내부적으로 자기 자신의 state를 가지고 있는 component입니다. 현재 필요한 값을 찾기 위해 ref를 사용하여 DOM query를 할 수 있습니다. 이것은 전통적인 HTML 과 비슷합니다.

아래의 UserProfile Component 에서의 이름 입력은 ref를 사용하여 접근합니다.

```js
class UserProfile extends React.Component {
  constructor(props) {
    super(props)
    this.handleSubmit = this.handleSubmit.bind(this)
    this.input = React.createRef()
  }

  handleSubmit(event) {
    alert('A name was submitted: ' + this.input.current.value)
    event.preventDefault()
  }

  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <label>
          {'Name:'}
          <input type="text" ref={this.input} />
        </label>
        <input type="submit" value="Submit" />
      </form>
    );
  }
}
```
  
대부분의 경우 forms 을 제어할 때는 controlled component 를 사용하는 것을 추천합니다.

31. ### What is the difference between createElement and cloneElement?
#### (createElement와 cloneElement의 차이점은 무엇인가요?)
UI 의 object representation으로 사용될 react element를 만들기 위해 JSX element 는 React.createElement() 함수로 변환됩니다. cloneElement는 element 를 복사하고 새로운 props 를 전달하는데 사용됩니다.

32. ### What is Lifting State Up in React?
#### (React 에서 Lifting State Up 은 무엇인가요?)
여러 component 들이 동일한 변경 데이터를 공유해야하는 경우 가까운 부모 component 로 state를 올리는 것이 좋습니다. 즉, 두개의 자식 component가 부모의 있는 동일한 데이터를 공유할 때 두개의 자식 component 들은 부모로 state를 올리는 대신 local state를 유지해야합니다.

33. ### What are the different phases of component lifecycle?
#### (component 라이프사이클 단계는 무엇이 다른가요?)
라이프 사이클에는 4가지 단계가 있습니다.

1. Initialization: component 는 초기 state 및 props 를 세팅을 준비합니다.
2. Mounting: component 가 브라우저 DOM에 mount 될 준비가 되었습니다. 이 단계에서는 componentWillMount, componentDidMount 를 사용할 수 있습니다.
3. Updating: 새로운 props를 보내거나 state를 업데이트하여 component 를 두가지 방법으로 update 할 수 있습니다. 이 단계에서는 shouldComponentUpdate (), componentWillUpdate () 및 componentDidUpdate 를 사용할 수 있습니다.
4. Unmounting: 브라우저 DOM에서 component 가 필요하지 않을때 mount를 해제시킵니다. 이 단계에서는 componentWillUnmount 를 사용할 수 있습니다.

![lifecycle](./public/phases.png)

34. ### What are the lifecycle methods of React?
#### (React의 lifecycle methods는 무엇인가요?)
- componentWillMount: rendering 전에 실행됩니다.
- componentDidMount: 첫 rendering 후에 실행됩니다. 이 단계에서 모든 AJAX 요청, DOM 또는 State의 update, event listener 가 설정되어야합니다.
- componentWillReceiveProps: 특정 props update가 state 변화를 트리거할 때 실행됩니다.
- shouldComponentUpdate: 컴포넌트의 업데이트 여부를 결정합니다. 기본적으로 return 값은 true 입니다. state 또는 props 가 업데이트 된 후 component 를 render 할 필요가 없을 경우 false를 return 할 수 있습니다. component가 새로운 props를 받으면서 생기는 rerender 을 막을 수 있습니다. 성능을 향상시키는데 좋습니다.
- componentWillUpdate: shouldComponentUpdate에서 true가 반환되었을 때 state & props 의 변화를 확인하고 re-rendering 되기전에 실행합니다.
- componentDidUpdate: 주로 props 나 state 변경에 대한 response 로 DOM을 업데이트할 때 사용됩니다.
- componentWillUnmount: 네트워크 요청을 취소하거나, component와 관련된 모든 event listeners 를 제거하는데 사용됩니다.

35. ### What are Higher-Order components?
#### (Higher-Order components 는 무엇인가요?)
Higher-Order component(HOC)는 component를 받아서 새로운 component를 return 하는 함수입니다. HOC는 React의 특성에서 파생된 패턴입니다. 
동적으로 제공되는 하위 component들을 그대로 사용하지만 입력받은 component를 수정하거나 복사하지 않기 때문에 "순수 components" 라고 부릅니다.

```js
const EnhancedComponent = higherOrderComponent(WrappedComponent);
```

HOC는 아래와 같은 많은 use cases 에 사용할 수 있습니다.

- Code reuse, logic and bootstrap abstraction
- Render High jacking
- State abstraction and manipulation
- Props manipulation

36. ### How to create props proxy for HOC component?
#### (HOC component 위한 props proxy 만드는법?)
다음과 같이 component에 전달된 props를 props proxy로 추가 / 편집 할 수 있습니다. 

```js
function HOC(WrappedComponent) {
  return class Test extends Component {
    render() {
      const newProps = {
        title: 'New Header',
        footer: false,
        showFeatureX: false,
        showFeatureY: true
      };

      return <WrappedComponent {...this.props} {...newProps} />
    }
  }
}
```

37. ### What is context?
#### (context가 뭔가요?)
Context 는 모든 레벨에 수동으로 props를 전달하지 않고 component tree를 통해 데이터를 전달할 수 있도록 제공해줍니다.
예를 들어, 인증된 유저, locale 설정, UI 테마는 많은 application 들에서 접근해야합니다.  

```js
const {Provider, Consumer} = React.createContext(defaultValue);
```

38. ### What is children prop?
#### (children prop란 무엇인가요?)
Children prop는 component를 data로 다른 component로 전달할 수 있도록 해주는 prop(this.prop.children)입니다.  
당신이 사용하는 prop 처럼 사용할 수 있습니다. React API에는 이 props와 함께 사용할 수 있는  React.Children.map, React.Children.forEach, React.Children.count, React.Children.only, React.Children.toArray등 여러가지 방법이 있습니다.

children prop의 간단한 사용법은 아래와 같습니다.

```js
var MyDiv = React.createClass({
  render: function() {
    return <div>{this.props.children}</div>;
  }
});

ReactDOM.render(
  <MyDiv>
    <span>Hello</span>
    <span>World</span>
  </MyDiv>,
  node
);
```

39. ### How to write comments in ReactJS?
#### (React에서 주석은 어떻게 쓰나요?)
ReactJS / JSX 에서의 주석은 JavaScript와 유사합니다. 한 줄 및 여러 줄 주석들은 모두 중괄호로 감쌉니다. 

#### Single-line comments:
```jsx
<div>
  {/* Single-line comments */}    // In vanilla JavaScript, the single-line comments are represented by double slash(//)
  Welcome {user}, Let's play React
</div>
```

#### Multi-line comments:
```jsx
<div>
  {/* Multi-line comments for more than
   one line */}
  Welcome {user}, Let's play React
</div>
```

40. ### What is the purpose of using super constructor with props argument?
#### (props argument와 함께 super constructor를 사용하는 목적은 무엇인가요?)
자식 클래스의 constructor 는 super() 메서드가 호출되기 전까지 this 참조 사용할 수 없습니다. es6 의 sub-classes 에서도 동일하게 적용됩니다.
super()에 props를 파라미터로 전달하는 이유는 child constructors에서 this.props로 접근하기 위해서입니다. 

#### Passing props:
```js
class MyComponent extends React.Component {
    constructor(props) {
        super(props);

        console.log(this.props);  // Prints { name: 'sudheer',age: 30 }
    }
}
```

#### Not passing props:
```js
class MyComponent extends React.Component {
    constructor(props) {
        super();

        console.log(this.props); // Prints undefined

        // But Props parameter is still available
        console.log(props); // Prints { name: 'sudheer',age: 30 }
    }

    render() {
        // No difference outside constructor
        console.log(this.props) // Prints { name: 'sudheer',age: 30 }
    }
}
```

위의 code snippets은 this.props의 동작이 constructor 만 다른 것을 보여줍니다. 생성자 밖에서의 동작은 동일합니다. 

41. ### What is reconciliation?
#### ([reconciliation](https://reactjs.org/docs/reconciliation.html)란 무엇인가요?)
Component 의 props 또는 state가 변경될 때 React는 새로 반환된 component를 이전에 rendered 된 component와 비교하여 DOM update가 필요한지 결정합니다. 두개의 component가 같지 않을때 React는 DOM을 update합니다. 이를 프로세스 reconciliation 라고합니다.

42. ### How to set state with a dynamic key name?
#### (동적 key name 으로 어떻게 set State를 하나요?)
만약 ES6 나 babel transpiler 사용하여 JSX 코드를 변환하는 경우 computed property names 으로 작업을 할 수 있습니다. 

```js
handleInputChange(event) {
  this.setState({ [event.target.id]: event.target.value })
}
```

43. ### What would be the common mistake of function being called every time the component renders?
#### (render가 될 때마다 호출되는 function 의 일반적인 실수는 무엇인가요?)

function을 parameter로 전달하는 동안 function 이 호출되지 않았는지 확인해야합니다. 

```js
render() {
  // Wrong: handleClick is called instead of passed as a reference!
  return <button onClick={this.handleClick()}>{'Click Me'}</button>
}
```

괄호 없이 function 을 전달하세요

```js
render() {
  // Correct: handleClick is passed as a reference!
  return <button onClick={this.handleClick}>{'Click Me'}</button>
}
```

44. ### Why is it necessary to capitalize component names?
#### (왜 Component 의 이름은 대문자로 표기해야하나요?)

Component 들은 DOM element가 아니기 때문에 대문자 표기가 필요합니다. component들은 constructors입니다. 또한 JSX 에서의 소문자 태그 이름은 component가 아닌 HTML 요소를 나타내기 때문입니다.

45. ### Why React uses className over class attribute?
#### (왜 React 는 class를 사용하지 않고 className 속성을 사용하나요?)
class는 Javascript 의 키워드입니다. JSX는 Javascript 의 확장입니다. 그것이 React가 class 대신 className을 사용하는 이유입니다. classNames prop 로 문자열을 전달하세요

```js
render() {
  return <span className={'menu navigation-menu'}>{'Menu'}</span>
}
```

46. ### What are fragments?
#### (fragments는 무엇인가요 ?)
fragments는 여러 Component 들을 반환하는데 사용되는 React의 일반적인 패턴입니다. fragments를 사용하면 DOM에 node 들을 추가하지 않고 하위 목록을 그룹화 할 수 있습니다. 

```js
render() {
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
      <ChildC />
    </React.Fragment>
  )
}
```

더 짧은 구문도 있지만, 많은 tool 들에서 지원되지 않습니다.

```js
render() {
  return (
    <>
      <ChildA />
      <ChildB />
      <ChildC />
    </>
  )
}
```

47. ### Why fragments are better than container divs?
#### (왜 fragments 가 div 보다 좋나요 ?)
1. Fragments 는 빠르고 DOM node를 만들지 않기 때문에 메모리를 적게 사용합니다. 이것은 매우 크고 깊은 트리에서 이익을 가집니다.  
2. Flexbox 나 CSS Grid과 같은 CSS 메커니즘에는 특별한 부모 - 자식 관계를 가지고 있습니다. 중간에 div 들을 추가하게 된다면 layout을 유지하기 어려워집니다. 
3. DOM Inspector은 덜 복잡합니다.

48. ### What are portals in React?
#### (React 에서 portals은 무엇입니까 ?)
portals 은 상위 Component 의 DOM 계층 구조 외부에 존재하는 DOM 노드로 자식을 render 하는데 권장되는 방법입니다. 

```js
ReactDOM.createPortal(child, container)
```

첫 번째 인자는 렌더링 가능한 React 하위요소 (element, string, fragment) 입니다. 두 번째 인자는 DOM element 입니다.


