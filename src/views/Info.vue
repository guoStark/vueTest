<template>
    <div>
      hello info component
      <button @click="add()">添加</button>
    </div>
</template>

<script>
import store from '@/store'
    export default {
        name: "Info",
        store,
        data(){
            return{
              msg: '国庆节3',
              old: 'old year'
            }
        },
        methods:{
            add(){
                console.log('add Event from info!')
                debugger
                store.commit('increase')
            },
            output () {
                console.log('in output')
            }
        }
    }
</script>

<style scoped>

</style>
