<template>
  <div class="about">
    <h1>This is an about page. This is so hard.</h1>
    <button @click="clickBtn">Test</button><br>
    <button @click="buttonnum">Count</button><br>
    <span>버튼을 클릭한 횟수 : {{buttonclick}}</span>
  </div>
</template>

<script>
  export default{
    data(){
     return{
        buttonclick:0
     }
    },
    methods:{
     clickBtn(){
        alert('테스트');
      },
     buttonnum(){
       //함수는 buttonnum function(){}나 위 방법이나 동일함
        this.buttonclick+=1;
     }
  }
}
</script>
