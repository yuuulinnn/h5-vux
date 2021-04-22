<template>
    <div class="hello">
        <x-input v-model="name" title="体验人姓名：" placeholder="请输入体验人姓名"></x-input>
        <calendar v-model="date" title="体检时间：" placeholder="请选择体检时间" @on-show="log('show')" @on-hide="log('hide')"></calendar>
    </div>
</template>

<script>
    import { XInput, Calendar, XButton, Cell } from 'vux';
    export default {
        name: 'HelloWorld',
        components: {
            XInput,
            XButton,
            Calendar,
            Cell
        },
        data() {
            return {
                name: '',
                date: ''
            };
        }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
