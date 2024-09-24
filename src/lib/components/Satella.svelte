<script lang="ts">
  // import { onMount } from 'svelte';

  // onMount(() => {
  //   const stella = document.querySelectorAll('.satella');
  //   stella.forEach((satella, i) => {
  //     satella.style.top = `${Math.random() * 100}vh`;
  //     satella.style.left = `${Math.random() * 100}vw`;
  //     satella.style.animationDuration = `${Math.random() * 2 + 3}s`;
  //     satella.style.animationDelay = `${Math.random()}s`;
  //   });
  // });
</script>

<section id="sky" class="relative w-full h-full bg-white">
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
  <span class="satella"></span>
</section>

<style>
  .satella{
    position: absolute;
    top: 50%;
    left: 50%;
    width: 4px;
    height: 4px;
    background: #000;
    border-radius: 50%;
    box-shadow: 0 0 0 4px #fff;
    z-index: 10;
    animation: animate 3s linear infinite;
    /* box-shadow: 0 0 0 4px rgba(0, 0, 0, 1), 0 0 0 8px rgba(0, 0, 0, 0.1), 0 0 20px rgba(0, 0, 0, 1)  ;
    &::after{
      content: '\d7';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 0;
      &::after{
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        box-shadow: 0 0 0 4px #000;
      }
    } */
  }
  .satella::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 250%;
    transform: translateY(-50%);
    width: 300px;
    height: 1px;
    background: linear-gradient(9deg, #000, transparent);
  }
  @keyframes animate {
    0% {
      transform: rotate(315deg) translateX(0);
      opacity: 1;
    }
    70% {
      opacity: 1;
    }
    100% {
      transform: rotate(315deg) translateX(-1000px);
      opacity: 0;
    }
  }
  
  .satella:nth-child(1){
      top: 0;
      right: 0;
      left:initial;
      animation-delay:0 ;
      animation-duration: 1s;
  }
  
  .satella:nth-child(2){
      top: 0;
      right: 80px;
      left:initial;
      animation-delay:0.2s;
      animation-duration: 3s;
  }
  
  .satella:nth-child(3){
      top: 80px;
      right: 0px;
      left:initial;
      animation-delay:0.4s ;
      animation-duration: 2s;
  }
  
  .satella:nth-child(4){
      top: 0;
      right: 180px;
      left:initial;
      animation-delay:0.6s;
      animation-duration: 1.5s;
  }
  
  .satella:nth-child(5){
      top: 0;
      right: 400px;
      left:initial;
      animation-delay:0.8s;
      animation-duration: 2.5s;
  }
  
  .satella:nth-child(6){
      top: 0;
      right: 600px;
      left:initial;
      animation-delay:1s ;
      animation-duration: 3s;
  }
  .satella:nth-child(7 ){
      top: 300px;
      right: 0px;
      left:initial;
      animation-delay:1s ;
      animation-duration: 1.75s;
  }
  
  .satella:nth-child(8){
      top: 0px;
      right: 700px;
      left:initial;
      animation-delay:1.4s ;
      animation-duration: 1.25s;
  }
  
  .satella:nth-child(9){
      top: 0px;
      right: 1000px;
      left:initial;
      animation-delay:0.75s ;
      animation-duration: 2.25s;
  }
  
  .satella:nth-child(10){
      top: 0px;
      right: 1000px;
      left:initial;
      animation-delay:2.75s ;
      animation-duration: 2.25s;
  }
</style>