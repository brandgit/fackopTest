<template>
  <div class="flex flex-col items-center w-full">
    <div class="flex flex-col items-center  text-center mt-[150px] w-[100%]">

      <!-- TOP PAGE -->
      <div class="w-[90%] font-bold text-[1.5rem] sm:text-[2rem] md:text-[2.5rem] lg:text-[3rem]">
        <p>
          Connecter les gens par la technologie pour renforcer leurs relations quotidiennes
        </p>
      </div>
      <div class="flex justify-center w-full">
        <div class="mt-10 w-[90%] h-[400px] sm:h-[700px] bg-white">
          <div class="containerVideo">
            <video
              muted
              autoplay="true"
              loop="true"
              class="videoTop"
              src="/videos/about.mp4"
            />
          </div>
        </div>
      </div>
      
      <!-- ABOUT OUR SERVICES -->
      <div class="flex flex-col items-center w-[90%]">
        
        <div class="w-[70%] font-bold sm:text-[20px] md:text-[30px] lg:text-[35px] mt-20">
          <p>
            FACKOP est un GROUPE NUMERIQUE qui a pour but de développer des
            solutions numériques et informatiques afin de faire en profité le
            plus grand nombre
          </p>
        </div>
        <NuxtLink class="text-[#5D3891] w-[80%] sm:text-[18px] py-5 mt-3" to="/services">En savoir plus sur nos Services</NuxtLink>
      </div>

        <!-- Services -->
        <!-- Service 1 -->
        <div class="w-[90%]">
          <p class="text-[1.3rem]  text-[#5D3891] font-bold sm:text-[20px] md:text-[30px] lg:text-[35px] mt-20">
              Accompagner les entreprise dans leur developpement
          </p>
          <div class="flex flex-col md:flex-row-reverse md:justify-between items-center">
            <img class="mt-10 rounded-[15px] md:w-[50%]" src="/images/serviceAbout1.jpg" alt="">
            <p class="sm:text-[1.3rem] md:text-[1rem] lg:text-[1.4rem] mt-5 md:w-[45%]">
              Nous sommes là pour vous accompagner dans votre développement, car ous croyons que les entreprises sont les moteurs de la croissance économique, et nous sommes déterminés à vous aider à atteindre vos objectifs en vous fournissant les outils et le soutien dont vous avez besoin. 
            </p>
          </div>
        </div>

        <!-- Service 2 -->
        <div class="w-[90%]">
          <p class="text-[#5D3891] font-bold sm:text-[20px] md:text-[30px] lg:text-[35px] mt-20">
            Facilité l'accès le quotidien de tous 
          </p>
          <div class="flex flex-col md:flex-row md:justify-between items-center">
            <img class="mt-10 rounded-[15px] md:w-[50%]" src="/images/serviceAbout4.jpg" alt="">
            <p class="sm:text-[1.3rem] md:text-[1rem] lg:text-[1.4rem] mt-5 md:w-[45%]">
              Grâce à nos solutions innovante, nous rendons l'accès à un large éventail de services quotidiens plus facile et plus rapide que jamais. Du shopping au transport en passant par solution de diverses domaines d'activités, nous vous offrons un moyen simple de gérer votre vie quotidienne.  
            </p>
          </div>
        </div>

        <!-- Service 3 -->
        <div class="w-[90%]">
          <p class="text-[#5D3891]  font-bold sm:text-[20px] md:text-[30px] lg:text-[35px] mt-20">
            Promouvoir le numérique
          </p>
          <div class="flex flex-col md:flex-row-reverse md:justify-between items-center">
            <img class="mt-10 rounded-[15px] md:w-[50%]" src="/images/serviceAboute2.jpg" alt="">
            <p class="sm:text-[1.3rem] md:text-[1rem] lg:text-[1.4rem] mt-5 md:w-[45%]">
              De la simplification des tâches quotidiennes à l'accès à des informations plus vastes, nous vous montrerons comment le numérique peut vous faciliter la vie. Rejoignez-nous dans notre mission pour promouvoir le numérique et découvrez comment vous pouvez en tirer le meilleur parti.
            </p>
          </div>
        </div>

      <!-- JOINT Fackop -->
      <div class="flex flex-col items-center w-full py-10 mt-16 bg-[#d2c1eb] ">
        <TitleH1 title="Rejoignez Fackop." />
        <div class="font-bold w-[80%] sm:text-[20px] mt-5">
          <p>
            Prenez part au développement de la technologie de demain en nous
            rejoignant.
          </p>
        </div>
        <div class="w-[80%] sm:text-[20px] mt-5">
          <p>
            La construction de systèmes numériques avancés requiert une collaboration interdisciplinaire entre personnes provenant de différents domaines et perspectives. Chez Fackop, nous sommes constamment à la recherche de personnes curieuses et talentueuses pour nous aider à concevoir des solutions sécurisées et de haute qualité.
          </p>
        </div>
        <div class="flex font-bold w-[80%] sm:text-[20px] mt-5">
          <h1>Nos offres:</h1>
        </div>
        <div class=" w-full py-20">
           <p>Pas d'offres disponible pour le moment</p>
      </div>
      </div>

      <!-- CONTACT -->
      <div class="flex flex-col items-center  text-center mt-[50px] w-[90%]">
      <TitleH1 title="Nos contacts" />
      <div class="w-[80%] sm:text-[20px] mt-5">
        <p>
          Nous sommes là pour vous accompagner, n'hésitez pas à nous faire part
          de vos besoins
        </p>
      </div>
      <NuxtLink
        class="text-[#5d3891] w-[80%] sm:text-[18px] mt-3"
        to="/contact"
      >
        En savoir plus sur nos contacts</NuxtLink
      >
    </div>
    
    <div class="mt-10 relative w-full h-[350px] sm:h-[400px] md:h-[500px] lg:h-[600px] bg-[green]">
      <div class="containerVideo">
        <video
          autoplay="true"
          loop="true"
          class="video"
          src="/Video/contact.mp4"
        />
      </div>
      <div
        class="absolute top-0 left-0 flex items-center justify-center w-full h-full"
      >
        <div class="flex flex-col justify-between w-[150px] h-[80px]">
          <NuxtLink
            class="flex cursor-pointer w-[100%] h-[45%] text-white justify-center items-center bg-black rounded-[10px] border-[2px] border-solid border-black"
            to="/contact"
          >
            Contact
          </NuxtLink>

          <NuxtLink
            class="flex cursor-pointer w-[100%] h-[45%] text-white justify-center items-center bg-black rounded-[10px] border-[2px] border-solid border-black"
            to="/newsletter"
          >
            Newsletter
          </NuxtLink>
        </div>
        <div
          class="flex justify-center items-center w-full h-full top-0 left-0 absolute"
        >
          <div class="flex flex-col justify-between w-[150px] h-[80px]">
            <NuxtLink
              class="flex cursor-pointer w-[100%] h-[45%] text-white justify-center items-center bg-black rounded-[10px] border-[2px] border-solid border-black"
              to="/contact"
              >Contact</NuxtLink
            >
            <NuxtLink
              class="flex cursor-pointer w-[100%] h-[45%] text-white justify-center items-center bg-black rounded-[10px] border-[2px] border-solid border-black"
              to="/newsletter"
              >Newsletter</NuxtLink
            >
          </div>
        </div>
      </div> 
    </div>
    </div>
  </div>
</template>

<script setup>
import { Icon } from "@iconify/vue";
</script>

<style scoped>
.wrapperAbout {
  width: 100%;
  height: 100vh;
  overflow: hidden;
  overflow-y: scroll;
  background-color: #141414;
}
.wrapperAbout::-webkit-scrollbar {
  background-color: transparent;
  width: 0px;
}


.containerVideo .videoTop {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 15px;
}

.containerVideo {
  min-height: 60%;
  height: 100%;
  position: relative;
  min-width: 200px;
}
.containerVideo .video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
