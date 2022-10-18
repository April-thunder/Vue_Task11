<template>
  <TheHeader />
  <TheMainSection />
  <TheDishesSection />
  <TheSlidesSection />
  <TheFormSection />
  <TheFooter />
</template>

<script>
    import TheHeader from "./components/TheHeader.vue";
    import TheMainSection from "./components/TheMainSection.vue";
    import TheDishesSection from "./components/TheDishesSection.vue";
    import TheSlidesSection from "./components/TheSlidesSection.vue";
    import TheFormSection from "./components/TheFormSection.vue";
    import TheFooter from "./components/TheFooter.vue";

    export default {
        components: {
            TheHeader,
            TheMainSection,
            TheDishesSection,
            TheSlidesSection,
            TheFormSection,
            TheFooter,
        },
    };
</script>
