# Hooks

Hook에는 여러종류가 있다.

`useState`, `useEffect`, `useReducer`, `useMemo`, `useCallback`, `useRef`, `CustomHooks` 외에 다른 Hook들도 있다. 

Hooks는 리액트 16.8부터 도입된 기능이다. 기존의 함수형 컴포넌트에서 할 수 없던 다양한 작업을 가능케 해준다.

## useState 함수 기반 상태 관리

```javascript
// name을 '' 으로 초기화
const [name, setName] = useState('');
// name값을 '이름'으로 변경
setName('이름');
```

## useEffect

```javascript
// 렌더링 될 때마다 호출
useEffect(() => {
  ...
})
// 마운트 될 때만 호출
useEffect(() => {
  ...
}, [])
// 특정 값이 업데이트 될 때 호출, 예) name 값이 업데이트 되었을 때만 호출
useEffect(() => {
  ...
}, [name])
```


## useReducer
useState보다 더 다양한 컴포넌트 상황에 따라 다양한 상태를 다른 값으로 업데이트해주고 싶을 때 사용

```javascript
function reducer(state, action) {
  return {...};
}
```


## useMemo
렌더링 하는 과정에서 특정 값이 바뀌었을 때만 연산, 바뀌지 않으면 이전 결과 다시사용

## useCallback (렌더링 성능 최적화)



## 다른 Hooks

<https://nikgraf.github.io/react-hooks/>

<https://github.com/rehooks/awesome-react-hooks>