<template>
    <div :class="color">
        <h2 @mouseover="incrementCount">Hovered {{ count }} times </h2>
    </div>
</template>

<script>
import myMixin from '../mixins/myMixin'
export default {
name: 'HoverCounter',
mixins: [myMixin],
data() {
    return {
        color: 'blue'
    }
}
}
</script>

<style>
.blue{
    background: blue;
    color:blanchedalmond
}
</style>