# reactjs-interview-questions-ko ✈️

원작자인 [sudheerj](https://github.com/sudheerj) 의 동의를 구하고 진행하는 번역본 입니다 :)   

영어 원본은 [여기](https://github.com/sudheerj/reactjs-interview-questions#what-is-reactjs) 를 확인해주세요

저에게 도움을 주시고싶은 분들은 fork 후 pull request 부탁드립니다 !  🌸 


**도움이 되셨다면 star 를 눌러주세요 :)** 

-------------------------------------------------------------------
| No. | Questions |
|---- | ---------
||**Core ReactJS**| |
|1  | [What is ReactJS?](#1.what-is-reactjs) |
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
|32 | [What is Lifting State Up in React?](#what-is-lifting-state-up-in-react)|
|33 | [What are the different phases of component lifecycle?](#what-are-the-different-phases-of-component-lifecycle)|
|34 | [What are the lifecycle methods of React?](#what-are-the-lifecycle-methods-of-react)|
|35 | [What are Higher-Order components?](#what-are-higher-order-components)|
|36 | [How to create props proxy for HOC component?](#how-to-create-props-proxy-for-hoc-component)|
|37 | [What is context?](#what-is-context)|
|38 | [What is children prop?](#what-is-children-prop)|
|39 | [How to write comments in ReactJS?](#how-to-write-comments-in-reactjs)|
|40 | [What is the purpose of using super constructor with props argument?](#what-is-the-purpose-of-using-super-constructor-with-props-argument)|
|41 | [What is reconciliation?](#what-is-reconciliation) |
|42 | [How to set state with a dynamic key name?](#how-to-set-state-with-a-dynamic-key-name) |
|43 | [What would be the common mistake of function being called every time the component renders?](#what-would-be-the-common-mistake-of-function-being-called-every-time-the-component-renders) |
|44 | [Why is it necessary to capitalize component names?](#why-is-it-necessary-to-capitalize-component-names) |
|45 | [Why React uses className over class attribute?](#why-react-uses-classname-over-class-attribute) |
|46 | [What are fragments?](#what-are-fragments) |
|47 | [Why fragments are better than container divs?](#why-fragments-are-better-than-container-divs) |
|48 | [What are portals in React?](#what-are-portals-in-react) |
|49 | [What are stateless components?](#what-are-stateless-components) |
|50 | [What are stateful components?](#what-are-stateful-components) |
|51 | [How to apply validation on props in React?](#how-to-apply-validation-on-props-in-react) |
|52 | [What are the advantages of React?](#what-are-the-advantages-of-react) |
|53 | [What are the limitations of React?](#what-are-the-limitations-of-react) |
|54 | [What are error boundaries in React v16](#what-are-error-boundaries-in-react-v16) |
|55 | [How error boundaries handled in React v15?](#how-error-boundaries-handled-in-react-v15) |
|56 | [What are the recommended ways for static type checking?](#what-are-the-recommended-ways-for-static-type-checking) |
|57 | [What is the use of react-dom package?](#what-is-the-use-of-react-dom-package) |
|58 | [What is the purpose of render method of react-dom?](#what-is-the-purpose-of-render-method-of-react-dom) |
|59 | [What is ReactDOMServer?](#what-is-reactdomserver) |
|60 | [How to use InnerHtml in React?](#how-to-use-innerhtml-in-react) |
|61 | [How to use styles in React?](#how-to-use-styles-in-react) |
|62 | [How events are different in React?](#how-events-are-different-in-react) |
|63 | [What will happen if you use setState in constructor?](#what-will-happen-if-you-use-setstate-in-constructor) |
|64 | [What is the impact of indexes as keys?](#what-is-the-impact-of-indexes-as-keys) |
|65 | [Is it good to use setState() in componentWillMount() method?](#is-it-good-to-use-setstate-in-componentwillmount-method) |
|66 | [What will happen if you use props in initial state?](#what-will-happen-if-you-use-props-in-initial-state) |
|67 | [How do you conditionally render components?](#how-do-you-conditionally-render-components)
|68 | [Why we need to be careful when spreading props on DOM elements??](#why-we-need-to-be-careful-when-spreading-props-on-dom-elements) |
|69 | [How you use decorators in React?](#how-you-use-decorators-in-react) |
|70 | [How do you memoize a component?](#how-do-you-memoize-a-component) |
|71 | [How you implement Server-Side Rendering or SSR?](#how-you-implement-server-side-rendering-or-ssr) |
|72 | [How to enable production mode in React?](#how-to-enable-production-mode-in-react) |
|73 | [What is CRA and its benefits?](#what-is-cra-and-its-benefits) |
|74 | [What is the lifecycle methods order in mounting?](#what-is-the-lifecycle-methods-order-in-mounting) |
|75 | [What are the lifecycle methods going to be deprecated in React v16?](#what-are-the-lifecycle-methods-going-to-be-deprecated-in-react-v16) |
|76 | [What is the purpose of getDerivedStateFromProps() lifecycle method?](#what-is-the-purpose-of-getderivedstatefromprops-lifecycle-method) |
|77 | [What is the purpose of getSnapshotBeforeUpdate() lifecycle method?](#what-is-the-purpose-of-getsnapshotbeforeupdate-lifecycle-method) |
|78 | [What is the difference between createElement() and cloneElement() methods?](#what-is-the-difference-between-createelement-and-cloneelement-methods) |
|79 | [What is the recommended way for naming components?](#what-is-the-recommended-way-for-naming-components) |
|80 | [What is the recommended ordering of methods in component class?](#what-is-the-recommended-ordering-of-methods-in-component-class) |
|81 | [What is a switching component?](#what-is-a-switching-component) |
|82 | [Why we need to pass a function to setState()?](#why-we-need-to-pass-a-function-to-setstate) |
|83 | [What is strict mode in React?](#what-is-strict-mode-in-react) |
|84 | [What are React Mixins?](#what-are-react-mixins) |
|85 | [Why is isMounted() an anti-pattern and what is the proper solution?](#why-is-ismounted-an-anti-pattern-and-what-is-the-proper-solution) |
|86 | [What are the Pointer Events supported in React?](#what-are-the-pointer-events-supported-in-react) |
|87 | [Why should component names start with capital letter?](#why-should-component-names-start-with-capital-letter) |
|88 | [Are custom DOM attributes supported in React v16?](#are-custom-dom-attributes-supported-in-react-v16) |
|89 | [What is the difference between constructor and getInitialState?](#what-is-the-difference-between-constructor-and-getinitialstate) |
|90 | [Can you force a component to re-render without calling setState?](#can-you-force-a-component-to-re-render-without-calling-setstate) |
|91 | [What is the difference between super() and super(props) in React using ES6 classes?](#what-is-the-difference-between-super-and-superprops-in-react-using-es6-classes) |
|92 | [How to loop inside JSX?](#how-to-loop-inside-jsx) |
|93 | [How do you access props in attribute quotes?](#how-do-you-access-props-in-attribute-quotes) |
|94 | [What is React PropType array with shape?](#what-is-react-proptype-array-with-shape) |
|95 | [How conditionally apply class attributes?](#how-conditionally-apply-class-attributes) |
|96 | [What is the difference between React and ReactDOM?](#what-is-the-difference-between-react-and-reactdom) |
|97 | [Why ReactDOM is separated from React?](#why-reactdom-is-separated-from-react) |
|98 | [How to use React label element?](#how-to-use-react-label-element) |
|99 | [How to combine multiple inline style objects?](#how-to-combine-multiple-inline-style-objects) |
|100| [How to re-render the view when the browser is resized?](#how-to-re-render-the-view-when-the-browser-is-resized)
|101| [What is the difference between setState and replaceState methods?](#what-is-the-difference-between-setstate-and-replacestate-methods) |
|102| [How to listen to state changes?](#how-to-listen-to-state-changes) |
|103| [What is the recommended approach of removing an array element in react state?](#what-is-the-recommended-approach-of-removing-an-array-element-in-react-state) |
|104| [Is it possible to use React without rendering HTML?](#is-it-possible-to-use-react-without-rendering-html) |
|105| [How to pretty print JSON with React?](#how-to-pretty-print-json-with-react) |
|106| [Why you can't update props in React?](#why-you-cant-update-props-in-react) |
|107| [How to focus an input element on page load?](#how-to-focus-an-input-element-on-page-load) |
|108| [What are the possible ways of updating objects in state?](#what-are-the-possible-ways-of-updating-objects-in-state) |
|109| [Why function is preferred over object for setState?](#why-function-is-preferred-over-object-for-setstate) |
|110| [How can we find the version of React at runtime in the browser?](#how-can-we-find-the-version-of-react-at-runtime-in-the-browser) |
|111| [What are the approaches to include polyfills in your create-react-app?](#what-are-the-approaches-to-include-polyfills-in-your-create-react-app) |
|112| [How to use https instead of http in create-react-app?](#how-to-use-https-instead-of-http-in-create-react-app) |
|113| [How to avoid using relative path imports in create-react-app?](#how-to-avoid-using-relative-path-imports-in-create-react-app) |
|114| [How to add Google Analytics for react-router?](#how-to-add-google-analytics-for-react-router) |
|115| [How to update a component every second?](#how-to-update-a-component-every-second) |
|116| [How do you apply vendor prefixes to inline styles in React?](#how-do-you-apply-vendor-prefixes-to-inline-styles-in-react) |
|117| [How to import and export components using react and ES6?](#how-to-import-and-export-components-using-react-and-es6) |
|118| [Why React component names must begin with a capital letter?](#why-react-component-names-must-begin-with-a-capital-letter) |
|119| [Why is a component constructor called only once?](#why-is-a-component-constructor-called-only-once) |
|120| [How to define constants in React?](#how-to-define-constants-in-react) |
|121| [How to programmatically trigger click event in React?](#how-to-programmatically-trigger-click-event-in-react) |
|122| [Is it possible to use async/await in plain React?](#is-it-possible-to-use-asyncawait-in-plain-react) |
|123| [What are the common folder structures for React?](#what-are-the-common-folder-structures-for-react) |
|124| [What are the popular packages for animation?](#what-are-the-popular-packages-for-animation) |
|125| [What is the benefit of styles modules?](#what-is-the-benefit-of-styles-modules) |
|126| [What are the popular React-specific linters?](#what-are-the-popular-react-specific-linters) |
|127| [How to make AJAX call and In which component lifecycle methods should I make an AJAX call?](#how-to-make-ajax-call-and-in-which-component-lifecycle-methods-should-i-make-an-ajax-call) |
|128| [What are render props?](#what-are-render-props) |
|   | **React Router** |
|129| [What is React Router?](#what-is-react-router) |
|130| [How React Router is different from history library?](#how-react-router-is-different-from-history-library) |
|131| [What are the \<Router> components of React Router v4?](#what-are-the-router-components-of-react-router-v4) |
|132| [What is the purpose of push and replace methods of history?](#what-is-the-purpose-of-push-and-replace-methods-of-history) |
|133| [How do you programmatically navigate using React router v4?](#how-do-you-programmatically-navigate-using-react-router-v4) |
|134| [How to get query parameters in React Router v4](#how-to-get-query-parameters-in-react-router-v4) |
|135| [Why you get "Router may have only one child element" warning?](#why-you-get-router-may-have-only-one-child-element-warning) |
|136| [How to pass params to history.push method in React Router v4?](#how-to-pass-params-to-historypush-method-in-react-router-v4) |
|137| [How to implement default or NotFound page?](#how-to-implement-default-or-notfound-page) |
|138| [How to get history on React Router v4?](#how-to-get-history-on-react-router-v4) |
|139| [How to perform automatic redirect after login?](#how-to-perform-automatic-redirect-after-login) |
|   | **React Internationalization** |
|140| [What is React-Intl?](#what-is-react-intl) |
|141| [What are the main features of React Intl?](#what-are-the-main-features-of-react-intl) |
|142| [What are the two ways of formatting in React Intl?](#what-are-the-two-ways-of-formatting-in-react-intl) |
|143| [How to use FormattedMessage as placeholder using React Intl?](#how-to-use-formattedmessage-as-placeholder-using-react-intl) |
|144| [How to access current locale with React Intl](#how-to-access-current-locale-with-react-intl) |
|145| [How to format date using React Intl?](#how-to-format-date-using-react-intl) |
|   | **React Testing** |
|146| [What is Shallow Renderer in React testing?](#what-is-shallow-renderer-in-react-testing) |
|147| [What is TestRenderer package in React?](#what-is-testrenderer-package-in-react) |
|148| [What is the purpose of ReactTestUtils package?](#what-is-the-purpose-of-reacttestutils-package) |
|149| [What is Jest?](#what-is-jest) |
|150| [What are the advantages of Jest over Jasmine?](#what-are-the-advantages-of-jest-over-jasmine) |
|151| [Give a simple example of Jest test case](#give-a-simple-example-of-jest-test-case) |
|   | **React Redux** |
|152| [What is Flux?](#what-is-flux) |
|153| [What is Redux?](#what-is-redux) |
|154| [What are the core principles of Redux?](#what-are-the-core-principles-of-redux) |
|155| [What are the downsides of Redux compared to Flux?](#what-are-the-downsides-of-redux-compared-to-flux) |
|156| [What is the difference between mapStateToProps() and mapDispatchToProps()?](#what-is-the-difference-between-mapstatetoprops-and-mapdispatchtoprops) |
|157| [Can I dispatch an action in reducer?](#can-i-dispatch-an-action-in-reducer) |
|158| [How to access Redux store outside a component?](#how-to-access-redux-store-outside-a-component) |
|159| [What are the drawbacks of MVW pattern](#what-are-the-drawbacks-of-mvw-pattern) |
|160| [Are there any similarities between Redux and RxJS?](#are-there-any-similarities-between-redux-and-rxjs) |
|161| [How to dispatch an action on load?](#how-to-dispatch-an-action-on-load) |
|162| [How to use connect from React Redux?](#how-to-use-connect-from-react-redux) |
|163| [How to reset state in Redux?](#how-to-reset-state-in-redux) |
|164| [Whats the purpose of at symbol in the redux connect decorator?](#whats-the-purpose-of-at-symbol-in-the-redux-connect-decorator) |
|165| [What is the difference between React context and React Redux?](#what-is-the-difference-between-react-context-and-react-redux) |
|166| [Why are Redux state functions called reducers?](#why-are-redux-state-functions-called-reducers) |
|167| [How to make AJAX request in Redux?](#how-to-make-ajax-request-in-redux) |
|168| [Should I keep all component's state in Redux store?](#should-i-keep-all-components-state-in-redux-store) |
|169| [What is the proper way to access Redux store?](#what-is-the-proper-way-to-access-redux-store) |
|170| [What is the difference between component and container in React Redux?](#what-is-the-difference-between-component-and-container-in-react-redux) |
|171| [What is the purpose of the constants in Redux? ](#what-is-the-purpose-of-the-constants-in-redux) |
|172| [What are the different ways to write mapDispatchToProps()?](#what-are-the-different-ways-to-write-mapdispatchtoprops) |
|173| [What is the use of the ownProps parameter in mapStateToProps() and mapDispatchToProps()?](#what-is-the-use-of-the-ownprops-parameter-in-mapstatetoprops-and-mapdispatchtoprops) |
|174| [How to structure Redux top level directories?](#how-to-structure-redux-top-level-directories) |
|175| [What is redux-saga?](#what-is-redux-saga) |
|176| [What is the mental model of redux-saga?](#what-is-the-mental-model-of-redux-saga) |
|177| [What are the differences between call and put in redux-saga](#what-are-the-differences-between-call-and-put-in-redux-saga) |
|178| [What is Redux Thunk?](#what-is-redux-thunk) |
|179| [What are the differences between redux-saga and redux-thunk](#what-are-the-differences-between-redux-saga-and-redux-thunk) |


## Core ReactJS

### 1. What is ReactJS? 
#### (React란 무엇인가요?)
[React](https://reactjs.org/docs/hello-world.html)는 SPA (Single Page Application) 즉, 단일 페이지 응용 프로그램에서 사용자 인터페이스를 구성는데 사용되는 오픈 소스 프론트엔드 JS 라이브러리 입니다.   
웹 및 모바일 앱의 Layer 를 다루는데 사용됩니다. 리액트는 페이스북의 소프트웨어 엔지니어 [Jordan Walke](https://twitter.com/jordwalke) 에 의해 만들어졌습니다.  
리액트는 2011 년 페이스북 뉴스피드에 발표되었고, 2012년 인스타그램에 처음 구축되었습니다.

### 2. What are the major features of ReactJS? 
#### (React의 특징은 무엇이 있을까요?)
React 의 주요 특징은 아래와 같습니다.
- RealDOM 을 조작하는데 많은 비용이 들어간다는 점을 고려하여 리액트는 RealDOM 대신 [VirtualDOM](https://www.youtube.com/watch?v=BYbgopx44vo)을 사용합니다.
- [서버 사이드 렌더링](https://subicura.com/2016/06/20/server-side-rendering-with-react.html)을 지원합니다.
- 단방향 데이터 흐름 또는 데이터 바인딩을 따릅니다.
- UI 구성 요소를 재사용할 수 있도록 개발할 수 있습니다.

### 3. What is JSX? 
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

### 4. What is the difference between Element and Component? 
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

### 5. How to create components in ReactJS? 
#### (React에서 컴포넌트를 어떻게 생성하나요?)   
ReactJS 는 Components 생성하는 두 가지 방법이 있습니다.

**Functional components**

ReactJS 에서 component를 생성하는 가장 간단한 방법입니다. props 를 받을 수 있고 React elements 를 리턴할 수 있습니다. 
이런 방법을 pure 한 JS의 function 이기 때문에 functional한 생성법이라고 부릅니다.

```js
function Greeting(props) {  
  return <h1> Hello, {props.message}</h1> 
}
```

**Class components**

ES6 [Class](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Classes)를 사용하여 component 를 정의할 수 있습니다. 위에서 본 functional 선언법을 아래와 같이 적용할 수 있습니다.

```js
class Greeting extends React.Component {
  render() {
    return <h1>Hello, {this.props.message}</h1>;
  }
}
```

### 6. When to use a Class Component over a Functional Component? 
#### (언제 클래스 컴포넌트를 사용하고 언제 Functional 컴포넌트를 사용할까요?)

Component 에서 state 또는 [life cycle methods](https://reactjs.org/docs/react-component.html#the-component-lifecycle) 를 필요로 한다면 Class component를 사용하고 그렇지 않다면 Functional component를 사용할 수 있습니다.

### 7. What are Pure Components? 
#### (순수 컴포넌트란 무엇인가요?)

[PureComponent](http://lucybain.com/blog/2018/react-js-pure-component)는 동일한 상태에서는 동일한 결과를 반환합니다. [shouldComponentUpdate](https://reactjs.org/docs/react-component.html#shouldcomponentupdate) 메서드를 다룰 수 있다는 점을 제외하고는 component와 동일합니다.   
props 또는 state 가 변경될 때 PureComponent 는 state 와 props 에 대해 [Shallow Compare](https://reactjs.org/docs/shallow-compare.html)을 수행합니다.  
반면 component는 현재 props와 변형될 state를 비교하지 않습니다. 그렇기 때문에 component는 shouldComponentUpdate가 호출 될 때 마다 다시 render 됩니다. (shouldComponentUpdate의 기본값은 true 이기 때문에)

### 8. What is state in ReactJS? 
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

### 9. What is props in ReactJS? 
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

이 "reactProp" (또는 사용자가 찾은 정의한) props는 React를 사용하여 생성된 component에서 접근이 가능하고, React의 native props 영역에 포함된 속성이 됩니다.

```js
props.reactProp;
```

### 10. What is the difference between state and props? 
#### (state와 props의 차이점은 무엇인가요?)
props와 state는 모두 JavaScript 객체입니다. 두가지 다 렌더링 결과에 영향을 주는 정보를 가지고 있지만, component 와 관련된 기능면에서 차이가 있습니다.  
props는 함수 매개변수와 같이 component 요소로 전달됩니다. state 는 component 안에서 관리되고 사용할 변수 선언과 비슷합니다.

### 11. Why should not we update the state directly? 
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

### 12. What is the purpose of callback function as an argument of setState? 
#### (setState에서 callback의 역할은 무엇인가요?)
callback 함수는 setState가 끝난 후 그리고 component 가 re-rendering 된 후 호출됩니다. setState는 비동기적으로 동작합니다. callback 함수는 모든 작업이 마무리된 후 사용됩니다. 

```js
setState({name: 'sudheer'}, () => console.log('The name has updated and component re-rendered'));
```
 
#### Note: callback 함수를 이용하는 것보단 lifecycle 메서드를 이용하는 것이 좋습니다.

### 13. What is the difference of event handling between HTML and React? 
#### (HTML과 React의 이벤트 처리 차이점은 무엇인가요?)
아래는 HTML과 React 의 이벤트처리의 몇 가지 차이점입니다.

HTML 에서는 이벤트 이름이 소문자여야 합니다.

```html
<button onclick="activateLasers()">
```

반면 React는 camelCase 를 사용합니다.

```html
<button onClick={activateLasers}>
```

HTML 에서는 기본 이벤트 동작을 막기위해 false 를 반환할 수 있습니다.

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

### 14. How to bind methods or event handlers in JSX callbacks?
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

### 15. How to pass a parameter to an event handler or callback? 
#### (이벤트 핸들러 또는 콜백에 매개변수를 어떻게 전달하나요?)

arrow function 으로 감싸서 event handler 에게 매개변수를 전달할 수 있습니다.

```js
<button onClick={() => this.handleClick(id)} />
```

위의 방법은 아래와 같이 method 를 사용하는 것과 같습니다

```html
<button onClick={this.handleClick.bind(this, id)} />
```
 
### 16. What are synthetic events in ReactJS? 
#### (React에서의 합성 이벤트는 무엇인가요?)

[synthetic event](https://reactjs.org/docs/events.html) 는 브라우저의 기본 이벤트를 감싼 cross-browser wrapper 입니다. API는 모든 브라우저에서 동작한다는 점을 제외하면, stopPropagation () 및 preventDefault () 를 포함해 브라우저 네이티브 이벤트와 같은 인터페이스를 가지고 있습니다.

### 17. What is inline conditional expressions? 
#### (인라인 조건식은 무엇인가요?)

조건부 표현식을 표현하기 위해 if 문 또는 삼항 연산자를 사용할 수 있습니다. 이런 표현법 외에도 중괄호로 묶은 다음 JS의 논리 연산자 (&&) 를 붙여 JSX 표현식에 포함시킬 수 있습니다.

```html
<h1>Hello!</h1>
 {messages.length > 0 &&
<h2>
  You have {messages.length} unread messages.
</h2>
```

### 18. What is Key and benefit of using it in lists? 
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

### 19. What is the use of create refs? 
#### (ref의 용도는 무엇인가요?)

두 가지의 접근법이 있습니다.

최근에 추가된 접근 방식입니다. [create ref](https://reactjs.org/docs/refs-and-the-dom.html)는 element 요소에 대한 참조를 반환하는데 사용할 수 있습니다. DOM의 요소나 compoennt 에 직접 접근해야 될 경우 유용할 수 있습니다.

### 20. How to create refs? 
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

### 21. What are forward refs?
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

### 22. Which is preferred option with in callback refs and findDOMNode()?
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

### 23. Why are String Refs legacy?
#### (왜 String Refs 는 legacy가 되었나요?)

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

### 24. What is Virtual DOM?
#### (가상돔이란 무엇인가요?)

가상돔이란 in-memory 즉 Real DOM의 메모리상에서의 표현입니다. UI의 표현은 메모리에 유지되고 Render함수와 화면을 표시하는 사이에 Real DOM 과 동기화됩니다. 이런 단계를 reconciliation 라고 부릅니다.

### 25. How Virtual DOM works?
#### [(가상돔은 어떻게 동작하나요?)](https://www.youtube.com/watch?v=BYbgopx44vo)

가상돔은 세 가지의 간단한 단계로 동작합니다.

1. 데이터가 변경될 때 전체 UI 는 가상돔안에서 re-rendered 됩니다.   

![vdom](./public/vdom1.png)

2. 그런 다음 변경되기전 DOM 과 새로운 변경된 DOM 의 변경점을 계산합니다.   

![vdom](./public/vdom2.png)

3. 계산이 완료되면 실제 DOM 에서 계산된 변경점들만 업데이트됩니다.     

![vdom](./public/vdom3.png)

### 26. What is the difference between Shadow DOM and Virtual DOM?
#### (Shadow DOM과 Virtual DOM의 차이점은 무엇인가요?)
Shadow DOM은 web component의 scope 및 CSS scope 지정을 위해 설계된 web browser 기술입니다. Virtual DOM 은 browser API를 기반으로 JS 라이브러리에서 구현되는 개념입니다.

### 27. What is React Fiber?
#### (React Fiber란 무엇인가요?)
React Fiber란 React v16 에서 핵심 알고리즘을 재구현 한것입니다. React Fiber 의 목표는 애니메이션, 레이아웃, 제스처, 작업을 일시정지하고, 중단 또는 재사용, 여러 유형의 업데이트 우선순위 조절, 동시성등 여러 기본사항에 대한 성능을 높이는 것 입니다.

### 28. What is the main goal of React Fiber?
#### (React Fiber의 주요 목표는 무엇인가요?)
React Fiber 의 목표는 애니메이션, 레이아웃, 제스처등의 성능을 높이는 것 입니다. 주요 목적은 incremental rendering 입니다.

**incremental rendering:** 렌더링 작업을 청크로 쪼개고 여러 프레임으로 분산 시키는 기능입니다.

### 29. What are controlled components?
#### (controlled components 란 무엇인가요?)
입력 요소를 제어하는 component를 controlled components 라고 부릅니다. 모든 상태 변경에는 연관된 handler funciton 이 있습니다.

예를 들어, 이름을 대문자로 쓰려면 아래 handleChange을 이용할 수 있습니다.

```js
handleChange(event) {
  this.setState({value: event.target.value.toUpperCase()})
}
```

### 30. What are uncontrolled components?
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

### 31. What is the difference between createElement and cloneElement?
#### (createElement와 cloneElement의 차이점은 무엇인가요?)
UI 의 object representation으로 사용될 react element를 만들기 위해 JSX element 는 React.createElement() 함수로 변환됩니다. cloneElement는 element 를 복사하고 새로운 props 를 전달하는데 사용됩니다.

### 32. What is Lifting State Up in React?
#### (React 에서 Lifting State Up 은 무엇인가요?)
여러 component 들이 동일한 변경 데이터를 공유해야하는 경우 가까운 부모 component 로 state를 올리는 것이 좋습니다. 즉, 두개의 자식 component가 부모에 있는 동일한 데이터를 공유할 때 두개의 자식 component 들은 local state를 유지하는 대신, 부모로 state를 올려야 합니다.

### 33. What are the different phases of component lifecycle?
#### (component 라이프사이클 단계는 무엇이 다른가요?)
라이프 사이클에는 4가지 단계가 있습니다.

1. Initialization: component 는 초기 state 및 props 를 세팅을 준비합니다.
2. Mounting: component 가 브라우저 DOM에 mount 될 준비가 되었습니다. 이 단계에서는 componentWillMount, componentDidMount 를 사용할 수 있습니다.
3. Updating: 새로운 props를 보내거나 state를 업데이트하여 component 를 두가지 방법으로 update 할 수 있습니다. 이 단계에서는 shouldComponentUpdate (), componentWillUpdate () 및 componentDidUpdate 를 사용할 수 있습니다.
4. Unmounting: 브라우저 DOM에서 component 가 필요하지 않을때 mount를 해제시킵니다. 이 단계에서는 componentWillUnmount 를 사용할 수 있습니다.

![lifecycle](./public/phases.png)

### 34. What are the lifecycle methods of React?
#### (React의 lifecycle methods는 무엇인가요?)
- componentWillMount: rendering 전에 실행됩니다.
- componentDidMount: 첫 rendering 후에 실행됩니다. 이 단계에서 모든 AJAX 요청, DOM 또는 State의 update, event listener 가 설정되어야합니다.
- componentWillReceiveProps: 특정 props update가 state 변화를 트리거할 때 실행됩니다.
- shouldComponentUpdate: 컴포넌트의 업데이트 여부를 결정합니다. 기본적으로 return 값은 true 입니다. state 또는 props 가 업데이트 된 후 component 를 render 할 필요가 없을 경우 false를 return 할 수 있습니다. component가 새로운 props를 받으면서 생기는 rerender 을 막을 수 있습니다. 성능을 향상시키는데 좋습니다.
- componentWillUpdate: shouldComponentUpdate에서 true가 반환되었을 때 state & props 의 변화를 확인하고 re-rendering 되기전에 실행합니다.
- componentDidUpdate: 주로 props 나 state 변경에 대한 response 로 DOM을 업데이트할 때 사용됩니다.
- componentWillUnmount: 네트워크 요청을 취소하거나, component와 관련된 모든 event listeners 를 제거하는데 사용됩니다.

### 35. What are Higher-Order components?
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

### 36. How to create props proxy for HOC component?
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

### 37. What is context?
#### (context가 뭔가요?)

Context 는 모든 레벨에 수동으로 props를 전달하지 않고 component tree를 통해 데이터를 전달할 수 있도록 제공해줍니다.
예를 들어, 인증된 유저, locale 설정, UI 테마는 많은 application 들에서 접근해야합니다.  

```js
const {Provider, Consumer} = React.createContext(defaultValue);
```

### 38. What is children prop?
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

### 39. How to write comments in ReactJS?
#### (React에서 주석은 어떻게 쓰나요?)

ReactJS / JSX 에서의 주석은 JavaScript와 유사합니다. 한 줄 및 여러 줄 주석들은 모두 중괄호로 감쌉니다. 

**Single-line comments:**

```jsx
<div>
  {/* Single-line comments */}    // In vanilla JavaScript, the single-line comments are represented by double slash(//)
  Welcome {user}, Let's play React
</div>
```

**Multi-line comments:**

```jsx
<div>
  {/* Multi-line comments for more than
   one line */}
  Welcome {user}, Let's play React
</div>
```

### 40. What is the purpose of using super constructor with props argument?
#### (props argument와 함께 super constructor를 사용하는 목적은 무엇인가요?)
자식 클래스의 constructor 는 super() 메서드가 호출되기 전까지 this 참조 사용할 수 없습니다. es6 의 sub-classes 에서도 동일하게 적용됩니다.
super()에 props를 파라미터로 전달하는 이유는 child constructors에서 this.props로 접근하기 위해서입니다. 

**Passing props**

```js
class MyComponent extends React.Component {
    constructor(props) {
        super(props);

        console.log(this.props);  // Prints { name: 'sudheer',age: 30 }
    }
}
```

**Not passing props:**

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

### 41. What is reconciliation?
#### ([reconciliation](https://reactjs.org/docs/reconciliation.html)란 무엇인가요?)

Component 의 props 또는 state가 변경될 때 React는 새로 반환된 component를 이전에 rendered 된 component와 비교하여 DOM update가 필요한지 결정합니다. 두개의 component가 같지 않을때 React는 DOM을 update합니다. 이를 프로세스 reconciliation 라고합니다.

### 42. How to set state with a dynamic key name?
#### (동적 key name 으로 어떻게 set State를 하나요?)

만약 ES6 나 babel transpiler 사용하여 JSX 코드를 변환하는 경우 computed property names 으로 작업을 할 수 있습니다. 

```js
handleInputChange(event) {
  this.setState({ [event.target.id]: event.target.value })
}
```

### 43. What would be the common mistake of function being called every time the component renders?
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

### 44. Why is it necessary to capitalize component names?
#### (왜 Component 의 이름은 대문자로 표기해야하나요?)

Component 들은 DOM element가 아니기 때문에 대문자 표기가 필요합니다. component들은 constructors입니다. 또한 JSX 에서의 소문자 태그 이름은 component가 아닌 HTML 요소를 나타내기 때문입니다.

### 45. Why React uses className over class attribute?
#### (왜 React 는 class를 사용하지 않고 className 속성을 사용하나요?)

class는 Javascript 의 키워드입니다. JSX는 Javascript 의 확장입니다. 그것이 React가 class 대신 className을 사용하는 이유입니다. classNames prop 로 문자열을 전달하세요

```js
render() {
  return <span className={'menu navigation-menu'}>{'Menu'}</span>
}
```

### 46. What are fragments?
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

### 47. Why fragments are better than container divs?
#### (왜 fragments 가 div 보다 좋나요 ?)

1. Fragments 는 빠르고 DOM node를 만들지 않기 때문에 메모리를 적게 사용합니다. 이것은 매우 크고 깊은 트리에서 이익을 가집니다.  
2. Flexbox 나 CSS Grid과 같은 CSS 메커니즘에는 특별한 부모 - 자식 관계를 가지고 있습니다. 중간에 div 들을 추가하게 된다면 layout을 유지하기 어려워집니다. 
3. DOM Inspector은 덜 복잡합니다.

### 48. What are portals in React?
#### (React 에서 portals은 무엇입니까 ?)

portals 은 상위 Component 의 DOM 계층 구조 외부에 존재하는 DOM 노드로 자식을 render 하는데 권장되는 방법입니다. 

```js
ReactDOM.createPortal(child, container)
```

첫 번째 인자는 렌더링 가능한 React 하위요소 (element, string, fragment) 입니다. 두 번째 인자는 DOM element 입니다.

### 49. What are stateless components?
#### (stateless 컴포넌트는 무엇인가요?)

Component의 동작과 상태가 독립적이라면 stateless component 를 구성할 수 있습니다. stateless component 는 class나 function 을 이용하여 만들 수 있습니다. 
lifecycle hook을 사용해야하는 경우가 아니라면 function component를 사용할 수 있습니다. function component를 사용한다면 많은 이점이 있습니다. 
쓰기, 이해 그리고 테스트가 빠르고 쉽습니다. 

### 50. What are stateful components?
#### (stateful components 는 무엇인가요?)

Component 의 동작이 component의 state에 의존한다면 stateful component라고 부를 수 있습니다. stateful component 는 항상 class components 이고, constructor에서 초기화합니다. 

```js
class App extends Component {
  constructor(props) {
    super(props)
    this.state = { count: 0 }
  }

  render() {
    // ...
  }
}
```

### 51. How to apply validation on props in React?
#### (React에서 Props의 유효성검사를 적용하나요 ?)

Application 이 개발 모드에서 실행될 때 React는 자동으로 component에 설정된 모든 props 들의 유효성을 체크합니다. 타입이 올바르지 않다면 React는 console에 경고 메세지를 생성할 것 입니다. 
성능에 영향이 가기 때문에 production 모드에서는 사용하지 않습니다. 필수 props는 isRequired로 정의됩니다.

정의 된 props 타입

- PropTypes.number
- PropTypes.string
- PropTypes.array
- PropTypes.object
- PropTypes.func
- PropTypes.node
- PropTypes.element
- PropTypes.bool
- PropTypes.symbol
- PropTypes.any

User component 에 대한 PropTypes 를 아래와 같이 정의할 수 있습니다.

```js
import React from 'react'
import PropTypes from 'prop-types'

class User extends React.Component {
  static propTypes = {
    name: PropTypes.string.isRequired,
    age: PropTypes.number.isRequired
  }

  render() {
    return (
      <>
        <h1>{`Welcome, ${this.props.name}`}</h1>
        <h2>{`Age, ${this.props.age}`}</h2>
      </>
    )
  }
}
```

Note: React v15.5 에서 PropType은 React.PropTypes 에서 prop-types 라이브러리로 옮겨졌습니다.

### 52. What are the advantages of React?
#### (React의 장점은 무엇인가요?)

1. 가상 DOM을 이용하여 application 의 성능을 향상시킵니다.
2. JSX는 코드를 읽고 쓰는 것을 쉽게 만들어줍니다.
3. 클라이언트와 서버측 (SSR) 모두 render 됩니다.
4. 오직 view library 이기 때문에 다른 프레임워크들 (Angular, Backbone)과 손쉽게 통합 할 수 있습니다.
5. Jest 와 같은 도구를 사용하여 단위 및 통합테스트를 쉽게 작성할 수 있습니다.

### 53. What are the limitations of React?
#### (React의 한계는 무엇인가요?)

1. React 전체 framework 가 아닌 view를 위한 library 일 뿐입니다.
2. 웹 개발을 처음 접하는 초심자들에게는 학습 곡선이 있습니다.
3. 기존의 MVC framework 에 React 를 합치기 위해서는 몇 가지 추가 구성이 필요합니다.
4. 인라인 템플릿 및 JSX를 사용하면 코드가 복잡해집니다.
5. 과도한 엔지니어링 또는 boilerplate 로 이어지는 작은 components 들이 너무 많습니다.

### 54. What are error boundaries in React v16?
#### (React v16 에서 error boundaries는 무엇인가요?)

Error boundaries 는 하위 component tree 에서 Javascript error 를 catch 하고, 에러를 기록하고, 오류가 발생한 component tree가 아닌 대체 UI를 표현해 주는 component 입니다.

class component 는 componentDidCatch 라는 새로운 lifecycle 메서드를 정의하면 Error boundaries 됩니다

```js
class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props)
    this.state = { hasError: false }
  }

  componentDidCatch(error, info) {
    // Display fallback UI
    this.setState({ hasError: true })
    // You can also log the error to an error reporting service
    logErrorToMyService(error, info)
  }

  render() {
    if (this.state.hasError) {
      // You can render any custom fallback UI
      return <h1>{'Something went wrong.'}</h1>
    }
    return this.props.children
  }
}
```

그 다음 일반 component 로 사용합니다.

```js
<ErrorBoundary>
  <MyWidget />
</ErrorBoundary>
```

### 55. How error boundaries handled in React v15?
#### (React v15 에서는 어떻게 error boundaries 처리하나요?)

React v15 에서는 unstable_handleError 메서드를 사용하여 error boundaries 에 대한 기본적인 지원을 했습니다. React v16에서 componentDidCatch로 이름이 변경되었습니다.

### 56. What are the recommended ways for static type checking?
#### (권장되는 static 한 타입 체크방법은 무엇인가요?)

일반적으로 우리는 React application 에서 타입 검사를 하기 위해 PropTypes library (React.PropTypes를 React v15.5 부터는 prop-types package 로 옮겼습니다)를 사용합니다.
대규모의 코드 베이스에서는 compile time 에서 타입 체크를 하고 자동 완성 기능을 제공해주는 Flow 나 TypeScript 와 같은 static type checkers 를 이용하는 것이 좋습니다. 

### 57. What is the use of react-dom package?
#### (react-dom 패키지의 사용법은 무엇인가요?)

React-dom 패키지는 App의 최상위 레벨에서 사용할 수 있는 DOM-specific 메서드를 제공합니다. 대부분의 Component 들은 이 모듈을 사용할 필요가 없습니다.
패키지의 일부 메서드는 다음과 같습니다. 

- render()
- hydrate()
- unmountComponentAtNode()
- findDOMNode()
- createPortal()

### 58. What is the purpose of render method of react-dom?
#### (React dom의 render 메서드의 목적은 무엇인가요?)

render 메서드는 제공된 컨테이너의 DOM에 React element를 render 하고 Component에 대한 참조를 반환하는데 사용됩니다. 
React element가 이전에 렌더링 되었다면 update 를 수행하고 최근의 변경사항을 반영하기 위해 필요에 따라 DOM을 변경합니다.

```js
ReactDOM.render(element, container[, callback])
```

만약 optional callback 이 제공된다면, callback은 component 가 렌더링되거나 업데이트 된 후에 실행됩니다.

### 59. What is ReactDOMServer?
#### (ReactDOMServer 란 무엇인가요?)

ReactDOMServer 객체를 사용하면 component를 static markup(일반적으로 노드 서버에서 사용됩니다.) 으로 렌더링 할 수 있습니다.
이 객체는 주로 서버사이드 렌더링(SSR) 에서 사용됩니다. 다음의 메서드는 서버 및 브라우저 환경 모두 사용할 수 있습니다.

- renderToString()
- renderToStaticMarkup()

예를들어 Express, Hapi, Koa 같은 노드 기반의 웹서버를 실행할때 renderToString을 호출하여 root component 를 문자열로 렌더링 한 다음 response를 보낼 수 있습니다

```js
// using Express
import { renderToString } from 'react-dom/server'
import MyPage from './MyPage'

app.get('/', (req, res) => {
  res.write('<!DOCTYPE html><html><head><title>My Page</title></head><body>')
  res.write('<div id="content">')
  res.write(renderToString(<MyPage/>))
  res.write('</div></body></html>')
  res.end()
})
```

### 60. How to use innerHTML in React?
#### (React에서 innerHTML을 어떻게 사용하나요?)

dangerouslySetInnerHTML 속성은 브라우저 DOM 에서 innerHTML 을 사용하기 위한 React 의 대체 속성입니다.
innerHTML과 마찬가지로 XXS (Cross-Site Scripting) 공격을 고려했을때 브라우저 DOM 에서 이 속성을 사용하는 것은 위험합니다.
__html 객체를 키로 HTML 텍스트를 값으로 전달하면됩니다. 

예제에서 MyComponent는 HTML 마크업을 설정하기 위해 dangerouslySetInnerHTML 속성을 사용하고 있습니다.

```js
function createMarkup() {
  return { __html: 'First &middot; Second' }
}

function MyComponent() {
  return <div dangerouslySetInnerHTML={createMarkup()} />
}
```

### 61. How to use styles in React?
#### (React 스타일을 어떻게 사용하나요?)

style 속성은 CSS 문자열 대신 camelCased 속성의 Javascript 객체를 허용합니다. 이것은 DOM Style Javascript 속성과 일치하며 효율적이고, XSS 보안의 허점을 방지할 수 있습니다.

```js
const divStyle = {
  color: 'blue',
  backgroundImage: 'url(' + imgUrl + ')'
};

function HelloWorldComponent() {
  return <div style={divStyle}>Hello World!</div>
}
```

Style의 key는 Javascript DOM Node (예 : node.style.backgroundImage)의 속성에 접근하는 것과 일관되게 하기 위해 camelCased 를 사용합니다. 
 
### 62. How events are different in React?
#### (React 에서 이벤트는 어떻게 다른가요?)

React element 에서의 이벤트 처리는 몇가지 문법상 차이점이 있습니다.

- React 이벤트 핸들러는 소문자보다는 camelCase 를 사용합니다.
- JSX 에서는 문자열이 아닌 이벤트 핸들러를 통해 function 을 전달합니다.

### 63. What will happen if you use setState() in constructor?
#### (constructor 에서 setState를 사용하면 무슨일이 생기나요? )

setState() 를 사용할 때 객체 상태가 할당되고 또한 component 와 모든 자식들을 재렌더링 합니다. 
이런 에러를 봤을겁니다. `Can only update a mounted or mounting component`. 그래서 우리는 this.state 를 사용하여 constructor 내부의 변수를 초기화 해야합니다.

### 64. What is the impact of indexes as keys?
#### (index 가 key 로 미치는 영향은 무엇인가요?)

React element 가 추적할 수 있도록 key 는 안정적, 예측가능, 고유 하여야합니다.
아래 코드 조각에서의 각 element 의 key 는 데이터를 따르지 않고 순서에 따라 결정됩니다. 
이것은 React 가 할 수 있는 최적화를 제한합니다.

```js
{todos.map((todo, index) =>
  <Todo
    {...todo}
    key={index}
  />
)}
```

만약 element 에 data 의 고유한 키값을 사용한다면, todo.id 가 목록에서 고유하고, 안정적이라고 가정한다면 React 는 elements 를 재평가 할 필요없이 element 를 재정렬 할 수 있습니다. 

```js
{todos.map((todo) =>
  <Todo {...todo}
    key={todo.id} />
)}
```

### 65. Is it good to use setState() in componentWillMount() method?
#### (componentWillMount 에서 setState를 사용하는게 좋나요 ?)

`componentWillMount` 안에서는 비동기적인 초기화는 피하는 것이 좋습니다. 
`componentWillMount` 는 마운트가 실행되기 직전에 호출됩니다. 
render () 전에 호출되기 때문에 상태를 설정하더라도 re-render 되지 않습니다.
`componentWillMount` 에서는 side-effects or subscriptions 을 피해야합니다.
우리는 `componentWillMount` 대신 `componentDidMount` 에서 component 초기화를 위한 비동기 호출을 실행해야 합니다.

```js
componentDidMount() {
  axios.get(`api/todos`)
    .then((result) => {
      this.setState({
        messages: [...result.data]
      })
    })
}
```

### 66. What will happen if you use props in initial state?
#### (state 의 초기상태에서 props 를 사용하면 어떻게되나요?)

만약 component 를 새로 고치지 않고 component 의 props 를 변경한다면 생성자 함수가 component 의 현재 상태를 업데이트 하지 않습니다. 
새로운 props 의 값이 표시되지 않습니다. state 의 초기화는 component 를 처음 만들 때만 실행됩니다.

 아래의 component 는 업데이트 된 input 의 값을 표시하지 않습니다.
 
 ```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)

    this.state = {
      records: [],
      inputValue: this.props.inputValue
    };
  }

  render() {
    return <div>{this.state.inputValue}</div>
  }
}
```

render 메소드 안에서 props 를 사용하면 값이 업데이트 됩니다.

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)

    this.state = {
      record: []
    }
  }

  render() {
    return <div>{this.props.inputValue}</div>
  }
}
```

### 67. How do you conditionally render components?
#### (조건에 따른 component 렌더링은 어떻게 하나요 ?)

경우에 따라서 state 에 의존하여 다르게 component 를 렌더링 하기를 원할것이다.
JSX 는 false 또는 undefined 때는 렌더링하지 않으므로 조건을 사용하여 특정 조건이 true 인 경우에만 
component의 특정 부분을 렌더링 할 수 있습니다.

```js
const MyComponent = ({ name, address }) => (
  <div>
    <h2>{name}</h2>
    {address &&
      <p>{address}</p>
    }
  </div>
)
```

만약 if-else 를 사용하기를 원한다면 삼항연산자를 쓰세요 

```js
const MyComponent = ({ name, address }) => (
  <div>
    <h2>{name}</h2>
    {address
      ? <p>{address}</p>
      : <p>{'Address is not available'}</p>
    }
  </div>
)
```

### 68. Why we need to be careful when spreading props on DOM elements?
#### (DOM element 에 props 를 spreading  할때 왜 조심해야 하나요?)

props 를 spreading 할 때 알려지지않은 HTML 속성을 추가 할 위험이 있습니다. 그것은 좋지않습니다.
대신 ...rest 연산자를 사용하여 prop destructuring 을 할 수 있으므로 필요한 props 만 추가할 수 있습니다.

 ```js
const ComponentA = () =>
  <ComponentB isDisplay={true} className={'componentStyle'} />

const ComponentB = ({ isDisplay, ...domProps }) =>
  <div {...domProps}>{'ComponentB'}</div>
```

### 69. How you use decorators in React?
#### (React 에서 decorators 는 어떻게 사용하나요?)

Class component 를 하나의 function 으로 변환하는 방식으로 decorate 할 수 있습니다.
Decorators 는 component 의 기능을 수정하기 위한 유연하고 읽기 쉬운 방법입니다.

```js
@setTitle('Profile')
class Profile extends React.Component {
    //....
}

const setTitle = (title) => (WrappedComponent) => {
  return class extends React.Component {
    componentDidMount() {
      document.title = title
    }

    render() {
      return <WrappedComponent {...this.props} />
    }
  }
}
```

NOTE: Decorators 는 ES7 에 포함되지 않았습니다. 현재 stage 2 에 제안되어 있습니다.

### 70. How do you memoize a component?
#### (memoize component 는 어떻게 사용하나요?)

function component 에 사용할 수 있는 memoize 라이브러리가 있습니다.
예를 들면 `moize` 라이브러리는 다른 component 에 component 를 memoize 할 수 있습니다.

```js
import moize from 'moize'
import Component from './components/Component' // this module exports a non-memoized component

const MemoizedFoo = moize.react(Component)

const Consumer = () => {
  <div>
    {'I will memoize the following entry:'}
    <MemoizedFoo/>
  </div>
}
```

### 71. How you implement Server Side Rendering or SSR?
#### (Server Side Rendering(SSR) 을 어떻게 구현하나요?)

React 는 이미 Node 서버에서 렌더링을 처리할 수 있도록 준비되어 있습니다.
특수한 버전의 DOM renderer 를 사용할 수 있으며, client side 와 동일한 패턴을 따릅니다.


```js
import ReactDOMServer from 'react-dom/server'
import App from './App'

ReactDOMServer.renderToString(<App />)
```

이 method 는 HTML 을 문자열로 내보내고, 문자열은 서버 응답의 일부로 페이지 본문 내부에 배치 할 수 있습니다.
client side 에서 React 는 이미 렌더링된 content 를 감지하여 중단된 부분을 원활히 처리합니다.


### 72. How to enable production mode in React?
#### (React에서 어떻게 production 모드를 활성화 하나요)

Webpack 의 DefinePlugin 메서드를 사용하여 NODE_ENV 를 production 으로 설정해야
propType 의 유효성 검사 및 추가적인 경고 같은 것들을 제거할 수 있습니다.

production 모드와는 별도로 코드를 minify 하면 Uglify 의 dead-code 의 제거와 주석을 제거하여 bundle 크기를 줄일 수 있습니다.

 
### 73. What is CRA and its benefits?
#### (CRA는 무엇이고 CRA의 이점은 무엇인가요?)

Create-Reaction-App CLI 사용하면 설정 단계 없이 React applications 생성하고 실행할 수 있습니다.

CRA 를 사용하여 Todo App 을 만듭니다

```bash
# Installation
$ npm install -g create-react-app

# Create new project
$ create-react-app todo-app
$ cd todo-app

# Build, test and run
$ npm run build
$ npm run test
$ npm start
```

### 74. What is the lifecycle methods order in mounting?
#### (마운팅에서 lifecycle 메서드의 순서는 무엇인가요?)

lifecycle 메서드는 component 의 instance 가 생성되어 DOM에 삽입 될 때 호출됩니다.

- constructor()
- static getDerivedStateFromProps()
- render()
- componentDidMount()

### 75. What are the lifecycle methods going to be deprecated in React v16?
#### (React v16 에서 사용되지 않을 lifecycle 메서드는 무엇인가요?)

안전하지 않은 코딩 방법이 될 수 있는 lifecycle 메서드는 비동기적으로 렌더링시 문제가 될 것 입니다. 

- componentWillMount()
- componentWillReceiveProps()
- componentWillUpdate()

React v16.3 부터는 UNSAFE_가 prefix 붙고, prefix 가 없는 버전은 React v17 에서 제거됩니다.

### 76. What is the purpose of getDerivedStateFromProps() lifecycle method?
#### (getDerivedStateFromProps() lifecycle 메서드의 목적은 무엇인가요?)

새로운 정적 getDerivedStateFromProps() lifecycle 메서드는 component 가 인스턴스화 된 후, 다시 렌더링 되기 전에 호출됩니다.  
object 를 반환하여 state 를 update 하거나, null 을 반환하여 새로운 props 에서 state update 가 필요하지 않음을 나타낼 수 있습니다.

```js
class MyComponent extends React.Component {
  static getDerivedStateFromProps(props, state) {
    // ...
  }
}
```

이 lifecycle 메서드는 componentDidUpdate() 와 함께 componentWillReceiveProps() 의 사용 사례에 적용할 수 있습니다.

### 77. What is the purpose of getSnapshotBeforeUpdate() lifecycle method?
#### (getSnapshotBeforeUpdate() lifecycle 메서드의 목적은 무엇인가요?)

새로운 [getSnapshotBeforeUpdate()](https://reactjs.org/docs/react-component.html#getsnapshotbeforeupdate) lifecycle 메서드는 DOM update 직전에 호출됩니다. 
이 메서드의 반환값은 componentDidUpdate() 의 세번째 파라미터로 전달됩니다.

```js
class MyComponent extends React.Component {
  getSnapshotBeforeUpdate(prevProps, prevState) {
    // ...
  }
}
```

이 lifecycle 메서드는 componentDidUpdate()와 함께 componentWillUpdate () 의 사용 사례에 적용할 수 있습니다.

### 78. What is the difference between createElement() and cloneElement() methods
#### (createElement() 와 cloneElement() 의 차이점은 무엇인가요?)

JSX 에서 React element 는 UI element 를 타내는 React.createElement() 변환됩니다.  
React.cloneElement ()는 element 를 복제하고 새로운 props를 전달하는데 사용됩니다.

### 79. What is the recommended way for naming components?
#### (component 의 이름을 지정하는 권장방법은 무엇인가요?)

displayName 대신 reference 를 이용하여 component 의 이름을 정하는 것을 추천한다.

displayName 사용
```js
export default React.createClass({
  displayName: 'TodoApp',
  // ...
})
```

추천 방법:
```js
export default class TodoApp extends React.Component {
  // ...
}
```

### 80. What is the recommended ordering of methods in component class?
#### (component class 안에서 메서드의 추천 순서는 무엇인가요?)

마운트에서 부터 렌더링 단계까지의 권장 메서드 지정 순서  

- static methods
- constructor()
- getChildContext()
- componentWillMount()
- componentDidMount()
- componentWillReceiveProps()
- shouldComponentUpdate()
- componentWillUpdate()
- componentDidUpdate()
- componentWillUnmount()
- click handlers or event handlers like onClickSubmit() or onChangeDescription()
- getter methods for render like getSelectReason() or getFooterContent()
- optional render methods like renderNavigation() or renderProfilePicture()
- render()

### 81. What is a switching component?
#### (switching component 란 무엇인가요?)

switching component는 여러 component 중 하나의를 렌더링 하는 component 입니다. 우리는 props 값을 매핑하기 위해 object 를 사용해야합니다. 

예를 들어, switching component 는 페이지의 props 를 기반으로 다른 component 를 보여줍니다.

```js
import HomePage from './HomePage'
import AboutPage from './AboutPage'
import ServicesPage from './ServicesPage'
import ContactPage from './ContactPage'

const PAGES = {
  home: HomePage,
  about: AboutPage,
  services: ServicesPage,
  contact: ContactPage
}

const Page = (props) => {
  const Handler = PAGES[props.page] || ContactPage

  return <Handler {...props} />
}

// The keys of the PAGES object can be used in the prop types to catch dev-time errors.
Page.propTypes = {
  page: PropTypes.oneOf(Object.keys(PAGES)).isRequired
}
```

### 82. Why we need to pass a function to setState()?
#### (왜 setState 에 함수를 전달해야하나요?)

이유는 setState 가 비동기적인 작업이기 때문입니다. 성능상의 이유로 state 의 변경은 일괄적으로 일어납니다, 그래서 setState() 의 호출 직후에 state가 변경되지 않을 수 있습니다.   
state 를 확실할 수 없기 때문에 setState()를 호출 할 때 현재의 state에 의존하면 안됩니다.  
해결책은 이전 state를 인자로 사용하는 setState()에 함수를 전달하는 것입니다.    
그렇게 하면 setState()가 가진 비동기성으로 인해 사용자가 접근할때 이전 state의 값을 가져오는 문제를 피할 수 있습니다. 

초기의 count 값이 0 이라고 가정하겠습니다. 세번의 증가연산 후의 값은 오직 1만 증가합니다.

```js
// assuming this.state.count === 0
this.setState({ count: this.state.count + 1 })
this.setState({ count: this.state.count + 1 })
this.setState({ count: this.state.count + 1 })
// this.state.count === 1, not 3
```

setState() 에 함수를 전달하면 올바르게 증가합니다.

```js
this.setState((prevState, props) => ({
  count: prevState.count + props.increment
}))
// this.state.count === 3 as expected
```

### 83. What is strict mode in React?
#### (React 에서 strict mode 는 무엇인가요?)

React.StrictMode 는 application 의 잠재적인 문제를 강조 표시하는데 유용한 component 입니다. `<Fragment>`처럼, `<StrictMode>` 도 추가적으로 DOM을 렌더링하지 않습니다. 
자식에 대한 추가적인 확인과 경고를 활성화합니다. 검사는 개발 모드에만 적용됩니다.  

```js
import React from 'react'

function ExampleApplication() {
  return (
    <div>
      <Header />
      <React.StrictMode>
        <div>
          <ComponentOne />
          <ComponentTwo />
        </div>
      </React.StrictMode>
      <Footer />
    </div>
  )
}
```

위의 예제에서 strict mode 는 <ComponentOne /> 와 <ComponentTwo /> 에만 적용됩니다.      
`<StrictMode>` 는 다음과 같은 도움을 줍니다. 

- 안전하지 않은 lifecycle 메서드를 식별합니다.
- 레거시 string ref API 에 대한 경고
- 예상치 못한 사이드 이펙트 감지 
- legacy context API 감지
    
    
### 84. What are React Mixins?
#### (React Mixins은 무엇인가요?)

Mixins은 공통적인 기능을 가질 수 있도록 component를 분리하는 방법입니다. Mixins은 사용하지 말아야합니다. higher-order components 또는 decorators 로 대체할 수 있습니다.   
props와 state가 이전의 props 와 state 가 얕게 같을때 불필요한 재 렌더링을 방지하기 위해 component 에서 사용할 수 있습니다.

```js
const PureRenderMixin = require('react-addons-pure-render-mixin')

const Button = React.createClass({
  mixins: [PureRenderMixin],
  // ...
})
``` 

### 85. Why is isMounted() an anti-pattern and what is the proper solution?
#### (왜 isMounted() 가 안티패턴이고 해결책은 무엇인가요?)

isMounted() 의 사용 사례는 component의 마운트가 해제 된 후에 setState()를 호출하지 않도록 하는 것입니다. component 마운트가 해제된 후 경고가 발생되기 때문입니다. 

```js
if (this.isMounted()) {
  this.setState({...})
}
```   

setState() 를 호출하기 전에 isMounted() 를 검사한다면 경고를 제거할 수 있지만, 경고의 목적을 잃어버릴 수 있습니다.
component의 마운트가 해제된 후에 reference 를 가지고 있다고 생각하기 때문에 isMounted()를 사용하는 것은 [code smell](https://ko.wikipedia.org/wiki/%EC%BD%94%EB%93%9C_%EC%8A%A4%EB%A9%9C) 입니다.

최적의 해결법은 component의 마운트가 해제된 후 setState() 가 호출될 수 있는 위치를 찾아 수정하는 것입니다. 
이러한 상황은 component가 데이터를 기다리고 데이터가 도착하기전 마운트가 해제될 때, 콜백으로 인해 많이 발생됩니다.
콜백은 마운트가 해제되기전에 componentWillUnmount 단계에서 취소되어야합니다. 

### 86. What are the Pointer Events supported in React?
#### (React 에서 지원하는 Pointer Events 는 무엇인가요?)

Pointer Events 는 모든 입력 이벤트를 다루는 통일된 방법을 제공합니다. 옛날에는 마우스와 각각 event listeners 를 다뤘지만, 
요즘에는 터치스크린, 펜이 있는 휴대전화와 같이 마우스와 상관이 없는 많이 장치가 있습니다. 
이런 이벤트들은 Pointer Events 를 지원하는 브라우저에서만 동작하는 것을 기억해야합니다.

React DOM 에서는 다음과 같은 event 를 사용할 수 있습니다.

- onPointerDown
- onPointerMove
- onPointerUp
- onPointerCancel
- onGotPointerCapture
- onLostPointerCaptur
- onPointerEnter
- onPointerLeave
- onPointerOver
- onPointerOut

### 87. Why should component names start with capital letter?
#### (왜 Component 의 이름은 대문자로 시작해야하나요?)

만약 JSX 를 사용하여 component 를 렌더링하는 경우 component 의 이름은 대문자로 시작하여야 합니다. 
그렇지 않으면 React 는 알 수 없는 태그로 인식하여 오류가 발생될 것 입니다.
이 규칙은 HTML 과 SVG 태그만 소문자로 시작할 수 있기 때문에 사용됩니다.

이름이 소문자로 시작하는 component class 를 정의할 수 있지만 가져올떄는 대문자여야 합니다.    

여기 소문자는 괜찮습니다.

```js
class myComponent extends Component {
  render() {
    return <div />
  }
}

export default myComponent
```

다른 파일에서 가져올때는 대문자로 시작해야합니다.

```js
import MyComponent from './MyComponent'
```

### 88. Are custom DOM attributes supported in React v16?
#### (React v16 에서 사용자 정의 DOM 속성이 지원되나요?)

네 지원됩니다. 과거 React 는 알려지지 않은 DOM 속성은 무시되었었습니다. 
React 가 인식하지 못하는 속성을 가진 JSX 를 작성한다면 React 는 건너뛸 것 입니다. 

예를 들면 다음과 같습니다.

```js
<div mycustomattribute={'something'} />
```

React v15 에서 빈 div 를 DOM 에 렌더링합니다.

```js
<div />
```

React v16 에서 알 수 없는 속성은 DOM 에 포함됩니다. 

```js
<div mycustomattribute='something' />
```

이 기능은 브라우저 별로 비표준 속성을 제공하고, 새로운 DOM API 를 시도, 다른 라이브러리와 같이 사용할 때 유용합니다.

### 89. What is the difference between constructor and getInitialState?
#### (constructor 와 getInitialState의 차이점은 무엇인가요?)

ES6 클래스를 사용할 떄는 constructor에서 state를 초기화할 수 있고, React.createClass 를 사용할 때는 getInitialState() 에서 상태를 초기화해야합니다.  
 
ES6 클래스 사용:

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.state = { /* initial state */ }
  }
}
```
React.createClass() 사용:

```js
const MyComponent = React.createClass({
  getInitialState() {
    return { /* initial state */ }
  }
})
```

**Note**: React.createClass() 는 이제 사용되지 않고, React v16 에서 제거됩니다. 대신 JS class 를 사용하세요 

### 90. Can you force a component to re-render without calling setState?
#### (setState 를 호출하지 않고 component 를 강제로 재 렌더링 시킬 수 있나요?)

기본적으로, component 의 state 또는 props 가 변경되면 component 는 다시 렌더링됩니다. 
render() 메소드가 다른 data 에 의존성이 있는 경우, forceUpdate() 를 호출하여 component에게 다시 렌더링이 필요하다고 알려줄 수 있습니다. 

```js
component.forceUpdate(callback)
```

forceUpdate() 의 사용은 피하고 render() 안의 this.props 와 this.state 는 읽는 용도로 사용하는 것이 좋습니다.

### 91. What is the difference between super() and super(props) in React using ES6 classes?
#### ES6 class 를 사용하는 React 에서 super() 와 super(props) 의 차이점은 무엇인가요?

constructor() 에서 this.props 에 접근하고 싶을때 super() 메서드에 props 를 전달해야합니다.

**super(props)를 사용:**

```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    console.log(this.props) // { name: 'John', ... }
  }
}
```

**super() 를 사용:**

```js
class MyComponent extends React.Component {
  constructor(props) {
    super()
    console.log(this.props) // undefined
  }
}
```

constructor() 의 밖에서의 this.props 에는 같은 값이 표시됩니다.

### 92. How to loop inside JSX?
#### 어떻게 JSX 안에서 loop 를 하나요?

ES6 arrow function 과 함께 Array.prototype.map 를 사용할 수 있습니다. 예를 들어, 객체의 items 배열은 component 의 배열로 맵핑됩니다.

```js
<tbody>
  {items.map(item => <SomeComponent key={item.id} name={item.name} />)}
</tbody>
```

for loop 를 사용하여 반복할 수 없습니다.

```js
<tbody>
  for (let i = 0; i < items.length; i++) {
    <SomeComponent key={items[i].id} name={items[i].name} />
  }
</tbody>
```

JSX 태그는 함수 호출로 변환되어지기 떄문에 표현식 안에서 JS 표현법을 사용할 수 없습니다.
이것은 stage 1 에 제안되어 변경되어질 수 있습니다.

### 93. How do you access props in attribute quotes?
#### (attribute 따옴표에서 props 에 어떻게 접근하나요?)

React (또는 JSX) 는 속성 값 안에 써넣은 값은 지원되지 않습니다. 아래의 표현식은 동작하지 않습니다. 

```js
<img className='image' src='images/{this.props.image}' />
```

그러나 중괄호 안에 JS 표현식을 감싸 속성 값으로 넣을 수 있습니다. 아래의 표현식은 동작합니다.

```js
<img className='image' src={'images/' + this.props.image} />
```

템플릿 문자열을 사용해도 동작합니다.

```js
<img className='image' src={`images/${this.props.image}`} />
```

### 94. What is React proptype array with shape?

특정 모양을 가진 component 에 객체 배열을 전달하고 싶다면 React.PropTypes.arrayOf()의 인자로 React.PropTypes.shape() 를 사용하세요

```js
ReactComponent.propTypes = {
  arrayWithShape: React.PropTypes.arrayOf(React.PropTypes.shape({
    color: React.PropTypes.string.isRequired,
    fontSize: React.PropTypes.number.isRequired
  })).isRequired
}
```

### 95. How conditionally apply class attributes?
#### (어떻게 조건에 따라 class 속성을 적용하나요?)

따옴표안에 중괄호를 사용하면 string 으로 인식되기 때문에 중괄호를 사용하면 안됩니다.

```js
<div className="btn-panel {this.props.visible ? 'show' : 'hidden'}">
```

중괄호 밖으로 옮겨야 합니다. (class 의 이름 사이에 공백을 포함하는 것을 잊으면 안됩니다.)

```js
<div className={'btn-panel ' + (this.props.visible ? 'show' : 'hidden')}>
```

템플릿 문자열을 사용해도 동작합니다.

```js
<div className={`btn-panel ${this.props.visible ? 'show' : 'hidden'}`}>
```

### 96. What is the difference between React and ReactDOM?
#### (React와 ReactDOM은 무엇이 다른가요?)

React package 에는 React.createElement (), React.Component, React.Children 및 element 와 component class 관련된 helper 들이 포함되어 있습니다.
이런 기능들은 component 를 구축하는데 필요한 helpers 로 생각할 수 있습니다.
react-dom package 에는 ReactDOM.render () 가 포함되어있고, react-dom/server 에는 ReactDOMServer.renderToString() 과 ReactDOMServer.renderToStaticMarkup() 포함되어있어 서버사이드 렌더링을 지원합니다.

### 97. Why ReactDOM is separated from React?
#### (왜 React 와 ReactDOM은 분리되어있나요?)

React 팀은 모든 DOM 과 관련된 기능들을 ReactDOM 이라는 라이브러리로 분리하였습니다. 
React v0.14 는 ReactDOM 이 분리된 첫번째 릴리즈입니다.
React-native, Reaction-Art, Reaction-Canvas, React-3 등 패키지의 일부를 보면 React 의 아름다움과 본질적인 부분이 브라우저나 DOM 과 아무런 관계가 없다는 것을 알 수 있습니다.
React 가 렌더링할 수 있는 많은 환경들을 만들기 위해, React 팀은 React 와 React-dom 을 분리할 계획을 세웠습니다.
이것은 웹 버전의 React 와 React native 사이의 공유할 수 있는 component 를 작성하는 방법을 개척합니다.

### 98. How to use React label element?
#### (React 에서 label element 를 어떻게 사용하나요?)

표준 `for` 속성을 사용하는 text input 에 바인드된 label element 를 렌더링하려고하면 속성이없는 HTML이 생성되고 console 에 경고가 출력됩니다.

```js
<label for={'user'}>{'User'}</label>
<input type={'text'} id={'user'} />
```

for 는 JS 의 예약된 키워드입니다, 대신 htmlFor 를 사용하세요 

```js
<label htmlFor={'user'}>{'User'}</label>
<input type={'text'} id={'user'} />
```

### 99. How to combine multiple inline style objects?
#### (어떻게 여러개의 inline style object 를 합치나요?)

React 에서 spread operator 를 사용할 수 있습니다.

```js
<button style={{...styles.panel.button, ...styles.panel.submitButton}}>{'Submit'}</button>
```

React Native 를 사용하고 있다면 배열 표기법을 사용할 수 있습니다.

```js
<button style={[styles.panel.button, styles.panel.submitButton]}>{'Submit'}</button>
```

### 100. How to re-render the view when the browser is resized?
#### (어떻게 브라우저가 resize 될 때 재 렌더링 시키나요?)

componentDidMount() 에서 resize 이벤트를 listen 할 수 있고, 크기(width, height)를 update 할 수 있습니다. 
componentWillUnmount() 에서 listener 를 제거해줘야합니다.
 
```js
class WindowDimensions extends React.Component {
  componentWillMount() {
    this.updateDimensions()
  }

  componentDidMount() {
    window.addEventListener('resize', this.updateDimensions)
  }

  componentWillUnmount() {
    window.removeEventListener('resize', this.updateDimensions)
  }

  updateDimensions() {
    this.setState({width: $(window).width(), height: $(window).height()})
  }

  render() {
    return <span>{this.state.width} x {this.state.height}</span>
  }
}
```

### 101. What is the difference between setState() and replaceState() methods?
#### (setState() 와 replaceState() 의 차이점은 무엇인가요?)

setState() 를 사용하면 이전 state 와 다음 state 가 병합됩니다. replaceState()는 현재 state 를 버리고 당신이 제공한 state 로 바꿉니다.
이전의 key 들을 모두 제거해야되는 경우가 아니라면 보통 setState() 가 사용됩니다.
replaceState()를 사용하는 대신 setState()에서 state 를 flase/null 로 설정할 수 있습니다.

### 102. How to listen to state changes?
#### (어떻게 state 의 변경을 listen 하나요?)

state 가 변경될때 다음의 lifecycle 메서드들이 호출됩니다.
이전에 제공된 state 와 props 의 값을 현재의 state와 props와 비교하여 의미있는 변화가 있는지 확인할 수 있습니다.

```js
componentWillUpdate(object nextProps, object nextState)
componentDidUpdate(object prevProps, object prevState)
```

### 103. What is the recommended approach of removing an array element in React state?
#### (React state 에서 배열요소를 제거하는 추천방법은 무엇인가요?)

좋은 방법은 Array.prototype.filter() 메서드를 사용하는 것입니다.

예를 들어, state update를 위한 removeItem () 메서드를 만들겠습니다.

```js
removeItem(index) {
  this.setState({
    data: this.state.data.filter((item, i) => i !== index)
  })
}
```

### 104. Is it possible to use React without rendering HTML?
#### (HTML 렌더링 없이 React를 사용할 수 있나요?)

latest version (최신버전 >= 16.2) 부터 가능합니다. 가능한 옵션은 다음과 같습니다.

```js
render() {
  return false
}
```

```js
render() {
  return null
}
```

```js
render() {
  return []
}
```

```js
render() {
  return <React.Fragment></React.Fragment>
}
```

```js
render() {
  return <></>
}
```

### 105. How to pretty print JSON with React?
#### (React와 함께 어떻게 이쁘게 JSON 을 print 하나요?)

`<pre>` 태그를 사용하여 JSON.stringify() 형식이 유지되도록 할 수 있습니다.

```js
const data = { name: 'John', age: 42 }

class User extends React.Component {
  render() {
    return (
      <pre>
        {JSON.stringify(data, null, 2)}
      </pre>
    )
  }
}

React.render(<User />, document.getElementById('container'))
```

### 106. Why you can't update props in React?
#### (왜 React에서 props 를 update 할 수 없나요?)

React 의 철학은 props 는 immutable(불변) 이어야하고 top-down (부모 -> 자식) 방식입니다.
부모는 모든 props 값을 자식에게 보낼 수 있지만, 자식은 받은 props 를 변경할 수 없습니다.

### 107. How to focus an input element on page load?
#### (어떻게 페이지 로드시에 input element 에 focus 하나요?)

input element 를 위한 ref 를 생성하여 componentDidMount() 에서 사용하면 됩니다.

```js
class App extends React.Component{
  componentDidMount() {
    this.nameInput.focus()
  }

  render() {
    return (
      <div>
        <input
          defaultValue={'Won\'t focus'}
        />
        <input
          ref={(input) => this.nameInput = input}
          defaultValue={'Will focus'}
        />
      </div>
    )
  }
}

ReactDOM.render(<App />, document.getElementById('app'))
```

### 108. What are the possible ways of updating objects in state?
#### (state 의 object 를 update 할 수 있는 방법은 무엇인가요?)

1. state 와 합쳐질 object 를 사용하여 setState() 호출  
- Object.assign() 을 사용하여 object 의 복사본을 만듭니다.

```js
const user = Object.assign({}, this.state.user, { age: 42 })
this.setState({ user })
```

**spread operator 를 사용:**

```js
const user = { ...this.state.user, age: 42 }
this.setState({ user })
```


**function 을 이용하여 setState() 호출:**

```js
this.setState(prevState => ({
  user: {
    ...prevState.user,
    age: 42
  }
}))
```

### 109. Why function is preferred over object for setState()?
#### (왜 setState()를 위한 function 이 object 보다 선호되나요?)

React 는 성능을 위해 여러 setState() 호출들을 일괄 처리 합니다.
이유는 this.props 와 this.state는 비동기로 update 될 수 있습니다. 다음 state 를 계산할 때 계산된 값을 신뢰하면 안됩니다.

카운터 예제는 기대한대로 update 되지 않습니다.

```js
// Wrong
this.setState({
  counter: this.state.counter + this.props.increment,
})
```

추천되는 접근방법은 object 가 아닌 function 으로 setState() 를 호출하는 것입니다.
function 은 첫번째 인자로 이전 state를 받고 두 번째 인자로 update가 적용될 때의 props 를 받습니다.

```js
// Correct
this.setState((prevState, props) => ({
  counter: prevState.counter + props.increment
}))
```

### 110. How can we find the version of React at runtime in the browser?
#### (브라우저에서 React의 버전을 runtime 시 어떻게 찾을 수 있나요?)

React.version 을 사용하면 버전을 가져올 수 있습니다.

```js
const REACT_VERSION = React.version

ReactDOM.render(
  <div>{`React version: ${REACT_VERSION}`}</div>,
  document.getElementById('app')
)
```

### 111. What are the approaches to include polyfills in your create-react-app?
#### (create-react-app 에 polyfills를 포함시키는 방법은 무엇인가요?)

**core-js 에서 수동 import:**

- polyfills.js 파일을 만들어 root index.js 에서 import 합니다. `npm install core-js` 또는 `yarn add core-js` 를 추가하고 필요한 기능을 import 합니다.

```js
import 'core-js/fn/array/find'
import 'core-js/fn/array/includes'
import 'core-js/fn/number/is-nan'
```

**Polyfill 서비스 사용:**

- polyfill.io CDN 을 사용하여 다음의 줄을 index.html 에 추가하고, 사용자 지정 브라우저별 Polyfill을 검색합니다.

```js
<script src='https://cdn.polyfill.io/v2/polyfill.min.js?features=default,Array.prototype.includes'></script>
```

위의 스크립트에서 Array.prototype.includes 는 기본 스펙에 포함되지 않았기 때문에 기능을 요청했습니다.

### 112. How to use https instead of http in create-react-app?
#### (create-react-app 에서 http 대신 https 를 어떻게 사용하나요?)

`HTTPS = true` 설정이 필요합니다.  package.json 에 scripts 부분을 편집할 수 있습니다.

```js
"scripts": {
  "start": "set HTTPS=true && react-scripts start"
}
```

또는 `set HTTPS=true && npm start` 을 실행하세요

### 113. How to avoid using relative path imports in create-react-app?
#### (create-react-app 에서 상대경로 import 를 어떻게 피하나요?)

프로젝트의 root 에 `env` 파일을 만들고 import path 를 작성해주세요.

```js
NODE_PATH=src/app
```

설정후 개발서버를 재시작 해주세요. 상대 경로없이 src/app 안에 있는 모든것을 import 할 수 있습니다.

### 114. How to add Google Analytics for React Router?
#### (어떻게 React Router 에 Google Analytics 를 추가하나요?)

history 객체에 listener 를 추가하여 각 페이지 뷰를 기록하세요.

```js
history.listen(function (location) {
  window.ga('set', 'page', location.pathname + location.search)
  window.ga('send', 'pageview', location.pathname + location.search)
})
```

### 115. How to update a component every second?
#### (어떻게 매 초 마다 component 를 업데이트 하나요?)

setInterval() 를 사용하여 변경을 트리거해야합니다. 오류 및 메모리 누수를 방지하려면 component unmount 시 타이머를 제거해야합니다.

```js
componentDidMount() {
  this.interval = setInterval(() => this.setState({ time: Date.now() }), 1000)
}

componentWillUnmount() {
  clearInterval(this.interval)
}
```

### 116. How do you apply vendor prefixes to inline styles in React?
#### (React 에서 어떻게 인라인 스타일에 vendor prefixes 를 붙일수 있나요?)

React 에서는 [vendor prefixes](https://developer.mozilla.org/en-US/docs/Glossary/Vendor_Prefix) 를 자동으로 적용해주지 않습니다. vendor prefixes 를 수동으로 추가해야합니다.

```jsx harmony
<div style={{
  transform: 'rotate(90deg)',
  WebkitTransform: 'rotate(90deg)', // note the capital 'W' here
  msTransform: 'rotate(90deg)' // 'ms' is the only lowercase vendor prefix
}} />
```
 
### 117. How to import and export components using React and ES6?
#### (React와 ES6에서 어떻게 component 를 import 와 export 할 수 있나요?)

component 를 export 하려면 default 를 사용해야합니다.

```jsx harmony
import React from 'react'
import User from 'user'

export default class MyProfile extends React.Component {
  render(){
    return (
      <User type="customer">
        //...
      </User>
    )
  }
}
``` 

export 를 사용하면 MyProfile 이 모듈로 내보내집니다. 다른 component 의 이름을 사용하지 않아도 동일한 파일을 import 할 수 있습니다.

### 118. Why React component names must begin with a capital letter?
#### (왜 React compnent 의 이름은 대문자여야하나요?)

JSX 에서 소문자 태그 이름은 HTML 태그로 간주됩니다. 그러나 점 ((property accessors) 이 있는 대문자, 소문자 태그 이름은 HTML 태그로 간주되지 않습니다.

- `<component />` compiles to React.createElement('component') (i.e, HTML tag)
- `<obj.component />` compiles to React.createElement(obj.component)
- `<Component />` compiles to React.createElement(Component)

### 119. Why is a component constructor called only once?
#### (왜 component 생성자는 한번만 호출되나요?)

React의 reconciliation  알고리즘에서는 custom component 가 다음 렌더링의 같은 위치에 나타나면 이전 component 와 동일하므로 인스턴스를 새로 만들지 않고 다시 사용한다고 가정합니다.

### 120. How to define constants in React?
##### (React 에서 어떻게 상수를 정의하나요?)

ES7 의 static 필드를 사용하여 상수를 정의 할 수 있습니다.

```js
class MyComponent extends React.Component {
  static DEFAULT_PAGINATION = 10
}
```

static 필드는 statge 3 의 제안된 부분입니다.

### 121. How to programmatically trigger click event in React?
#### (React 에서 어떻게 프로그래밍 방식으로 클릭 이벤트를 트리거 할 수 있나요?)

callback 을 통한 ref prop 를 사용하여 `HTMLInputElement` 객체에 대한 참조를 가져와 class property 로 저장하고,
나중에 저장된 참조를 사용를 이용하여 `HTMLElement.click` 메서드를 사용해 이벤트 핸들러에서 클릭 이벤트를 트리거 할 수 있습니다.  

이 작업은 두 단계로 나눌 수 있습니다.

**render 메서드 안에서 ref 생성**
 
```jsx harmony
<input ref={input => this.inputElement = input} />
```

**이벤트 핸들러에서 클릭 이벤트 제공:**

```js
this.inputElement.click()
```

### 122. Is it possible to use async/await in plain React?
#### (기본 React 에서 async/await 를 사용할 수 있나요?)

React 에서 async/await 을 사용하고 싶다면 Babel 과 transform-async-to-generator 플러그인이 필요합니다.

### 123. What are the common folder structures for React?
#### (React 의 일반 폴더 구조는 무엇인가요?)

여기 React project 의 파일 구조에 대한 두 가지의 사례가 있습니다.

**기능 또는 경로별로의 그룹:**

프로젝트를 구조화하는 하나의 일반적인 방법으로는 기능이나 경로별로 그룹화된 CSS, JS, test 들을 함께 구성하는 것입니다.

```text
common/
├─ Avatar.js
├─ Avatar.css
├─ APIUtils.js
└─ APIUtils.test.js
feed/
├─ index.js
├─ Feed.js
├─ Feed.css
├─ FeedStory.js
├─ FeedStory.test.js
└─ FeedAPI.js
profile/
├─ index.js
├─ Profile.js
├─ ProfileHeader.js
├─ ProfileHeader.css
└─ ProfileAPI.js
```

**파일 형식의 그룹화**

프로젝트를 구조화하는 다른 인기있는 방법으로는 유사한 파일들을 그룹화하는 것입니다.

```text
api/
├─ APIUtils.js
├─ APIUtils.test.js
├─ ProfileAPI.js
└─ UserAPI.js
components/
├─ Avatar.js
├─ Avatar.css
├─ Feed.js
├─ Feed.css
├─ FeedStory.js
├─ FeedStory.test.js
├─ Profile.js
├─ ProfileHeader.js
└─ ProfileHeader.css
```

### 124. What are the popular packages for animation?
#### (애니메이션을 위한 인기있는 패키지는 무엇인가요?)

React 생태계에서 인기있는 애니메이션 패키지는 React Transition Group과 React Motion 입니다.

### 125. What is the benefit of styles modules?
#### (styles modules 의 이점은 무엇인가요?)

styles modules 은 component 에서 style 의 값을 하드 코딩하는 것을 피하기 위해 추천됩니다. 
서로 다른 UI component 에서 사용될 수 있는 값들은 자체 모듈에서 받아와야 합니다.

예를 들어, 이런 style 들은 별도의 component 로 받아낼 수 있습니다.

```js
export const colors = {
  white,
  black,
  blue
}

export const space = [
  0,
  8,
  16,
  32,
  64
]
```
 
다른 component 들에서 개별적으로 가져올 수 있습니다.  

```
import { space, colors } from './styles'
```

### 126. What are the popular React-specific linters?
#### (인기있는 React linters 는 무엇인가요?)

ESLint 는 인기있는 Javascript linters 입니다. ESLint 는 코드 스타일을 분석할 수 있는 플러그인입니다.
React 에서 대부분 사용하는 npm 패키지 중 하나는 `eslint-plugin-react` 입니다.
기본적으로 몇가지의 best practices 를 확인하여 규칙을 바탕으로 iterators 의 key 에서 전체 prop type 까지 확인합니다.
다른 인기있는 플러그인은 `eslint-plugin-jsx-a11y` 이며, 접근성을 통해 문제를 해결하는데 도움을 줍니다.
JSX 는 일반적인 HTML 문법과 약간 다르게 제공하므로, `alt` text 그리고 `tabindex` 같은 문제는 플러그인으로 선택되지 않습니다.

### 127. How to make AJAX call and in which component lifecycle methods should I make an AJAX call?
#### (어떻게 AJAX 를 호출하고 어떤 lifecycle 에서 메서드를 호출해야하나요?)

AJAX 라이브러리인 Axios, jQuery AJAX, 그리고 브라우저에 내장된 fetch 를 사용할 수 있습니다.
`componentDidMount()` lifecycle 메서드에서 데이터를 불러와야합니다.
setStaet() 를 사용하여 데이터를 검색할때 component 를 update 할 수 있습니다.

예를 들어, API 에서 직원목록을 가져와 local state 를 설정합니다:

```jsx harmony
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.state = {
      employees: [],
      error: null
    }
  }

  componentDidMount() {
    fetch('https://api.example.com/items')
      .then(res => res.json())
      .then(
        (result) => {
          this.setState({
            employees: result.employees
          })
        },
        (error) => {
          this.setState({ error })
        }
      )
  }

  render() {
    const { error, employees } = this.state
    if (error) {
      return <div>Error: {error.message}</div>;
    } else {
      return (
        <ul>
          {employees.map(item => (
            <li key={employee.name}>
              {employee.name}-{employees.experience}
            </li>
          ))}
        </ul>
      )
    }
  }
}
```

### 128. What are render props?
#### (Render Props 란 무엇인가요?)

Render Props 는 값이 함수인 prop 를 이용하여 component 간에 코드를 공유하는 기술입니다.
아래 component 는 render prop 을 사용하여 React element 를 반환합니다.

```jsx harmony
<DataProvider render={data => (
  <h1>{`Hello ${data.target}`}</h1>
)}/>
```

React Router 와 DownShift 라이브러리는 이 패턴을 사용합니다.

## React Router

### 129. What is React Router?
#### (React Router 가 무엇인가요?)

React Router 는 React 에 구현된 강력한 routing 라이브러리 입니다.
페이지에 보여지는 내용과 URL 을 동기화된 상태로 유지해주고, 애플리케이션에 새로운 화면과 흐름을 추가할 수 있게 도와줍니다.

### 130. How React Router is different from history library?
#### (React router 와 history 라이브러리의 다른점은 무엇인가요?)

React router 는 history 라이브러리를 감싼 래퍼입니다. React router는 브라우저의 `window.history` 과 상호작용을 하고, 브라우저 및 hash history 을 다룹니다.
또 모바일 앱 개발 (React Native) 및 Node 의 unit testing 처럼 global history 가 없는 환경에 유용한 memory 히스토리를 제공합니다.

### 131. What are the <Router> components of React Router v4?
#### (React router v4 의 <Router> component 는 무엇이 있나요?)

React router v4는 아래와 같은 3가지 component 를 제공합니다.

```jsx harmony
- <BrowserRouter>
- <HashRouter>
- <MemoryRouter>
```

위의 components 들은 browser, hash, 그리고 memory history 인스턴스를 만듭니다.
React Router v4 는 Router Object 의 context 를 통해 history 인스턴스의 속성과 메서드를 이용할 수 있게 해줍니다.

### 132. What is the purpose of push() and replace() methods of history?
#### (history의 push() 와 replace()  메서드의 목적은 무엇인가요?)

history 인스턴스에는 navigation 을 위한 두 가지 메서드가 있습니다.

- push()
- replace()

방문한 위치의 history 를 배열로 생각한다면, push() 는 배열에 새 위치를 추가하는 것이고 replace() 는 현재의 위치를 새 위치로 변경하는 것입니다.

### 133. How do you programmatically navigate using React Router v4?
#### (어떻게 프로그래밍 방식으로 React Router v4 의 navigate  를 사용하나요?)

component 안에서 프로그래밍 방식으로 routing/navigation 을 수행하는 세가지의 다른 방법이 있습니다.

**withRouter() higher-order function 을 사용하기:**

withRouter () higher-order function 은 history object 를 component 의 prop 로 삽입합니다.
이 객체는 context 의 사용을 피하기 위해 push() 그리고 replace() 메서드를 제공합니다.

```jsx harmony
import { withRouter } from 'react-router-dom' // this also works with 'react-router-native'

const Button = withRouter(({ history }) => (
  <button
    type='button'
    onClick={() => { history.push('/new-location') }}
  >
    {'Click Me!'}
  </button>
))
```

**Route component 그리고 render props 패턴 사용하기:**

`<Router>` component 는 withRouter() 와 같은 prop 를 전달하므로, history prop 를 통해 history 메서드에 접근할 수 있습니다.

```jsx harmony
import { Route } from 'react-router-dom'

const Button = () => (
  <Route render={({ history }) => (
    <button
      type='button'
      onClick={() => { history.push('/new-location') }}
    >
      {'Click Me!'}
    </button>
  )} />
)
```

**context 사용**

이 옵션은 추천되지 않으며 불안정한 API 로 처리됩니다.

```jsx harmony
const Button = (props, context) => (
  <button
    type='button'
    onClick={() => {
      context.history.push('/new-location')
    }}
  >
    {'Click Me!'}
  </button>
)

Button.contextTypes = {
  history: React.PropTypes.shape({
    push: React.PropTypes.func.isRequired
  })
}
```

### 134. How to get query parameters in React Router v4?
#### (React Router v4 에서 어떻게 query parameters 가져오나요?)

수년동안 다른 구현 지원에 대한 사용자들의 요청이 있었기 때문에 React Router v4의 query strings 을 parse 하는 기능이 제거되었습니다.
그래서 사용자들이 선호하는 구현방식을 선택하도록 결정되었습니다.
추천 방법은 query strings 라이브러리를 사용하는것 입니다.

```jsx harmony
const queryString = require('query-string');
const parsed = queryString.parse(props.location.search);
```

native 방식을 원한다면 URLSearchParams 을 사용할 수 있습니다.

```jsx harmony
const params = new URLSearchParams(props.location.search)
const foo = params.get('name')
```

IE11에는 polyfill을 사용해야합니다.

### 135. Why you get "Router may have only one child element" warning?
#### (왜 "Router 는 오직 하나의 자식 element 만 있을 수 있습니다" 라는 경고를 받나요?)

`<Switch>` 는 route 를 독점적으로 렌더링하기 때문에 `<Switch>` 으로 Route 들을 감싸야합니다.

먼저 Switch 를 가져와야 추가해야 합니다.

```jsx harmony
import { Switch, Router, Route } from 'react-router'
```

`<Switch>` 블록안에 routes 를 정의해아합니다.

```jsx harmony
<Router>
  <Switch>
    <Route {/* ... */} />
    <Route {/* ... */} />
  </Switch>
</Router>
```

### 136. How to pass params to history.push method in React Router v4?
#### (React Router v4 에서 어떻게 history.push 메서드에 파라미터를 전달하나요?)

navigating 하는 동안 history object 에 props 를 전달할 수 있습니다.

```js
this.props.history.push({
  pathname: '/template',
  search: '?name=sudheer',
  state: { detail: response.data }
})
```

`search` 속성은 push() 메서드에 query params 을 전달하는데 사용됩니다.

### 137. How to implement default or NotFound page?
#### (기본 페이지 또는 NotFound 를 어떻게 구현하나요?)

`<Switch>` 는 일치하는 첫번째 자식 `<Route>` 를 렌더링합니다. 경로가 없는 `<Route>` 는 항상 일치합니다.
아래와 같이 경로를 속성을 제거해주면됩니다.

```jsx harmony
<Switch>
  <Route exact path="/" component={Home}/>
  <Route path="/user" component={User}/>
  <Route component={NotFound} />
</Switch>
```

### 138. How to get history on React Router v4?
#### (어떻게 React Router v4에서 history를 얻나요?)

**history object 를 내보내고 이 모듈을 전체 프로젝트에 가져오는 모듈을 만드세요.**

예를 들면, history.js 파일을 만듭니다.

```js
import { createBrowserHistory } from 'history'

export default createBrowserHistory({
  /* pass a configuration object here if needed */
})
```

**기본 구현된 routers 대신 `<Router>` component 를 사용해야합니다. index.js 에서 위의 history.js 를 가져왔습니다.**

```jsx harmony
import { Router } from 'react-router-dom'
import history from './history'
import App from './App'

ReactDOM.render((
  <Router history={history}>
    <App />
  </Router>
), holder)
```

**기본 구현된 history object 와 유사하 history object 의 push 메서드를 사용할 수 있습니다.**

```jsx harmony
// some-other-file.js
import history from './history'

history.push('/go-here')
```

### 139. How to perform automatic redirect after login?
#### (어떻게 로그인후에 자동으로 redirect 를 시키나요?)

`react-router` 패키지는 React Router 에 `<Redirect>` component 를 제공합니다. `<Redirect>` 을 렌더링하면 새로운 위치로 이동합니다.
server-side redirect 와 같이, history stack 의 현재 위치를 새로운 위치로 덮어씌웁니다. 

```jsx harmony
import React, { Component } from 'react'
import { Redirect } from 'react-router'

export default class LoginComponent extends Component {
  render() {
    if (this.state.isLoggedIn === true) {
      return <Redirect to="/your/redirect/page" />
    } else {
      return <div>{'Login Please'}</div>
    }
  }
}
```

## React Internationalization

### 140. What is React Intl?
#### (React Intl 이 무엇인가요?)

[React Intl](https://github.com/yahoo/react-intl) 라이브러리는 문자열, 날짜와 숫자, 다중화 formatting 을 다룰 수 있는 component 와 api 를 제공합니다.
React Intl 는 components 와 API 를 통해 React 에 바인딩을 제공하는 FormatJS 의 일부분입니다.

### 141. What are the main features of React Intl?
#### (React Intl 의 주요 특징은 무엇인가요?)

- [구분자와 함께 숫자를 표시합니다](https://medium.com/@marcelmokos/internationalize-react-apps-done-right-using-react-intl-library-82978dbe175e)
- 날짜와 시간을 정확하게 표시합니다.
- "now" 를 기준으로 날짜를 표시합니다.
- 150 개 이상의 언어를 지원합니다.
- 브라우저와 노드에서 실행됩니다.
- 표준을 기반으로 구축되었습니다.

### 142. What are the two ways of formatting in React Intl?
#### (React Intl 에서 formatting 을 하는 두 가지 방법은 무엇인가요?)

라이브러리는 문자, 숫자와 날짜의 형식을 지정하는 두 가지 방법을 제공합니다. : React component 또는 API 

```jsx harmony
<FormattedMessage
  id={'account'}
  defaultMessage={'The amount is less than minimum balance.'}
/>
```

```jsx harmony
const messages = defineMessages({
  accountMessage: {
    id: 'account',
    defaultMessage: 'The amount is less than minimum balance.',
  }
})

formatMessage(messages.accountMessage)
```

### 143. How to use <FormattedMessage> as placeholder using React Intl?
#### (어떻게 React Intl를 사용하여 <FormattedMessage> 를 placeholder 로 사용하나요?)

react-intl 의 <Formatted... /> component 는 elements 를 리턴하므로, placeholders, alt text, etc 등을 사용할 수 없습니다.
이런 경우에는 하위 레벨의 API formatMessage() 를 사용해야합니다.
higher-order component 인 injectIntl() 를 사용하여 component 에 intl object 를 주입하고 object 에서 사용할 수 있는 formatMessage() 를 사용하여 message 형식을 지정할 수 있습니다.

```jsx harmony
import React from 'react'
import { injectIntl, intlShape } from 'react-intl'

const MyComponent = ({ intl }) => {
  const placeholder = intl.formatMessage({id: 'messageId'})
  return <input placeholder={placeholder} />
}

MyComponent.propTypes = {
  intl: intlShape.isRequired
}

export default injectIntl(MyComponent)
```

### 144. How to access current locale with React Intl?
#### (어떻게 React Intl 를 사용하여 현재 locale 에 접근하나요?)

`injectIntl()` 를 사용하면 application 의 모든 component 에서 현재 locale 을 가져올 수 있습니다.

```jsx harmony
import { injectIntl, intlShape } from 'react-intl'

const MyComponent = ({ intl }) => (
  <div>{`The current locale is ${intl.locale}`}</div>
)

MyComponent.propTypes = {
  intl: intlShape.isRequired
}

export default injectIntl(MyComponent)
```

### 145. How to format date using React Intl?
#### (React Intl 을 사용해서 어떻게 날짜 형식을 지정하나요?)

higher-order component 인 `injectIntl()` 는 component 의 props 를 통해 `formatDate ()` 메서드에 대한 접근을 제공합니다.
이 메서드는 FormatedDate 의 인스턴스 내부에서 사용되며 형식이 지정된 날짜의 문자 표현을 반환합니다.

```jsx harmony
import { injectIntl, intlShape } from 'react-intl'

const stringDate = this.props.intl.formatDate(date, {
  year: 'numeric',
  month: 'numeric',
  day: 'numeric'
})

const MyComponent = ({intl}) => (
  <div>{`The formatted date is ${stringDate}`}</div>
)

MyComponent.propTypes = {
  intl: intlShape.isRequired
}

export default injectIntl(MyComponent)
```

## React Testing

### 146. What is Shallow Renderer in React testing?
#### (React 테스트에서 얕은 렌더링은 무엇인가요?)

얕은 렌더링은 React 에서 단위 테스트 케이스를 작성하는데 유용합니다.
그것은 component 를 한단계 깊이로 렌더링하며 인스턴스화 또는 렌더링 되지 않은 하위 component 의 행동에 대한 걱정없이 
렌더링 메서드가 반환하는 것에 대한 사실을 주장할 수 있습니다.

예를 들어, 다음과 같은 component 가 있는 경우:

```jsx harmony
function MyComponent() {
  return (
    <div>
      <span className={'heading'}>{'Title'}</span>
      <span className={'description'}>{'Description'}</span>
    </div>
  )
}
```

다음과 같이 주장 할 수 있습니다:

```jsx harmony
import ShallowRenderer from 'react-test-renderer/shallow'

// in your test
const renderer = new ShallowRenderer()
renderer.render(<MyComponent />)

const result = renderer.getRenderOutput()

expect(result.type).toBe('div')
expect(result.props.children).toEqual([
  <span className={'heading'}>{'Title'}</span>,
  <span className={'description'}>{'Description'}</span>
])
```

### 147. What is TestRenderer package in React?
#### (React 의 TestRenderer 패키지는 무엇인가요?)

패키지는 component 를 DOM 또는 Native mobile 환경에 의존없이 순수 Javascript Object 로 렌더링 할 수 있는 renderer 를 제공합니다.
패키지를 사용하면 브라우저 또는 jsdom 의 사용없이 ReactDOM 또는 React Native 에서 렌더링 되는 플랫폼의 뷰 계층구조 (DOM 트리와 유사하다) 의 스냅샷을 쉽게 가져올 수 있습니다.

```jsx harmony
import TestRenderer from 'react-test-renderer'

const Link = ({page, children}) => <a href={page}>{children}</a>

const testRenderer = TestRenderer.create(
  <Link page={'https://www.facebook.com/'}>{'Facebook'}</Link>
)

console.log(testRenderer.toJSON())
// {
//   type: 'a',
//   props: { href: 'https://www.facebook.com/' },
//   children: [ 'Facebook' ]
// }
```

### 148. What is the purpose of ReactTestUtils package?
#### (ReactTestUtils 패키지의 목적은 무엇인가요?)

ReactTestUtils 는 with-addons 에서 제공되며 유닛 테스트를 위해 시뮬레이션된 DOM 에 대한 작업을 수행할 수 있습니다.

### 149. What is Jest?
#### (Jest 는 무엇인가요?)

Jest 는 Facebook 에서 만든 Jasmine 기반의 Javascript 단위 테스트 프레임워크이며 자동화 된 모의 생성 및 jsdom 환경을 제공합니다.
종종 component 를 테스트하기위해 사용됩니다.

### 150. What are the advantages of Jest over Jasmine?
#### (Jasmine 보다 좋은 Jest 의 장점은 무엇인가요?)

Jasmine 과 비교하였을때 몇가지 장점이 있습니다.

- 소스코드에서 실핼할 테스트를 자동으로 찾아줍니다.
- 테스트 실행시 자동으로 모의 의존성을 가져옵니다.
- 비동기 코드를 동기적으로 테스트할 수 있습니다.
- command line 에서 테스트를 실핼할 수 있도록 가짜 DOM 구현 (jsdom 을 통해) 테스트를 실행합니다.
- 병렬 프로세스에서 테스트가 실행되어 빨리 완료됩니다.

### 151. Give a simple example of Jest test case
#### (Jest 테스트 케이스의 간단한 예제입니다)

`sum.js` 파일에 두개의 숫자를 더하는 함수의 테스트를 작성해보겠습니다.

```js
const sum = (a, b) => a + b

export default sum
```

테스트가 포함되어 있는 `sum.test.js` 파일을 만들어주세요

```js
import sum from './sum'

test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3)
})
```

`package.json` 에 다음 부분을 추가해주세요 

```json
{
  "scripts": {
    "test": "jest"
  }
}
```

마지막으로 yarn test 또는 npm test 를 실행해주세요 Jest 는 결과를 출력해줄거에요

```text
$ yarn test
PASS ./sum.test.js
✓ adds 1 + 2 to equal 3 (2ms)
```

## React Redux

### 152. What is flux?
#### (Flux 가 뭔가요?)

Flux 는 전통적인 MVC 패턴을 교체하기 위해 사용되는 application 설계 패러다임 입니다.  
Flux 는 라이브러리나 프레임워크는 아니고 React 와 단방향 데이터 흐름의 개념을 보완해주는 새로운 아키텍쳐입니다. 
Facebook 은 React로 작업할때 Flux 패턴을 사용합니다.

dispatcher, stores 그리고 views 컴포넌트 사이의 작업흐름은 input 과 output 이 다음과 같이 구분되어집니다.

![flux](./public/flux.png)

### 153. What is Redux?
#### (Redux 가 뭔가요?)

Redux 는 Flux 설계 패턴을 기반으로한 Javascript App 을 위한 예측 가능한 상태 컨테이너입니다. 
Redux 는 React 또는 다른 view 라이브러리들과 함께 사용될 수 있습니다.
그것은 작고 (2KB 정도) 종속성이 없습니다.

### 154. What are the core principles of Redux?
#### (React 의 핵심적인 원리는 무엇인가요?)

Redux 는 세가지의 기본원리를 따릅니다.
 
1. 단일 출처: 전체 application 의 상태는 하나의 스토어의 객체 트리에 저장됩니다. 
단일 상태 트리를 이용하면 시간 경과에 따른 변경사항 추척과 디버깅 또는 application 의 검사를 쉽게해줍니다.

2. 읽기전용의 상태: 상태를 변경하는 유일한 방법은 발생한 일에 대한 액션을 보내는것입니다.
이것은 view 와 Network callback 에서 상태를 직접 쓰지 않도록 보장합니다.

3. 순수함수로 만들어진다: 상태 트리가 액션에 의해 어떻게 변환될지를 reducers 에 작성해야합니다. 
Reducers 는 이전의 상태와 매개변수를 받는 순수함수이고 다음 상태를 반환해줍니다.

### 155. What are the downsides of Redux compared to Flux?
#### (Flux 와 비교했을때 Redux 의 단점은 무엇인가요?)

단점을 말하는것 보다는 Flux 보다 Redux 를 사용하는 것에 있어 타협점이 거의 없습니다. 예시는 다음과 같습니다.  

- 변이를 피하는 방법을 배워야합니다 : Flux 는 data 의 변이에 대해 유동적입니다. 그러나 Redux 는 변이를 좋아하지 않고 Redux 를 보완해주는 많은 패키지들이
 상태를 변화시키지 않도록 합니다. `redux-immutable-state-invariant` 나 `Immutable.js` 같은 개발 전용 패키지로 실시할 수 있으며, 당신의 팀에게 변이가 없는 코드를 가르칠 수 있습니다.
 
- 신중하게 패키지를 선택해야합니다: Flux 는 실행취소/다시실행, 지속성 또는 폼에 대한 문제를 해결하려 하지 않지만, Redux 는 미들웨어
 및 Store 개선 등 확장된 포인트들을 가지고 풍부한 생태계를 만들어 냈습니다.
 
### 156. What is the difference between mapStateToProps() and mapDispatchToProps()?
#### (mapStateToProps() 와 mapDispatchToProps() 의 다른점은 무엇인가요?)

`mapStateToProps()` 는 component 가 업데이트된 상태(다른 component 에 의해 업데이트된) 를 가져올 수 있게 도와주는 유틸리티입니다. 

```js
const mapStateToProps = (state) => {
  return {
    todos: getVisibleTodos(state.todos, state.visibilityFilter)
  }
}
```

`mapDispatchToProps()` 는 component 가 이벤트를 발생시킬 수 있도록 도와주는 유틸리티입니다. (application 의 상태가 변경될 수 있도록 action 을 보냄)

```js
const mapDispatchToProps = (dispatch) => {
  return {
    onTodoClick: (id) => {
      dispatch(toggleTodo(id))
    }
  }
}
```

### 157. Can I dispatch an action in reducer?
#### (reducer 에서 action 을 전달할 수 있나요?)

reducer 안에서 action 을 보내는 것은 안티패턴입니다. reducer 는 side effects 가 없어야하고 단순히 action 에 대한 처리와 새로운 객체를 반환해야합니다.
reducer 안에서 액션을 보내거나 listeners 를 추가한다면 다른 side effects 가 발생할 수 있습니다.

### 158. How to access Redux store outside a component?
#### (component 의 밖에서 Redux store 에 어떻게 접근하나요?)

`createStore()` 를 사용하여 만든 store 모듈을 내보내면 됩니다. 또한 global  window 객체를 더럽히면 안됩니다.

```js
store = createStore(myReducer)

export default store
```

### 159. What are the drawbacks of MVW pattern?
#### (MVW 패턴의 단점은 무엇인가요?)

- DOM 의 조작은 매우 느리고 비싸기 때문에 applications 의 동작을 느리고 비효율적이게합니다.
- 순환되는 종속성은 모델과 뷰를 복잡하게 만듭니다 
- 협업 applications 에서는 많은 데이터의 변화가 일어납니다 (ex. Google docs)
- 많은 코드를 추가하지않고 실행을 취소할 수 있는 방법이 없습니다.

### 160. Are there any similarities between Redux and RxJS?
#### (Redux 와 RxJS 의 유사한점이 있나요?)

두 라이브러리는 다른 목적을 가지고 있습니다. 그러나 약간의 유사점이 있습니다.

Redux 는 application 의 전체 상태를 관리하기 위한 툴입니다. 일반적으로 UI 를 위한 구조로 사용됩니다.   
RxJS 는 반응형 프로그래밍 라이브러리입니다. 일반적으로 Javascript 에서 비동기적인 작업을 위해 사용됩니다. Promises 의 대안으로 사용할 수 있습니다. 
Redux 의 store 는 반응형이기 때문에 반응형 패러다임을 사용합니다. store 는 action 을 관찰하여 스스로 변화합니다. 
RxJS 또한 반응형 패러다임을 사용하지만 아키텍쳐는 아니므로 Observables 라는 빌딩 블록을 사용하여 패턴을 제공합니다.
  
### 161. How to dispatch an action on load?
#### (어떻게 load 시에 action 을 전달하나요?)

`componentDidMount` 와 `render()` 메서드에서 액션을 전달할 수 있고 데이터를 확인할 수 있습니다.

```jsx harmony
class App extends Component {
  componentDidMount() {
    this.props.fetchData()
  }

  render() {
    return this.props.isLoaded
      ? <div>{'Loaded'}</div>
      : <div>{'Not Loaded'}</div>
  }
}

const mapStateToProps = (state) => ({
  isLoaded: state.isLoaded
})

const mapDispatchToProps = { fetchData }

export default connect(mapStateToProps, mapDispatchToProps)(App)
```

### 162. How to use connect() from React Redux?
#### (어떻게 React Redux 에서 connect() 를 사용하나요?)

container 에서 store 를 사용하려면 두 단계를 따라야합니다.

- `mapStateToProps() 사용`: store 의 상태 값들을 지정 props 에 맵핑합니다. 
- 위의 props 를 컨테이너에 맵핑합니다: `mapStateToProps` 함수에 의해 리턴된 객체들은 컨테이너에 연결됩니다. `react-redux` 에서 `connect()` 를 가져올 수 있습니다.

```jsx harmony
import React from 'react'
import { connect } from 'react-redux'

class App extends React.Component {
  render() {
    return <div>{this.props.containerData}</div>
  }
}

function mapStateToProps(state) {
  return { containerData: state.data }
}

export default connect(mapStateToProps)(App)
```

### 163. How to reset state in Redux?
#### (어떻게 Redux 에서 상태 값을 초기화하나요?)

`combineReducers()`로 생성된 reducer 에게 action 을 위임하도록 application 에 root reducer 를 작성해야합니다. 

예를 들어, `rootReducer()` 는 `USER_LOGOUT` action 후 초기 상태 값을 반환하도록 합니다. reducer 는 action 에 상관없이
 첫 번째 매개변수가 undefined 로 호출될 때, 초기 상태 값을 반환합니다. 

```js
const appReducer = combineReducers({
  /* your app's top-level reducers */
})

const rootReducer = (state, action) => {
  if (action.type === 'USER_LOGOUT') {
    state = undefined
  }

  return appReducer(state, action)
}
```

`redux-persist` 를 사용할 경우 storage 를 비워야 할 수도 있습니다. `redux-persist` 은 복사된 상태값을 storage engine 에 저장해둡니다. 
우선 storage engine 을 가져오고, 상태를 undefined 로 설정하기 전에 storage state key 들을 비워주세요  

```js
const appReducer = combineReducers({
  /* your app's top-level reducers */
})

const rootReducer = (state, action) => {
  if (action.type === 'USER_LOGOUT') {
    Object.keys(state).forEach(key => {
      storage.removeItem(`persist:${key}`)
    })

    state = undefined
  }

  return appReducer(state, action)
}
```

### 164. Whats the purpose of at symbol in the Redux connect decorator?
#### (Redux connect decorator 의 at symbol 의 목적은 무엇인가요?)

@ symbol 은 decorators 를 나타내기위한 자바스크립트 표현식입니다. Decorators 는 설계시에 class 와 속성에 주석을 달고 수정을 할 수 있게 해줍니다.

decorator 가 없는 Redux 를 예로 들어보겠습니다.

- Without decorator:

```js
import React from 'react'
import * as actionCreators from './actionCreators'
import { bindActionCreators } from 'redux'
import { connect } from 'react-redux'

function mapStateToProps(state) {
  return { todos: state.todos }
}

function mapDispatchToProps(dispatch) {
  return { actions: bindActionCreators(actionCreators, dispatch) }
}

class MyApp extends React.Component {
  // ...define your main app here
}

export default connect(mapStateToProps, mapDispatchToProps)(MyApp)
```

- With decorator:

```js
import React from 'react'
import * as actionCreators from './actionCreators'
import { bindActionCreators } from 'redux'
import { connect } from 'react-redux'

function mapStateToProps(state) {
  return { todos: state.todos }
}

function mapDispatchToProps(dispatch) {
  return { actions: bindActionCreators(actionCreators, dispatch) }
}

@connect(mapStateToProps, mapDispatchToProps)
export default class MyApp extends React.Component {
  // ...define your main app here
}
```

위의 예제는 decorator 의 사용여부를 제외하고는 비슷합니다. decorator 는 아직 자바스크립트 runtime 에 구현되지 않았습니다.
여전히 실험적인 주제이므로 변화될 수 있습니다. decorators 를 지원하기 위해 babel 을 사용할 수 있습니다.

### 165. What is the difference between React context and React Redux?
#### (React context 와 React Redux 는 무엇이 다른가요?)

application 에서 직접적으로 Context 를 사용할 수 있으며 깊게 중첩된 component 들에게 데이터를 전달하는데 유용합니다.
Redux 는 훨씬 강력하며 Context API 가 지원하지 않는 많은 기능들을 제공해줍니다.
React Redux 는 내부적으로 Context 를 사용하지만 public API 에 공개하지 않았습니다.

### 166. Why are Redux state functions called reducers?
#### (왜 Redux 상태 함수를 reducers 라 부르나요 ?)

Reducers 는 항상 모든 이전과 현재의 action 들을 기반으로 누적한 상태를 반환합니다. 
Redux reducer 가 호출 될 때 마다 상태와 액션이 파라미터로 전달됩니다. 
상태는 action 에 따라 축소되거나 누적되어 다음 상태를 반환합니다. 
최종 상태를 얻기 위한 action을 실행함에 있어 action 단위와 store 의 초기 상태 값을 줄일 수 있습니다. 

### 167. How to make AJAX request in Redux? 
#### (어떻게 Redux 에서 AJAX 요청을 하나요?)

비동기 action 을 정의할 수 있는 `redux-thunk` 미들웨어를 사용할 수 있습니다.

fetch API 를 사용하여 특정한 계정을 AJAX call 로 가져오는 예제를 살펴보겠습니다.

```js
export function fetchAccount(id) {
  return dispatch => {
    dispatch(setLoadingAccountState()) // Show a loading spinner
    fetch(`/account/${id}`, (response) => {
      dispatch(doneFetchingAccount()) // Hide loading spinner
      if (response.status === 200) {
        dispatch(setAccount(response.json)) // Use a normal function to set the received state
      } else {
        dispatch(someError)
      }
    })
  }
}

function setAccount(data) {
 return { type: 'SET_Account', data: data }
}
```

### 168. Should I keep all component's state in Redux store?
#### (Redux Store 에서 component 들의 모든 상태를 저장하고 있어야 하나요?)

Redux Store 에서는 Data 를 저장하고 component 내부에서는 UI 에 관련된 상태들을 저장합니다. 

### 169. What is the proper way to access Redux store?
#### (Redux store 에 접근하는 올바른 방법은 무엇인가요?)

component 에서 store 에 접근하는 가장 좋은 방법은 `connect()` 함수를 사용하는 것 입니다. 
connect() 함수는 기존의 component 를 감싸 새로운 component 를 만듭니다. 
이 패턴은 `Higher-Order Components` 라고 불리며, React 에서 일반적으로 component 의 기능을 확장하는 기본적인 방법입니다. 이 방법은 상태와 action 생성자를 component 에 매핑하고 store 가 update 되면 자동적으로 
component 에 state 와 action 생성자를 전달할 수 있도록 해줍니다.

connect 를 사용한 `<FilterLink>` component 를 예로 들어보겠습니다.

```jsx
import { connect } from 'react-redux'
import { setVisibilityFilter } from '../actions'
import Link from '../components/Link'

const mapStateToProps = (state, ownProps) => ({
  active: ownProps.filter === state.visibilityFilter
})

const mapDispatchToProps = (dispatch, ownProps) => ({
  onClick: () => dispatch(setVisibilityFilter(ownProps.filter))
})

const FilterLink = connect(
  mapStateToProps,
  mapDispatchToProps
)(Link)

export default FilterLink
```

성능 최적화가되어 있고 일반적으로 버그를 유발할 가능성이 적기 때문에 Redux 개발자들은 Context API 를 사용하여 직접 store 에 접근하는 것 보다는 `connect()` 를 사용하는것을 대부분 추천합니다.

```js
class MyComponent {
  someMethod() {
    doSomethingWith(this.context.store)
  }
}
```

### 170. What is the difference between component and container in React Redux?
#### (React Redux 에서 container 와 component 의 다른점은 무엇인가요?)

Component 는 application 의 보여지는 부분을 묘사하는 class 또는 function component 입니다.   
Container 는 Redux store 와 연결된 component 를 부르는 비공식적인 용어입니다.  
Container 는 Redux 의 state update 와 action 을 구독하며, DOM element 를 렌더링하지 않습니다. 하위 표현 component 들에게 rendering 을 위임합니다.

### 171. What is the purpose of the constants in Redux?
#### (Redux 안의 상수들의 목적은 무엇인가요?)

상수를 사용하면 IDE 를 사용할 때 프로젝트 전체에서 특정한 기능의 모든 사용내역을 쉽게 찾을 수 있습니다. 또한 오타로 인한 어리석은 버그를 방지할 수 있습니다. 오타의 경우 즉시 `ReferenceError` 에러가 발생합니다.

일반적으로 우리는 하나의 파일에 저장합니다 (`constants.js` 또는 `actionTypes.js`)

```js
export const ADD_TODO = 'ADD_TODO'
export const DELETE_TODO = 'DELETE_TODO'
export const EDIT_TODO = 'EDIT_TODO'
export const COMPLETE_TODO = 'COMPLETE_TODO'
export const COMPLETE_ALL = 'COMPLETE_ALL'
export const CLEAR_COMPLETED = 'CLEAR_COMPLETED'
```

Redux 에서는 두 가지의 공간에서 사용합니다.

1. action 생성중: 

`actions.js` 를 만듭니다.

```js
import { ADD_TODO } from './actionTypes';

export function addTodo(text) {
  return { type: ADD_TODO, text }
}
```

2. reducers 안에서 
`reducer.js` 를 만듭니다.

```js
import { ADD_TODO } from './actionTypes'

export default (state = [], action) => {
  switch (action.type) {
    case ADD_TODO:
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ];
    default:
      return state
  }
}
```

### 172. What are the different ways to write mapDispatchToProps()?
#### (mapDispatchToProps() 를 작성하는 다른 방법은 무엇이 있나요?)

`mapDispatchToProps()` 안에서 `dispatch()` 를 사용하여 action creators 를 바인딩하는 몇가지 방법이 있습니다. 아래와 같은 몇가지 옵션들이 있습니다.

```js
const mapDispatchToProps = (dispatch) => ({
 action: () => dispatch(action())
})
```

```js
const mapDispatchToProps = (dispatch) => ({
 action: bindActionCreators(action, dispatch)
})
```

```js
const mapDispatchToProps = { action }
```

세 번째 옵션은 첫 번째 옵션의 축약형 입니다.

### 173. What is the use of the ownProps parameter in mapStateToProps() and mapDispatchToProps()?
#### (mapStateToProps() 그리고 mapDispatchToProps() 에서 ownProps 매개변수는 어떻게 사용하나요?)

만약 `ownProps` 매개변수가 명시되었다면, React Redux 는 component 로 전달된 props 를 연결된 함수들로 전달합니다.

만약 connected component 를 사용한다면: 

```jsx
import ConnectedComponent from './containers/ConnectedComponent';

<ConnectedComponent user={'john'} />
```

`mapStateToProps()` 그리고 `mapDispatchToProps()` 함수 안에서의 `ownProps` 는 객체입니다.

```js
{ user: 'john' }
```

이 객체를 사용하여 무엇을 반환할지 결정할 수 있습니다.

### 174. How to structure Redux top level directories?
#### (어떻게 Redux 의 상위 레벨 디렉토리를 구성하나요?)

대부분의 application 들은 아래와 같은 상위 디렉토리를 가집니다.

- Components: Redux 를 알지못하는 멍청한 component 들
- Containers: Redux 와 연결된 똑똑한 component 들
- Actions: 파일의 이름이 app의 일부와 일치하는 모든 action creator 들 
- Reducers: 파일의 이름이 state key 와 일치하는 모든 reducer 들
- Store: store 초기화 설정

이 폴더 구조는 중소의 app 에 적합합니다.

### 175. What is redux-saga?
#### (react-sage 는 무엇인가요?)

`redux-saga` 는  side effects (데이터 가져오기 같은 비동기적인 작업이나 browser cache 에 접근하는 것등) 을 React/Redux applications 에서 조금 더 쉽게 만들어주는 라이브러리입니다.

NPM 에서 사용할 수 있습니다.

```shell
$ npm install --save redux-saga
```

### 176. What is the mental model of redux-saga?
#### (redux-sage 의 근본적 모델은 무엇인가요?)

sage는 application 안에 분리된 쓰레드이고, side effects 를 위한 단독적인 책임을 가지고있습니다.
`redux-saga` 는 redux 미들웨어입니다. 메인 application 에서 Redux actions 과 함께 쓰레드를 시작, 중지, 취소 할 수 있으며 전체의 Redux application 상태에 접근할 수 있고 Redux actions 도 전달할 수 있습니다.

### 177. What are the differences between call() and put() in redux-saga?
#### (redux-saga 에서 call() 과 put() 의 차이점은 무엇인가요?)

`call()` 과 `put()` 둘 다 effect 를 만드는 함수입니다. `call()` 함수는 middleware 가 promise 를 어떻게 호출할지에 대한 설명하는 effect 을 생성하는데 사용됩니다. `put()` 함수는 store 에 action 을 통하여 전달하도록 미들웨어에게 가르치는 effect 를 생성합니다.

특정한 사용자의 데이터를 가져오는 예제를 보고 effects 가 어떻게 동작하는지 봅시다.

```js
function* fetchUserSaga(action) {
  // `call` function accepts rest arguments, which will be passed to `api.fetchUser` function.
  // Instructing middleware to call promise, it resolved value will be assigned to `userData` variable
  const userData = yield call(api.fetchUser, action.userId)

  // Instructing middleware to dispatch corresponding action.
  yield put({
    type: 'FETCH_USER_SUCCESS',
    userData
  })
}
```

### 178. What is Redux Thunk?
#### (Redux Thunk 는 무엇인가요?)

Redux Thunk 는 action 대신 함수를 반환하는 action 생성자를 작성 할 수 있는 미들웨어입니다.
Thunk 는 action dispatch 를 지연 시키거나, 특정한 조건이 성립되는 경우에만 dispatch 하도록 할 수 있습니다. 내부 함수는 매개변수로 store method dispatch 그리고 getState 를 받습니다. 

### 179. What are the differences between redux-saga and redux-thunk?
#### (redux-saga 와 redux-thunk 의 차이점은 무엇인가요 ?)

Redux Thunk 와 Redux Saga 는 모두 side effect 를 방지합니다. 
대부분의 시나리오에서 Thunk 는 Promise 를 사용하여 처리하고 Saga 는 Generators 를 사용합니다. Promise 는 많은 개발자들에게 친숙하여 Thunk 는 다루기 쉽고, Sagas / Generator 는 매우 강력하지만 러닝커브가 있습니다. 
두 미들웨어 모두 공존 할 수 있습니다. Thunk 로 시작하여도 만약 Saga 가 필요하다면 도입 할 수 있습니다.

### 180. What is Redux DevTools?
#### (Redux DevTools 은 무엇인가요?)

Redux DevTools 은 Redux 를 위한 hot reload 기능을 가진 시간 여행 환경의 실시간 편집이 가능한 툴입니다. 액션을 다시 재현하거나 UI 를 사용자정의에 맞게 만들 수 있습니다.
Redux DevTools 을 프로젝트에 설치하여 사용하고 싶지 않다면 Chrome 또는 Firefox 용 Extension 사용을 고려 할 수 있습니다.

### 181. What are the features of Redux DevTools?
#### (Redux DevTools 의 목적은 무엇인가요?)

1. 모든 상태와 액션을 검사 할 수 있습니다.
2. action 을 취소하여 작업을 되돌릴 수 있습니다.
3. reducer 의 코드를 변경한다면 각각의 준비된 action 은 다시 평가됩니다. 
4. action 에서 어떤 일이 일어났는지, 오류가 발생하였는지 알 수 있습니다.
5. `persistState()` store enhancer 을 사용하면 page reload 에서 debug session 을 지속할 수 있습니다.

### 182. What are Redux selectors and why to use them?
#### (Redux selectors 는 무엇이고 왜 사용해야하나요?)

Selectors 는 Redux state 를 인수로받고 데이터를 반환하여 component 로 전달하는 함수입니다.

예를 들어, 사용자의 세부정보를 얻으려면:

```js
const getUserData = state => state.user.data
```

### 183. What is Redux Form?
#### (Redux Form 은 무엇인가요?)

