<!-- <template>
    <h2>Simple form</h2>
    <ul>
        <li v-for="item in error" v-bind:key="item">
            {{ item }} not valid
        </li>
    </ul>
 <form>  
    <lable>Email:</lable>
    <input type="text" placeholder=" enter email" v-model="form.email"/>
    <br/> <br/>
    <lable>Password:</lable>
    <input type="password" placeholder="enter password" v-model="form.password"/>
    <br/><br/>
    <select v-model="form.country">
    <option>Ind</option>
    <option>UK</option>
    <option>USA</option>
    </select>
    <br/><br/>
    <h3>Gender</h3>
    <lable>Male:</lable>
    <input type="radio" name="gender" value="male" v-model="form.gender">
    <br/><br/>
    <h3>Female:</h3>
    <input type="radio" name="gender" value="female" v-model="form.gender">
    <br/><br/>
    <h3>Technology</h3>
    <lable>Java</lable>
    <br/><br/>
    <input type="checkbox" value="java" v-model="form.technology">
    <br/><br/>
    <lable>.Net</lable>
    <br/><br/>
    <input type="checkbox" value=".net" v-model="form.technology">
    <br /><br />
    <button v-on:click="login" type="button">Login</button>
 </form>
</template>
<script>
export default{
    name:"Home",
    data(){
        return{
            form:{
                email:'',
                password:'',
                country:'',
                gender:'',
                technology:[]
            },
            error:[],
        }
    },
    methods:{
        login(){
            this.error=[];
          for(const item in this.form){
            if(this.form[item] === ""||this.form [item].length===0){
                this.error.push(item)
            }
          }  
          if(this.error.lenght===0){
            alert("data has been submitted");
          }
          console.log(this.form,this.error)
        }
    }
}
</script>
<style scoped>
h2{
    color:orange

} -->
<!-- </style> -->
<!-- <template>
    <h1>Computed Properties</h1>
    <h2>{{ (dollars*rupeesVal)-discount }}</h2>
    <h2>{{ getResult }}</h2>
</template>
<script>
export default{
    name:"Home",
    data(){
        return {
            dollars:100,
            rupeesVal:70,
            discount:10,
        }
    },
    methods(){
         getResultMethod()
         return (this.dollars*this.rupeesVal)-this.discount;
    },
    computed:{
        getResult(){
           return (this.dollars*this.rupeesVal)-this.discount;
        }
    }
} -->
    
<!-- </script>
<style scoped>
h1{
    color:coral
}
h2{
    color:rgb(35, 235, 9)
}
</style> -->
<!-- <template>
    <h1>{{ count }}</h1>
    <button v-on:click="count-count+1"> + </button>
    <button v-on:click="count-count-1"> - </button>
</template>
<script>
export default {
    name:"Home",
    data()
    {
        return{
            count:0
        }
    },
    watch:{
        count(val)
        {
          if(val>5)[
            alert("stop counting")
          ]
        }
    }
}
</script> -->
<!-- <template>
    <h1>Dynamic Component</h1>
    <button @click="tab-'Java'">Load Java</button>
    <button @click="tab-'Php'">Load Php</button>
    <button @click="tab-'Node'">Load Node</button>
    
    <component :is="tab"/>
</template>
<script>
import Java from './Java.vue'
import Php from './Php.vue'
import Node from './Node.vue'
export default{
    name:"Home",
    components:{
        Java,Php,Node
    },
    data(){
        return{
            tab:'Java'
        }
    }
}
</script>
<style>
h1{
    color:orange
}
h3{
    color:rgb(10, 61, 44)
}
</style> -->
<!-- <template>
    <h2>Before MOunted</h2>
    <h3>mount testing</h3>
</template>
<script>
export default{
    name:"Home",
    data(){
        return{
            name:'pcm'
        }
    },
    beforeMount(){
        console.warn("beforeMount",this.$el)
    },
    mounted(){
        console.warn("mounted"),this.$el
    }
}
</script>
<style scoped>
h2{
    color:rgb(138, 179, 67)
}
h3{
    color:aqua
}
</style> -->
<!-- <template>
    <h2>Routing</h2>
</template>
<script>
export default{
    name:"Home",
}
</script>
<style scoped>
h2{
    color:orange
}
</style> -->
<!-- <template>
    <h1>Two Way Binding</h1>
    <input type="text" v-model="count" />
    <h2>{{ count }}</h2>
</template>
<script>
export default{
    name:"Home",
    data(){
        return {
            count:10
        }
    
}
}
</script> -->
<!-- <template>
    <h1>Get Input Field Value</h1>
    <input type="text" placeholder="enter email" v-model="email">
    <br/>
    <br/>
    <input type="password" password="enter password" v-model="password">
    <br/><br/>
    <button v-on:click="getdata()">Get Values</button>

</template>
<script>
export default{
    name:"Home",
    data(){
       return{
        email:"satwik",
        password:null
       }
    },
    methods:{
        getdata(){
            console.warn("values:",this.email,this.password)
        }
    }
}
</script>


<style scoped>
h3{
    color: rgb(0, 10, 70);
    background-color: blanchedalmond;
}
</style> -->
<!-- <template>
    <h1>Technology</h1>
    <label for="java">Java</label>
    <input type="checkbox" value="java" v-model="technology" id="java">
    <lable for="php">Php</lable>
    <input type="checkbox" value="php" v-model="technology" id="php">
    <lable for="node">Node</lable>
    <input type="checkbox" value="node" v-model="technology" id="node">
    <h4>Selected technology :{{ technology }}</h4>
</template>
<script>
export default{
    name:"Home",
    data(){
        return{
            technology:[]
        }
    }
}
</script>  -->
<!-- <template>
    <h1 v-if="show">If Condition</h1>
    <h1 v-else>Else Condition</h1>
    <button v-on:click="show=!show">Toggle</button>
</template>
<script>
export default{
    name:"Home",
    data(){
        return{
            show:true
        }
    }
}
</script>
 <template>
    <h1>For Loop in vue js</h1>
    <ul>
        <li v-for="dot in technology" :key="dot">
             {{ dot }}
        </li>
    </ul>
    <br/>
    <br/>
    <ul>
        <li v-for=" dot in user" :key="dot">
              Name is:{{ dot.name }}
              Email is:{{ dot.email }}
        </li>
    </ul>
</template>
<script>
export default{
    name:"Home",
        data(){

            return{
                technology:['java','php','html','node'],
                user:[{
                    name:"kss",
                    email:"kss@test.com"
            },
        {
            name:"Ssk",
            email:"Ssk@test.com"
        },
        {
             name:"Dss",
             email:"Dss@test.com"
        }]
            }
        }
    }
</script> -->
<!-- <template>
   <h1>OP</h1>
    <input type="text" placeholder="enter email" v-model="email">
    <br/>
    <br/>
    <input type="text">
    <br>
    <input type="password" password="enter password" v-model="password">
    <br/><br/>
    <button @click="show">Click</button>
</template>
let em = "email";
<script>
export default{
    name:"Home",
    data(){
        return{ 
            email:null,
            password:null,
            show:true

        }
    }
}
</script> -->

<!-- <template>
<h1>Ref in Vue #3</h1>
<input type="text" ref="input"/>
<button v-on:click="getData">Click</button>
</template>
<script>
export default{
    name:"Home",
    methods:{
        getData(){
           this.$refs.input.focus();
           let val=this.$refs.input.value;
           alert(val)
        }
    }
}
</script>
<style scoped>
h1{
    color:rgb(14, 124, 128)
}
</style> -->
<!-- <template>
    <h1>Form Modifers</h1>
    <input type="text" v-model="data">
    <h2>Data is:{{ data }}</h2>
</template>
<script>
export default{
    name:"Home",
    data(){
        return {
            data:''
        }
    }
}
</script> -->
<template>
    <h2>Non Props Data</h2>
    <Nonpro/>
</template>
<script>
import Nonpro from './Nonpro.vue';
export default{
    name:'Home',
    components:{
        Nonpro
    }
}
</script>




