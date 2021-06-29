<template>
  <div class="container-center">
    <div class="py-5">
      <div class="flex justify-between">
        <div>
          <span class="text-logo">
            { <span class="color-text-primary">Leo</span>nardo }
          </span>
        </div>

        <div>
          <span class="px-2 item-menu">
            <a href="#">Home</a>
          </span>
          <span class="px-2 item-menu">
            <a href="#skills">Skills</a>
          </span>
          <span class="px-2 item-menu">
            <a href="#projects">Proyectos</a>
          </span>
          <span class="px-2 item-menu">
            <a href="#">Trabajemos</a>
          </span>
        </div>
      </div>
    </div>
    <Nuxt />

    <div class="fixed right-0 bottom-30">
      <div>
        <span class="px-1">
          <a href="https://github.com/Leonardo-Antonio" target="_blank">
            <img width="40px" src="../assets/github.svg" alt="github" />
          </a>
        </span>
        <span class="px-1">
          <img width="40px" src="../assets/linkedin.svg" alt="linkedin" />
        </span>
        <span class="px-1">
          <a href="mailto:leo2001.nl08@gmail.com">
            <img width="40px" src="../assets/mail.svg" alt="mail" />
          </a>
        </span>
        <span class="px-1">
          <a href="https://wa.me/996501260" target="_blank">
            <img width="40px" src="../assets/wsp.svg" alt="wsp" />
          </a>
        </span>
      </div>
    </div>
  </div>
</template>

<style>
.bottom-30 {
  bottom: 30%;
}
</style>
