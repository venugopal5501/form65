<template>
    <h1>Computed Property</h1>
    <h3>{{ getResult }}</h3>
</template>
<script>
export default {
    name: "yesNo",
    data() {
        return {
            name: "Sciene",
        }
    },

    computed: {
        getResult() {
            return this.name.split("").reverse("").join("")
        }
    }
}
</script>


<style></style>
