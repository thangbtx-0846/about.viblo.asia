<template>
  <section id="first-section"
    class="relative near-full-height">
    <div id="brand" class="flex flex-col absolute">
      <img src="../assets/logo.svg" alt="Viblo Logo" id="logo" class="mb-3">
      <div class="text-center select-auto"><strong>Free</strong> service for technical knowledge <strong>sharing</strong></div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
  #first-section {
    background: radial-gradient(#003dbd, #01001e);

    &:after {
      content: "";
      background: url(../assets/viblo-pattern-art.svg) left bottom no-repeat;
      mix-blend-mode: screen;
      opacity: 0.25;
      top: 0;
      left: 0;
      bottom: 0;
      right: 0;
      position: absolute;
    }

    #brand {
      left: 50%;
      top: 32%;
      transform: translateX(-50%);
      color: #7acaff;
      z-index: 2;
    }
  }

  .near-full-height {
    height: 90vh;
  }

  @media (max-width: 800px) {
    .near-full-height {
      height: 45vh;
    }
  }
</style>
