<template>
 <div id="app">
   <div class="container">
     <div class="row header mb-5 p-3">
       <div class="col-lg-12">         
        <h2 clas> What I do Today</h2>
       </div>
     </div>
     <div class="row content">
        <div class="col-lg-12">
          <div class="pekerjaan-Skripsi">
            <div class="row">
              <div 
              v-for="tugasSaya in tugas" 
              v-bind:key="tugasSaya.id" 
              class="mb-3 tugas col-lg-12 text-left">
                <ItemTugas />
                </div>
            </div>
            </div>
          </div> 
        </div>
     </div>   
   </div>

</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import ItemTugas from"./components/ItemTugas.vue";
export default {
  name: "app",
  data: function(){
    return{
      tugas: [
        {
          id: 1,
          nama: "membersihakan kamar",
          isDone: false 
        },
         {
          id: 2,
          nama: "membersihakan Lemari",
          isDone: false
        },
         {
          id: 3,
          nama: "membersihakan meja",
          isDone: false 
        },
        {
          id: 4,
          nama: "membersihakan kasur",
          isDone: true 
        },
        {
          id: 5,
          nama: "membersihakan wc",
          isDone: false 
        }
      ]
    }
  },
  component: {
      ItemTugas
  }
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.header{
  background: #1abc9c;
}
.header h2{
  margin: 0;
}
.tugas .item{
  font-size: 20px;
}
.item-complate{
  color: red;
}
</style>
