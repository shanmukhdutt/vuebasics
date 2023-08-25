<template>
    <h2>{{data.name}}</h2>
    <h3>{{data.email}}</h3>
    <button v:onClick="">Alert Name</button>
</template>

<script>
export default{
    name:'User',
    props:{
        data:Object
    },
}
</script>
<style>
.user{
    background-color: skyblue;
    padding:10px;
    border-bottom:1px solid;
    margin-bottom:20px;
}
</style>