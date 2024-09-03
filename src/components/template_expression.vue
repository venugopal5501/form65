<template>
    <h1>Venugopal</h1>
    <h2>{{ name.split("").reverse("").join("") }}</h2>
</template>

<script>
export default {
    name: 'computeProperty',
    data() {
        return {
            name: "VenuGopal"
        }
    }
}
</script>
<style></style>