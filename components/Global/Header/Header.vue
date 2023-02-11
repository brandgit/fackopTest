<script setup>
 import { ref } from 'vue'
 import { Icon } from '@iconify/vue';
 const STATE = ref(true)
 const StateAllFackop = ref(true)
 const IsActiveP = ref(true)
 const IsActiveA = ref(false)
 const IsActiveS = ref(false)
 const IsActiveC = ref(false)

 function changeOfStateP()
  {
        if(IsActiveP != true){
            IsActiveP.value = true
            IsActiveA.value = false
            IsActiveS.value = false
            IsActiveC.value = false
        }else{
            IsActiveA.value = false
            IsActiveS.value = false
            IsActiveC.value = false
        }
       
  }
  function changeOfStateS()
  {
        if(IsActiveS != true){
            IsActiveP.value = false
            IsActiveA.value = false
            IsActiveS.value = true
            IsActiveC.value = false
        }else{
            IsActiveP.value = false
            IsActiveA.value = false
            IsActiveC.value = false
        }
       
  }
  function changeOfStateA()
  {
        if(IsActiveA != true){
            IsActiveP.value = false
            IsActiveA.value = true
            IsActiveS.value = false
            IsActiveC.value = false
        }else{
            IsActiveP.value = false
            IsActiveS.value = false
            IsActiveC.value = false
        }
       
  }
  function changeOfStateC()
  {
        if(IsActiveC != true){
            IsActiveP.value = false
            IsActiveA.value = false
            IsActiveS.value = false
            IsActiveC.value = true
        }else{
            IsActiveP.value = false
            IsActiveA.value = false
            IsActiveS.value = false
        }
       
  }
  
  function changeOfState()
  {
      STATE.value = true &&  !STATE.value
   }

   function changeOfStateAllFackop()
    {
        if(StateAllFackop){
            StateAllFackop.value = false
        }else{
            StateAllFackop.value = true
            StateAllFackop.value = false
        }
       
    }
</script>

<template>
    <div class="wrappHeader">
        <div class="flex justify-between items-center w-[90%] h-full">
            <div class="flex justify-between items-center h-full w-[120px]  sm:w-[155px] ">
                <div class="wrapperMenuBurger">
                    <div class="wrapperButtonMenuBurger">
                        <div @click="changeOfState()" class="buttonMenuBurger">
                            <div v-bind:class="[STATE ? 'barBurgerUnclicked' : 'barBurgerClicked']"></div>
                            <div v-bind:class="[STATE ? 'barBurgerUnclicked' : 'barBurgerClicked']"></div>
                            <div v-bind:class="[STATE ? 'barBurgerUnclicked' : 'barBurgerClicked']"></div>
                        </div>
                    </div>
                    <div @click="changeOfState()" v-bind:class="[STATE ? 'notActive' : 'active']">
                        <div v-if="!STATE" class="contentMenuBurger">
                           <div class="h-[200px] w-[95%]">
                                <div class="flex flex-col justify-evenly h-full sm:text-[15px] ">
                                    <NuxtLink  to="/"><h1>Home</h1></NuxtLink>
                                    <NuxtLink to="/services"><h1>Services</h1></NuxtLink>
                                    <NuxtLink to="/about"><h1>About</h1></NuxtLink>
                                    <NuxtLink to="/contact"><h1>Contacts</h1></NuxtLink>
                                </div>
                           </div>
                           <div class="h-[200px] w-[95%] ">
                                <div class="flex items-center cursor-pointer text-[11px] sm:text-[15px] ">
                                    <h1 >All Fackop ressources</h1>
                                </div>
                                <div class="flex text-[#908d8d]  ml-4 flex-col justify-evenly h-[150px] ">
                                    <NuxtLink  to="/"><h1>Home</h1></NuxtLink>
                                    <NuxtLink to="/services"><h1>Services</h1></NuxtLink>
                                    <NuxtLink to="/about"><h1>About</h1></NuxtLink>
                                    <NuxtLink to="/contact"><h1>Contacts</h1></NuxtLink>
                                </div>
                           </div>
                           <div class="flex items-end w-[95%] h-[200px] ">
                                <div class='flex w-full text-[14px] text-white'>
                                    <div class='flex text-xs flex-col  pt-5 pb-3 items-center w-[90%]   border-t-white border-solid border-t-[2px]'>
                                        <p>Copyright - Fackop © 2023 Inc.</p>
                                        <p class="sm:ml-5">Tous droits réservés.</p>
                                        <p class="sm:ml-5">Mentions légales</p>
                                    </div>
                                </div>
                           </div>
                        </div>
                        
                        <div v-else></div>
                    </div>
                </div>
                <NuxtLink to="/"><img class=" w-[90px] sm:w-[120px]" src="/logos/LogoFackop6.0.png" alt="logo-fackop"></NuxtLink>
            </div>
            <nav class="w-[55%] h-full">
                <div class="flex items-center justify-end w-full h-full" >
                    <div class="flex items-center justify-between  h-full w-[300px] ">
                        <NuxtLink  @click="changeOfStateP()"  class="flex items-center  h-full  " to="/"><h1 :class="[IsActiveP? 'isClicked1' : 'isClicked2' ]" >Presentation</h1></NuxtLink>
                        <NuxtLink @click="changeOfStateS()" class="flex items-center  h-full  " to="/services"><h1 :class="[IsActiveS? 'isClicked1' : 'isClicked2' ]">Services</h1></NuxtLink>
                        <NuxtLink @click="changeOfStateA()" class="flex items-center  h-full  " to="/about"><h1 :class="[IsActiveA? 'isClicked1' : 'isClicked2' ]">About</h1></NuxtLink>
                        <NuxtLink @click="changeOfStateC()" class="flex items-center  h-full  " to="/contact"><h1 :class="[IsActiveC? 'isClicked1' : 'isClicked2' ]">Contacts</h1></NuxtLink>
                    </div>
                </div>
            </nav>
            <div @click="StateAllFackop = true &&  !StateAllFackop" class="flex items-center cursor-pointer text-[11px] sm:text-[15px] ">
                <h1 class="text-" >All Fackop ressources</h1>
                <Icon class="text-white sm:ml-1 w-10 h-7" icon="ic:baseline-arrow-drop-down" />
            </div>
            <div :class="[StateAllFackop? 'nomodalCart' : 'modalCart' ]" @click="StateAllFackop = true &&  !StateAllFackop">
                <div class="flex justify-end w-[90%] ">
                    <div class=" px-6 rounded-[3px] mt-[55px] w-[160px] sm:w-[200px] h-[200px] sm:h-[220px] bg-white text-black text-[11px] sm:text-[12px]" v-if="!StateAllFackop">
                        <ul class="flex  flex-col h-[90%] justify-evenly">
                            <li class="cursor-pointer">Fallaa</li>
                            <li class="cursor-pointer">Allô-Tchop</li>
                            <li class="cursor-pointer">Clando</li>
                            <li class="cursor-pointer">Kidangui</li>
                            <li class="cursor-pointer">Ogoula</li>
                            <li class="cursor-pointer">Pôpô</li>
                        </ul>
                    </div>
                    <div v-else></div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.wrappHeader{
    display: flex;
    min-width: 320px;
    position: fixed;
    justify-content: center;
    width: 100%;
    height: 80px;
    background-color: rgba(0, 0, 0, .4);
    color: white;
    z-index: 1;
}

.wrapperMenuBurger{
        height: 80%;
        display: block;
    }
    nav{
        display: none;
    }
    .wrapperButtonMenuBurger{
        display: flex;
        align-items: center;
        width: 100%;
        height: 100%;
    }
    .buttonMenuBurger {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 15px;
        width: 20px;
        cursor: pointer;
    }
    .barBurgerUnclicked {
    height: 2px;
    width: 100%;
    background-color: white;
    /* background: linear-gradient(to right, rgba(253,255,0, .8) 35%, rgba(52, 73, 194, .8) 69%); */
    }
    .barBurgerClicked {
    height: 2px;
    width: 100%;
    background-color: white;
    /* background: linear-gradient(to right, rgba(253,255,0, .8) 35%, rgba(52, 73, 194, .8) 69%); */
    }
    .barBurgerClicked:nth-child(1) {
    transform: rotate(45deg) translate(0.25em, 0.3em);
    transition: ease-out 0.5s;
    }
    .barBurgerClicked:nth-child(2) {
    transform: scale(0.1);
    transition: ease-out 0.5s;
    }
    .barBurgerClicked:nth-child(3) {
    transform: rotate(-45deg) translate(0.25em, -0.3em);
    transition: ease-out 0.5s;
    }
    .barBurgerUnclicked {
    transform: rotate(0) translate(0);
    transition: cubic-bezier(0.175, 0.885, 0.32, 1.275) 0.5s;
    }
    .active {
    width: 100%;
    height: 100vh;
    z-index: 2;
    display: flex;
    
    top: 80px;
    left: 0px;
    position: fixed;
    transition: ease-out 0.5s;
    font-family: monospace;

    }
    .notActive{
        display: flex;
        position: fixed;
        width: 0%;
        height: 100vh;
        transition: ease-out 0.5s;
        top: 80px;
        left: 0px;
        z-index: 2;
    }

    .modalCart{
    display: flex;
    justify-content: center;
    position: fixed;
    width: 100%;
    height: 100vh;
    transition: ease-out 0.5s;
    top: 0px;
    right: 0px;
    z-index: 2;
}
.nomodalCart{
    display: flex;
    position: fixed;
    width: 100vw;
    height: 0px;
    transition: ease-out 0.5s;
    top: 0px;
    right: 0px;
}

.contentMenuBurger{
    /* flex flex-col items-end w-[250px] h-full bg-black */
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    width: 250px;
    height: 100%;
    backdrop-filter: blur(15px);
        background-color:rgb(0, 0, 0, .5);
}

    @media screen and (min-width: 1030px) {
    .wrapperMenuBurger {
        display: none;
    }

    nav{
        display: block;
    }
}

.isClicked1{
    display: flex;
    align-items: center;
    height: 100%;
    border-bottom-style: solid;
    border-bottom-width: 2px;
    border-bottom-color: aliceblue;
}

</style>
