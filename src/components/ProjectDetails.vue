<template>
    <div class="projectDetails">
        <div :class="projectDetail.class" v-for="projectDetail in projectDetails" :key="projectDetail.id">
            <div class="banner__heading">
                <h2 :class="projectDetail.titleClass">{{ projectDetail.title }}</h2>
                <p :class="projectDetail.descriptionClass">{{ projectDetail.description }}</p>
            </div>
        </div>
        <CarouselComponent />
    </div>
</template>

<script>
import CarouselComponent from './CarouselComponent.vue'
import { mapState } from 'vuex';
export default {
    name: 'FinalExaminationProjectDetails',

	components: { CarouselComponent },
    data() {
        return {

        };
    },

    computed: {
        ...mapState(['projectDetails']),
    },

    methods: {

    },
};
</script>
<style>
    .projectDetails{
        margin-bottom: 200px;
    }
</style>