<template>
  <div id="app">
    <TodoHeader></TodoHeader>
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>
  </div>
</template> 

<script>
// 컴포넌트들을 임포트한다.
// TodoHeader.vue 파일을 TodoHeader 라는 이름으로 담겠다.
import TodoHeader from './components/TodoHeader.vue'
import TodoInput from './components/TodoInput.vue'
import TodoList from './components/TodoList.vue'
import TodoFooter from './components/TodoFooter.vue'

export default {
  methods: {
    
  },
  // created : vue instance가 생성되자마자 호출됨 (vue lifecycle hook)
  created(){
      
  },
  components: {
    // 컴포넌트 태그명 : 컴포넌트 내용
    // 'TodoHeader' : TodoHeader,
    // 'TodoInput' : TodoInput,
    // 'TodoList' : TodoList,
    // 'TodoFooter' : TodoFooter
    // ES6 - 속성명과 값 명이 동일할때 아래와 같이 축약할 수 있다.
    TodoHeader,
    TodoInput,
    TodoList,
    TodoFooter
  }
}
</script>

<style>
/* 앱 전체에서 적용할 css를 여기에 선언한다. */
body {
  text-align: center;
  background-color: #f6f6f6;
}
input {
  border-style: groove;
  width: 200px;
}
button {
  border-style: groove;
}
.shadow {
  box-shadow: 5px 10px 10px rgba(0, 0, 0, 0.03);
}
</style>
