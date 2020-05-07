<template>
  <div class="skill">
    <div class="skill__wrapper">
      <div class="skill__ico">
        <i v-if="awesome" :class="[icon, 'fa-2x']"></i>
        
      </div>
      <div class="skill__name">{{ name }}</div>
    </div>
  </div>
</template>

<script>

export default {
  name: "Skill",
  props: {
    name: {
      type: String
    },
    icon: {
      type: String
    },
    awesome: {
      type: Boolean
    }
  },
};
</script>

<style lang="scss" scoped>
.skill {
  //   border: 4px solid red;
  border-radius: 200px;
  width: 8rem;
  
  box-sizing: content-box;
  margin: 1em;
  &__ico {
    color: var(--text-primary);
    // border: 4px solid blue;
    font-size: 3rem;
  }
  &__wrapper {
    // border: 4px solid pink;
    
    flex-direction: column;
    justify-content: space-between;
    position: relative;
    z-index: 4;
  }
  &__name {
    
    font-family: futura-pt, sans-serif;
    font-weight: 200;
    font-style: normal;
    font-size: 1.5rem;
    padding-bottom: 0.6em;
    width: 130%;
    color: var(--text-secondary);
  }
  //   .psd {
  //     // fill: var(--text-primary);
  //     background-image: url("../assets/skills_ico/iconfinder_logo_brand_brands_logos_adobe_photoshop_1907196.svg");
  //     height: 1.8em;
  //     width: 1.8em;
  //   }
}
</style>