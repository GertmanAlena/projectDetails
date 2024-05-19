<template>
  <div>
    <img class="banner-image" :src="require(`@/assets/${imageBanner}`)" alt="imageBanner">

  </div>
</template>

<script>
import { mapState } from 'vuex';
export default {
  name: 'BannerComponentProjectDetails',

  data() {
    return {

    };
  },

  mounted() {

  },
  computed: {
    ...mapState(['imageBanner']),
  },

  methods: {
    imgUrl() {
      return require(`@/assets/${this.imageBanner}`)
    },
  },
};
</script>
<style>
.banner {
  padding-left: calc(50% - 1200px/2);
  padding-right: calc(50% - 1200px/2);
  margin-top: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.banner-image{
  padding-left: calc(50% - 2000px / 2);
  padding-right: calc(50% - 1200px / 2);
}
.banner__heading {
  width: 658px;
  height: 437px;
  /* Автолейаут */
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  padding-bottom: 90px;

  /* Inside Auto Layout */
  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 42px;

}

.title-project-details {
  color: rgb(41, 47, 54);
  font-family: DM Serif Display;
  font-size: 50px;
  font-weight: 400;
  line-height: 125%;
  letter-spacing: 2%;
  text-align: left;
  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 11px 0px;
}

.text-project-details {
  color: rgb(77, 80, 83);
  font-family: Jost;
  font-size: 22px;
  font-weight: 400;
  line-height: 150%;
  letter-spacing: 1%;
  text-align: left;
  flex: none;
  order: 1;
  flex-grow: 0;
  margin: 11px 0px;
  width: 658px;
  height: 363px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  padding: 0px;
  text-align: justify;
}
.image-banner{
  
}
</style>