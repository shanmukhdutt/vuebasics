<template>
   <!-- <h2>Get Checkbox and Radio Button</h2>
   <h3>Technology</h3>
   <lable for="java">Java</lable>
   <input type="checkbox" value="java" v-model="technology" id="java">
   <lable for="php">Php</lable>
   <input type="checkbox" value="php" v-model="technology" id="php">
   <lable for="node">Node</lable>
   <input type="checkbox" value="node" v-model="technology" id="node">
   <br /><br />
   <h3>Who I am</h3>
   <lable for="student">Student</lable>
   <input type="radio" value="student" name="who" v-model="who" id="student">
   <lable for="developer">Developer</lable>
   <input type="radio" value="developer" name="who" v-model="who" id="developer">
     <br /><br />
     <h4>Selected Technology:{{ technology }}</h4> -->
     <!-- <h2>Reuse Component</h2>
     <ul>
     <li v-for="item in users" :key="item.name">
        <User :data="item" />
    
    </li>
     </ul> -->
     <!-- <h2>{{ text }}</h2>
     <div v-html="tag"></div>
     <div v-html="tag"></div> -->
     <!-- <div>{{ tag }}</div> -->
     <h2>CSS Binding</h2>
     <h3 :class="applyStyle">Home Component</h3>
     <button @click="colorfull=!colorfull">Apply style</button>
</template>
<script>
export default{
    name:"Home",
    data()  
    {
        return {
            colorfull:false
        }
    },
    computed:{ 
        applyStyle(){
            return{
                green:this.colorfull,
                err:true,
                other:true
            }
        }
    }
    // data(){
    //     return{
    //         text:"Html text",
    //         tag:"<h3>Html tag<h3>",
    //         text:"<h2>Html tag 2<h2>"
    //     }
    // }
}
// import User from './User.vue'
// export default{
//     name:'Home',
//     components:{
//         User
//     },
//     data(){
//         return{
//             users:[
//                 {
//                     name:"xyz",
//                     email:"xyz@zyx.com"
//                 },
//                 {
//                     name:"abc",
//                     email:"abc@cba.com"
//                 },
//                 {
//                     name:"def",
//                     email:"def@fed.com"
//                 },
//                 {
//                     name:"ghi",
//                     email:"ghi@ihg.com"
//                 }
//             ]
//         }
//     },    
// }
</script>
<style scoped>
h2{
    color:brown
}
/* h3{
    color:green
}
h4{
    color:darkorchid
} */
.green{
    background-color: chartreuse;
    color: antiquewhite;
    width: 190px;
    padding:15px;
}
.err{
    color:crimson
}
.other{
    padding:10px
}
</style>