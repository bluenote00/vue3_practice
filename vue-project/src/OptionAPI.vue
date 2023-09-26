
<script>

// 옵션 API 형식

export default {
  // 반응형 상태 -> this에 노출
  data() {
    return {
      count: 0
    }
  },

  // methods는 속성 값을 변경하고 업데이트 할 수 있는 함수이며
  // 템플릿 내에서 이벤트 핸들러로 바인딩 될 수 있다.
  methods: {
    increment() {
      this.count++
    }
  },

  // 수명 주기 훅 : 컴포넌트가 마운트 된 후 호출된다.
  mounted() {
    console.log(`숫자 세기의 초기값은 ${this.count} 입니다.`)
  }
}
</script>

<template>
  <button @click="increment">숫자 세기: {{ count }}</button>
</template>



