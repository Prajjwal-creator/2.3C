<template>
    <div id="app">
        <!-- Place your template syntax code here -->
        <h1>{{ message }}</h1>
        <div v-html="htmlContent"></div>
        <div :id="dynamicId"></div>
        <p>{{ computedValue }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: "Text Interpolation",
            htmlContent: "<strong>Raw HTML</strong>",
            dynamicId: "myDynamicId",
        };
    },
    computed: {
        computedValue() {
            return "Computed Value";
        },
    },
};
</script>

<style scoped>
/* Add scoped CSS here or import an external CSS file */
</style>
