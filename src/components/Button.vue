<script setup lang="ts">
interface Props {
    msg: string;
}

const props = defineProps<Props>();
const { msg } = props;
</script>

<template>
    <div>
        <button type="button" :class="$style.button">{{ msg }}</button>
    </div>
</template>

<style module>
.button {
    border: 0.1rem solid red;
    background-color: white;
}
</style>
