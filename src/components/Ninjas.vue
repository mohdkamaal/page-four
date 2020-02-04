<template>
<div id="ninjas">
    <ul>
        <li v-for="ninja in ninjas" v-on:click="ninja.show = !ninja.show">
            <h2>{{ ninja.name }}</h2>
            <h3 v-show="ninja.show">{{ ninja.speiality }}</h3>
        </li>
    </ul>
</div>
</template>



<script>
export default {
    data(){
        return{
            ninjas: [
                {name:'CREATE CLASS & VIEW CLASS', speciality: 'Vue Components', show: false},
                {name:'CREATE TEACHER VIEW ALL SUBJECTS WISE', speciality: 'Vue Components', show: false},
                {name:'CREATE EMPLOYEE', speciality: 'Vue Components', show: false},
                {name:'TRANSPORTATION', speciality: 'Vue Components', show: false},
                {name:'ACCOUNT', speciality: 'Vue Components', show: false},
                {name:'LIBRARY', speciality: 'Vue Components', show: false},
                {name:'HOSTEL', speciality: 'Vue Components', show: false},
                {name:'HEALTH', speciality: 'Vue Components', show: false},
                {name:'STUDENT T.C', speciality: 'Vue Components', show: false},
            ]
        }
    }
}
</script>

<style scoped>
#ninjas{
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
}
ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}
li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 15px;
    border: 1px solid rgb(129, 69, 207);
    border-radius: 20px;
    margin: 15px;
    font-family: Arial;
    color: rgb(129, 69, 207);
    cursor: pointer;
    box-shadow: 10px 10px 15px #888888;
}

</style>