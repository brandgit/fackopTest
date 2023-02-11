<template>
  <div class="containerVideo">
    <video
      autoplay="true"
      loop="true"
      class="video"
      src="/Video/Fackopvideobg1.mp4"
    />
    <div
      class="flex flex-col top-[25%] sm:top-[35%] lg:top-[30%] absolute w-full z-1 bg-blck"
    >
      <div
        class="w-[70%] ml-[5%] sm:w-[600px] sm:text-[25px] md:w-[650px] md:text-[35px] lg:w-[900px] xl:w-[900px] text-[20px] lg:text-[45px] text-white font-bold"
      >
        <p>
          Dans le but de développer des solutions numériques et informatiques,
          <br />
          Le GROUPE FACKOP se mets à votre disposition en vous proposant une
          diversité de services.
        </p>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.containerVideo {
  min-height: 100vh;
  position: relative;
  min-width: 330px;
}
.containerVideo .video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.contenent {
  position: relative;
  animation: carousel 10s ease-in-out infinite;
}

@keyframes carousel {
  0%,
  20% {
    transform: translateY(0);
  }
  25%,
  45% {
    transform: translateY(-25px);
  }
  50%,
  70% {
    transform: translateY(-50px);
  }
  75%,
  95% {
    transform: translateY(-75px);
  }
  100% {
    transform: translateY(-100px);
  }
}

@media screen and (min-width: 640px) {
  @keyframes carousel {
    0%,
    20% {
      transform: translateY(0);
    }
    25%,
    45% {
      transform: translateY(-30px);
    }
    50%,
    70% {
      transform: translateY(-60px);
    }
    75%,
    95% {
      transform: translateY(-90px);
    }
    100% {
      transform: translateY(-120px);
    }
  }
}
</style>
