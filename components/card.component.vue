<template>
  <div>
    <div class="card-container shadow-md flex justify-center items-center">
      <div>
        <h4 class="text-center title-card color-primary">{{ title }}</h4>
        <p class="text-card text-center">
          {{ text }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardComponent',
  props: {
    title: {
      type: String,
    },
    text: {
      type: String,
    },
  },
}
</script>

<style>
.card-container {
  width: 250px;
  height: 250px;
}

.title-card {
  font-family: Saira;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 39px;
}

.text-card {
  font-family: Roboto;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 20px;
  color: #000000;
}
</style>
