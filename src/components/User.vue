<template>
    <div id="user">
        <h3>Anand</h3>
        <h3>Bala</h3>
        <h3>Dinesh</h3>
        <h3 v-bind="$attrs">Kumar</h3>
    </div>
</template>
<script>
export default {
    name: 'userPage',
}
</script>
<style scoped>
#user {
    text-align: left;
}

h3 {
    color: blue;
}
</style>