<template>
    <div class="hello">
        <h1>{{ msg }}</h1>
    </div>
</template>
<script>
export default{
name:'HelloWorld',
props:{
    msg:String
}
}
</script>
<style scoped>
h1{
    color:cornflowerblue;
    background-color: rgb(235, 230, 230);
    padding:20px;
    align-content: center;

}
</style>
