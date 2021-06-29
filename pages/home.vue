<template>
  <div class="container-center">
    <div>
      <div class="flex flex-row justify-between items-center py-5">
        <div>
          <span class="title">
            <span class="color-text-primary">Leonardo</span> Antonio <br />
            Nolasco Leyva
          </span>
          <div>
            <span class="subtitle">DESARROLLADOR DE SOFTWARE</span>
          </div>
          <div class="pt-3">
            <button class="btn-primary">Contactar</button>
          </div>
        </div>
        <div>
          <img src="../assets/logo-main.svg" alt="logo-main" />
        </div>
      </div>
    </div>

    <div class="w-full" id="skills">
      <div>
        <div class="text-center py-10">
          <h4 class="items-title">Skills</h4>
        </div>
      </div>
      <div>
        <div class="grid grid-rows-3 grid-cols-4 gap-12">
          <div class="w-full flex justify-center">
            <img src="../assets/skills/gopher.svg" alt="golang" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/nodejs.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/nestjs.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/mongodb.svg" alt="" />
          </div>

          <div class="w-full flex justify-center">
            <img src="../assets/skills/docker.png" alt="golang" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/github.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/mysql.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/digital-ocean.svg" alt="" />
          </div>

          <div class="w-full flex justify-center">
            <img src="../assets/skills/javascript.svg" alt="golang" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/typescript-icon.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/vue.svg" alt="" />
          </div>
          <div class="w-full flex justify-center">
            <img src="../assets/skills/nuxt-icon.svg" alt="" />
          </div>
        </div>
      </div>
    </div>

    <div class="w-full" id="projects">
      <div class="text-center py-10">
        <h4 class="items-title">Proyectos</h4>
      </div>

      <div>
        <div class="flex flex-row justify-between">
          <div v-for="item of projects" :key="item">
            <CardComponent :title="item.title" :text="item.text" />
          </div>
        </div>
      </div>
    </div>

    <div id="form">
      <div class="text-center pt-10">
        <h4 class="items-title">Trabajemos</h4>
      </div>

      <div class="pb-10">
        <div class="w-full flex justify-center">
          <div class="container-form">
            <div class="py-2">
              <input
                placeholder="Ingrese sus nombres"
                type="text"
                class="input w-full px-5"
              />
            </div>
            <div class="py-2">
              <input
                placeholder="Ingrese sus apellidos"
                type="text"
                class="input w-full"
              />
            </div>
            <div class="py-2">
              <textarea
                placeholder="Mensaje o consulta"
                row="40"
                class="input w-full"
              ></textarea>
            </div>
            <div>
              <button class="btn-primary-auto">Enviar</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'profile',
  data() {
    return {
      projects: [
        {
          title: 'Project 1',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum deserunt eum voluptatem reprehenderit tempore dolor nihil repudiandae, neque eos, facilis aspernatur',
        },
        {
          title: 'Project 2',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum deserunt eum voluptatem reprehenderit tempore dolor nihil repudiandae, neque eos, facilis aspernatur',
        },
        {
          title: 'Project 3',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum deserunt eum voluptatem reprehenderit tempore dolor nihil repudiandae, neque eos, facilis aspernatur',
        },
        {
          title: 'Project 3',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum deserunt eum voluptatem reprehenderit tempore dolor nihil repudiandae, neque eos, facilis aspernatur',
        },
      ],
    }
  },
}
</script>

<style>
.container-form {
  display: flex;
  justify-content: center;
  flex-direction: column;
  width: 400px;
}
</style>
