<template>
     <div class="flex flex-col py-20 items-center w-full">
      <h1
        class="text-[25px] py-5 sm:text-[30px] md:text-[40px] lg:text-[50px] font-bold"
      >
        GROUPE NUMERIQUE
      </h1>
      <div class="lg:flex lg:py-16 w-[90%]">
        <div class="w-full py-10 lg:py-0 lg:w-[40%]">
          <div class="flex flex-col w-[100%] lg:mt-20">
            <div class="text-[25px] w-[90%]">
              <p class="text-[#5d3891] font-bold">
                Créez l'histoires avec votre GROUPE NUMERIQUE
              </p>
            </div>
            <div class="w-[80%] sm:text-[20px] mt-5">
              <p>
                Ne restez pas en arrière, adoptez les technologies numériques
                pour augmenter votre efficacité et rester compétitif sur le
                marché actuel en constante évolution.
              </p>
            </div>
          </div>
        </div>
        <div class="containerVideoTop">
          <video  muted
            autoplay="true"
            loop="true" class="videoTop" src="/videos/introHomePageVideo.mp4" />
        </div>
      </div>
    </div>
</template>

<style scoped>

.containerVideoTop {
  min-height: 60%;
  position: relative;
  min-width: 200px;
}
.containerVideoTop{
  width: 100%;
  height: 400px;
}
.containerVideoTop .videoTop {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 15px;
}

@media screen and (min-width: 820px) {
  .containerVideoTop {
    min-height: 70vh;
    position: relative;
    min-width: 200px;
  }
}

@media screen and (min-width: 1024px) {
  .containerVideoTop {
    min-height: 70vh;
    position: relative;
    min-width: 200px;
    width: 60%;
  }
}
</style>