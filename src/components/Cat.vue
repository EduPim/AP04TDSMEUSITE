<template>
    <div>
        <div id="selection">
            <button id="button" type="button" class="btn" v-on:click="catSize++">BIG Cats</button>
            <button id="button" type="button" class="btn" v-on:click="catSize--">SMALL Cats</button>
            <button id="button" type="button" class="btn" @click="holder=Switch1(holder);">Change Cat 1</button>
            <button id="button" type="button" class="btn" @click="holder=Switch2(holder);">Change Cat 2</button>
            <button id="button" type="button" class="btn" @click="holder=Switch3(holder);">SURPRISE</button>
        </div>
        <div>
            <img id="cat1" src="../assets/jinx2.gif" class="jinxcat" v-bind:style="{ width: catSize + '%',visibility: hidden }">
            <img id="cat2" src="../assets/3dcat2.gif" class="jinxcat" v-bind:style="{ width: catSize + '%',visibility: hidden}">
        </div>
    </div>  
</template>

  <script>

    export default {
        methods:{
            Switch1(){
                document.getElementById('cat1').style.visibility = 'visible';
                document.getElementById('cat2').style.visibility = 'hidden';
            },
            Switch2(){
                document.getElementById('cat1').style.visibility = 'hidden';
                document.getElementById('cat2').style.visibility = 'visible';
            },
            Switch3(){
                document.getElementById('cat1').style.visibility = 'visible';
                document.getElementById('cat2').style.visibility = 'visible';
            },
        },
        sl: '#selection',
        data () {
            return {
                catSize: 20,
                hidden: "hidden"
            }
        }
    }



  </script>
  <style scoped>
  </style>